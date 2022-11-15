# Local Enumeration

### tty

`python3 -c 'import pty; pty.spawn("/bin/bash")'`

### ssh

**id\_rsa** file that contains a private key that can be used to connect to a box via ssh.

It is usually located in the `.ssh` folder in the user's home folder. (Full path: `/home/user/.ssh/id_rsa`)

Get that file on your system and give it read/write-only permissions for your user:\
(`chmod 600 id_rsa`) and connect by executing `ssh -i id_rsa user@ip`).

Execute `ssh-keygen` and you should see **id\_rsa** and `id_rsa.pub` files appear in your own **.ssh** folder.

Copy the content of the **id\_rsa.pub** file and put it inside the **authorized\_keys** file on the target machine (located in .ssh folder). After that, connect to the machine using your id\_rsa file.

### Basic enumeration

Execute `uname -a` to print out all information about the system.

**.bash\_profile** and **.bashrc** are files containing shell commands that are run when Bash is invoked.&#x20;

Execute `sudo -V` to retrieve the version. Its version can help you identify known exploits and vulnerabilities.&#x20;

Run `sudo -l` to check if a user on the box is allowed to use sudo with any command on the system.&#x20;

### /etc

`cat /etc/passwd` It's a plain-text file that contains a list of the system's accounts, giving for each account some useful information like user ID, group ID, home directory, shell, and more.

**Example:**

`goldfish:x:1003:1003:,,,:/home/goldfish:/bin/bash`

1. (goldfish) - Username
2. (x) - Password. (x character indicates that an encrypted account password is stored in /etc/shadow file and cannot be displayed in the plain text here)
3. (1003) - User ID (UID): Each non-root user has his own UID (1-99). UID 0 is reserved for root.
4. (1003) - Group ID (GID): Linux group ID
5. (,,,) - User ID Info: A field that contains additional info, such as phone number, name, and last name. (,,, in this case means that I did not input any additional info while creating the user)
6. (/home/goldfish) - Home directory: A path to user's home directory that contains all the files related to them.
7. (/bin/bash) - Shell or a command: Path of a command or shell that is used by the user. Simple users usually have /bin/bash as their shell, while services run on /usr/sbin/nologin.

The `/etc/shadow` file stores actual password in an encrypted format (aka hashes) for user’s account with additional properties related to user password.

**Example:**

`goldfish:$6$1FiLdnFwTwNWAqYN$WAdBGfhpwSA4y5CHGO0F2eeJpfMJAMWf6MHg7pHGaHKmrkeYdVN7fD.AQ9nptLkN7JYvJyQrfMcfmCHK34S.a/:18483:0:99999:7:::`

1. (goldfish) - Username
2. ($6$1FiLdnFwT...) - Password : Encrypted password. Basic structure: **$id$salt$hashed**, The $id is the algorithm used On GNU/Linux as follows:
   * $1$ is MD5
   * $2a$ is Blowfish
   * $2y$ is Blowfish
   * $5$ is SHA-256
   * $6$ is SHA-512
3. (18483) - Last password change: Days since Jan 1, 1970 that password was last changed.
4. (0) - Minimum: The minimum number of days required between password changes (Zero means that the password can be changed immidiately).
5. (99999) - Maximum: The maximum number of days the password is valid.
6. (7) - Warn: The number of days before the user will be warned about changing their password.

`/etc/host`s is a simple text file that allows users to assign a hostname to a specific IP address.

### SUID (Set User ID)

`find / -perm -u=s -type f 2>/dev/null`

\-u=s searches files that are owned by the root user.\
\-type f search for files, not directories

### Port Forwarding

&#x20;In order to see all TCP connections, execute `netstat -at | less`

`netstat -tulpn` will provide you a much nicer output with the most interesting data.

### Automating scripts

**Linpeas**

`wget https://raw.githubusercontent.com/carlospolop/privilege-escalation-awesome-scripts-suite/master/linPEAS/linpeas.sh`

**LinEnum**

`wget https://raw.githubusercontent.com/rebootuser/LinEnum/master/LinEnum.sh`

\








