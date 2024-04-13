# Questions

1.  You need to delete a user from the system, including their home directory. Which of the following utility commands accomplishes this task?

    1. `userdel`
    2. `userdel -r`
    3. `userdel -R`
    4. `deluser`

    Answer:

    B.  The `userdel` command is used for this purpose, and the `-r` option (lowercase) deletes both the home directory and mail spool files. The `-R` (uppercase) option informs the `userdel` command to use a `chroot` directory.
2.  You need to enable the web server (running as the `www-data` user and group) to write into a directory called `/home/webfiles`. Which commands will accomplish this task in the most secure manner?

    1. `chgrp www-data /home/webfiles ; chmod 775 /home/webfiles`
    2. `chmod 777 /home/webfiles`
    3. `chgrp www-data /home/webfiles ; chmod 711 /home/webfiles`
    4. `chmod 707 /home/webfiles`

    Answer:

    A.  The best option among these choices is to change the group to `www-data` and change the permissions such that the group can write into the directory. Option B should never be used because it enables world-writing to the directory. The other options will not allow the web server group to write into the directory.
3.  Assume that passwords must be changed every 60 days. Which command will change the date of the user's last password change without the user actually changing the account password?

    1. `chage -f`
    2. `chage -W`
    3. `chage -l`
    4. `chage -d`

    Answer:

    D.  The `chage` command is used for this purpose. The `-d` option sets the days since the last password change and is measured in days since January 1, 1970. The `-W` option is the days of warning for changing a password, and the `-l` option displays a list of the various settings related to the account. There is no `-f` option.
4.  What is the order in which user configuration files are located on login to a Bash shell?

    1. `.bash_login`, `.profile`, `/etc/profile`
    2. `.bash_profile`, `.bash_login`, `.profile`
    3. `.profile`, `.bash_login`, `.bash_profile`
    4. `.bash_login`, `.bash_profile`, `.profile`

    Answer:

    B.  User-based configuration files are located in the order `.bash_profile`, `.bash_login`, and `.profile`. Only the first file found is executed; the others are ignored. The file `/etc/profile` is a system-wide bash profile.
5.  Within which directory should you place files to have them automatically copied to a user's home directory when the user is created?

    1. `/etc/userhome`
    2. `/etc/templateuser`
    3. `/etc/skel`
    4. `/home/skel`

    Answer:

    C.  The `/etc/skel` directory contains files to be copied to the user's home directory. The other directories listed for this question do not exist by default.
6.  Which bash parameter or option will cause the shell to be executed without reading the initialization files?

    1. `--no-rc`
    2. `--no-init`
    3. `--norc`
    4. `--rc-none`

    Answer:

    C.  The `--norc` option causes bash to execute without reading the `/etc/bash.bashrc` (Debian derivatives) or `/etc/bashrc` (Red Hat derivatives) file or the local `~/.bashrc` file. The other options listed do not exist as options for bash, which is the default shell on most popular Linux distributions.
7.  You need to create a function that will be available each time you log in to the system. Within which file should this function be placed?

    1. `.bash_profile`
    2. `.rc`
    3. `/etc/profile`
    4. `.bash_run`

    Answer:

    A.  The `.bash_profile` file, if it exists in your home directory, will be executed on login. Note that placing the function in `/etc/profile` would technically work, but then the function would be available to all users, which is not what the question asked for.
8.  Assuming X forwarding has been enabled on the SSH server, which environment variable is used to set the location for newly spawned windows from within an SSH session?

    1. `DISPLAY`
    2. `XTERMINAL`
    3. `XTERM`
    4. `XDISP`

    Answer:

    A.  The `DISPLAY` variable can be used to remotely send the windows of an X session to another computer when using protocols like SSH. There is no `XTERMINAL` or `XDISP` environment variable, and `XTERM` is typically a terminal window and not an environment variable.
9.  Which of the following options in the SSH configuration file needs to be enabled so that X sessions can be sent over an SSH connection?

    1. `X11Connect yes`
    2. `X11Forwarding yes`
    3. `ForwardX yes`
    4. `XForward yes`

    Answer:

    B.  The `X11Forwarding` option must be enabled in order for X connections or windows generated from the X server to be sent over an SSH connection.
10. Which file contains user information such as username and real name and is readable by all users of the system?

    1. `/etc/pass`
    2. `/etc/shadow`
    3. `/etc/passwd`
    4. `/etc/userinfo`

    Answer:

    C.  The `/etc/passwd` file contains various information about users on a system such as username and real name, along with user ID (UID) and login shell. The file is world-readable. The `/etc/shadow` file contains encrypted passwords but is not readable by all users. The other two files shown as options do not exist by default.
11. Which of the following commands changes a group called `DomainAdmins` to `DomainUsers`?

    1. `groupmod -n DomainUsers DomainAdmins`
    2. `groupchg DomainAdmins DomainUsers`
    3. `chgroup DomainAdmins DomainUsers`
    4. `group -N DomainAdmins DomainUsers`

    Answer:

    A.  The `groupmod` command is used for this purpose, and the `-n` option is used to change the group name. The other commands listed do not exist.
12. When running `useradd`, which option needs to be specified in order for the user's home directory to be created?

    1. `-h`
    2. `-m`
    3. `-x`
    4. `-a`

    Answer:

    B.  The `-m` option causes the user's home directory to be created. By default, if this option isn't specified and `CREATE_HOME` has not been set, the `home` directory won't be created. The `-h` option displays help text, and the other options shown are not valid.
13. Which of the following commands locks out password-based login for a user but does not prevent other forms of login?

    1. `usermod -L`
    2. `userdel -r`
    3. `useradd -h`
    4. `userlock`

    Answer:

    A.  The `usermod -L` command locks an account by placing an `!` in the encrypted password. If the user has another means to log in, such as with an SSH key, using `usermod -L` will not prevent their login. Among the other answers, `userdel -r` deletes a user and `useradd -h` displays help related to adding a user to the system. There is no `userlock` command.
14. Which of the following commands produces a report listing the last password change date for all users on the system?

    1. `passwd -a`
    2. `passwd -S`
    3. `passwd -a -S`
    4. `passwd --all`

    Answer:

    C.  The `passwd` command will be used for this purpose. The `-a` option displays all users but requires the use of `-S` to indicate status. The `-S` option alone will not produce a report for all users, and the `--a`ll option is an alias for `-a`.
15. Which file contains a list of usernames, UIDs, and encrypted passwords?

    1. `/etc/passwd`
    2. `/etc/shadow`
    3. `/etc/encpass`
    4. `/etc/grouppass`

    Answer:

    B.  The `/etc/shadow` file contains usernames, UIDs, and encrypted passwords and is not readable by any non-root user on the system due to the sensitive nature of the encrypted passwords. The `/etc/passwd` file contains usernames and UIDs but not encrypted passwords. The other two files listed for this question do not exist.
16. Which command is used to change a user's home directory to `/srv/data/username` and move the contents at the same time?

    1. `usermod -d /srv/data/username -m`
    2. `homedir -m /srv/data/username`
    3. `userex -m /srv/data/username`
    4. `userchg /m /srv/data/username -d`

    Answer:

    A.  The `usermod` command is used for this purpose. The `-d` option changes the home directory from its normal location at `/home`. The `-m` option moves the contents. The other commands shown for this question are not valid.
17. Which option to `useradd` will add groups for a user?

    1. `-g`
    2. `-x`
    3. `-l`
    4. `-G`

    Answer:

    D.  The `-G` option is a list of supplemental groups to which the user will be added. A lowercase `-g` option provides the primary GID. The `-l` option causes the user to not be added to the `lastlog` and `faillog` databases. There is no `-x` option.
18. Which option to `useradd` creates a system user rather than a normal user?

    1. `-r`
    2. `-s`
    3. `-a`
    4. `-S`

    Answer:

    A.  The `-r` option creates a system user, which will typically entail no expiration, no home directory, and a UID below 1000. The `-s` option defines the shell and is not typically used for this purpose. The `-a` and `-S` options do not exist.
19. Which file contains encrypted password information for groups?

    1. `/etc/group`
    2. `/etc/gshadow`
    3. `/etc/gsecure`
    4. `/etc/group.conf`

    Answer:

    B.  The `/etc/gshadow` file contains secure information such as an encrypted password for groups, where applicable. The `/etc/group` file contains general information on groups. The other two files listed as options do not exist.
20. Which of the following best describes a valid use of the `groupdel` command?

    1. You may force group deletion with the `-f` option.
    2. If a user's primary group is to be deleted, that user must be deleted first or have their primary group changed.
    3. `Groupdel` can be run at any time, regardless of group membership.
    4. The `-r` option for `groupdel` will recursively change users’ GIDs after group deletion.

    Answer:

    B.  The `groupdel` command cannot delete groups unless there are no users who have the given group as their primary GID. Therefore, option B best fits the scenario. There is no `-f` or `-r` option, making options A and D incorrect.
21. Which of the following commands displays the UID, primary group, and supplemental groups for a given user?

    1. `id`
    2. `getid`
    3. `passwd`
    4. `chage`

    Answer:

    A.  The `id` command shows the username, UID, primary group, and GID along with supplemental groups. The `passwd` and `chage` commands are not used for this purpose. There is no `getid` command.
22. Which option to the `usermod` command is used to change a given user's real name?

    1. `-R`
    2. `-n`
    3. `-d`
    4. `-c`

    Answer:

    D.  The `-c` option changes the comment field in `/etc/passwd`. The comment field is typically associated with the real name of the account. The `-R` option indicates a `chroot` directory, while `-d` indicates a change of home directory. There is no `-n` option.
23. A user needs to work with printers and printer-related items. Which of the following commands adds the user (called `username` in the options) to the appropriate group for this purpose?

    1. `usermod -aG printerusers username`
    2. `usermod -aG lpadmin username`
    3. `usermod -gA lpadm username`
    4. `usermod -a lpadm username`

    Answer:

    B.  The `usermod` command with the `-aG` option is used to append a group onto the user's list of groups. In this case, the user needs to be a member of the `lpadmin` group.
24. You need to examine who is currently logged in to the system. Which of the following commands will display this information?

    1. `listuser`
    2. `fuser`
    3. `ls -u`
    4. `w`

    Answer:

    D.  The `w` command shows currently logged-in users along with information such as uptime and load average and is similar to the `who` command. The `fuser` command is used to show open files, and the `-u` option to `ls` controls the display for file listings. There is no `listuser` command.
25. Within the following entry in `/etc/shadow`, to what does the number 15853 refer? `mail:*:15853:0:99999:7:::`

    1. The UID of the mail user
    2. The number of files owned by mail
    3. The date of the last password change (since 1/1/1970)
    4. The number of days until the account expires

    Answer:

    C.  The date of the last password change, as measured in days since January 1, 1970, is contained in the third field of a `shadow` entry. The expiration date would be the eighth field, as separated by colons.
26. Which of the following commands displays a listing of who is logged in to the server along with the date and time that they logged in?

    1. `whois`
    2. `who`
    3. `loggedin`
    4. `curusers`

    Answer:

    B.  The `who` command displays who is currently logged in and the date and time they logged in. The `whois` command displays information about domains. The other commands are not valid.
27. Which of the following commands adds a group?

    1. `groupadd`
    2. `addgrp`
    3. `grpadd`
    4. `creategroup`

    Answer:

    A.  The `groupadd` command is used to add a group to the system. The other options shown are not valid.
28. Which of the following commands enables the sticky bit for a user on a file called `homescript.sh`?

    1. `chmod +sticky homescript.sh`
    2. `chmod 755 homescript.sh`
    3. `chmod u+t homescript.sh`
    4. `chown u+sticky homescript.sh`

    Answer:

    C.  The sticky bit is set using `+t`. For this question, the user permission is being affected, thus the `u` as an argument to `chmod`. Among the other answers, the `chown` command is valid but changes ownership, not permissions, and thus isn't used for the purpose described in the question.
29. The umask reports as 022. What is the permission that will be in effect for a newly non-executable created file?

    1. `u+rw, g+r, w+r`
    2. 755
    3. 644
    4. `a+r`

    Answer:

    C.  The 022 umask will translate into 644 permissions on a new non-executable file.
30. Which of the following best describes the relationship between UIDs and GIDs on a Linux system when an authentication server is being configured?

    1. The UID and GID are the same across the system for a given user.
    2. Each user has a UID and GID that are the same and are created when the user is created.
    3. The UID represents the user, while the GID is a globally unique user ID.
    4. There is no direct relationship between UID and GID.

    Answer:

    D.  There is no direct relationship between the UIDs and GIDs on a system. UIDs represent users, while GIDs represent group IDs. On some systems, the UID and GID numbers will match for regular users, but this is not a requirement and is more of a coincidence.
31. When you're configuring a server for an SNMP server role, which ports need to be allowed through the firewall for SNMP traffic?

    1. Ports 23 and 25
    2. Ports 110 and 143
    3. Ports 80 and 443
    4. Ports 161 and 162

    Answer:

    D.  SNMP traffic takes place on ports 161 and 162. Although the traffic is usually on UDP, the TCP ports are also reserved for SNMP. Ports 110 and 143 are used for POP3 and IMAP, respectively, while 23 and 25 are Telnet and SMTP. Finally, ports 80 and 443 are HTTP and HTTPS.
32. You need to look at information on logins beyond what was captured by the current log file for the last command. Which option to the last command can be used to load information from an alternate file?

    1. `-a`
    2. `-t`
    3. `-e`
    4. `-f`

    Answer:

    D.  Loading of alternate files is accomplished using the `-f` option. Doing so facilitates exactly the scenario described: being able to examine logins from old log files. The `-a` option controls the location of the display for the host, while `-t` controls the display to show the logins as of the specified date and time. There is no `-e` option.
33. When creating a certificate authority server role, which of the following commands generates a private key for use with SSL and places it into the file `/etc/ssl/example.com.private`?

    1. `openssl genrsa -out /etc/ssl/example.com.private`
    2. `openssl generate-private > /etc/ssl/example.com.private`
    3. `openssl genpriv > /etc/ssl/example.com.private`
    4. `openssh genkey -out /etc/ssl/example.com.private`

    Answer:

    A.  The `openssl` command will be used for this purpose, with the `genrsa` option. An output file is specified with `-out`. The other commands containing `openssl` all contain an invalid option. The final command is `openssh` and is not used for this scenario.
34. Which of the following options within an OpenSSH server configuration is used to determine whether the root user can log in directly with an SSH client?

    1. `PermitRootLogin`
    2. `AllowRoot`
    3. `RootLogin`
    4. `PermitDirectRootLogin`

    Answer:

    A.  The `PermitRootLogin` directive, set to `yes` or `no`, determines whether the root user can log in directly. This option is set within the server configuration file at `/etc/ssh/sshd_config`. In general, server-wide configuration files for SSH are stored in `/etc/ssh` while user-specific configuration files are stored in each user's home directory. The other options shown are not valid.
35. Which option to `ssh` creates a port forwarding to which remote clients can also connect?

    1. `-L`
    2. `-R`
    3. `-P`
    4. `-E`

    Answer:

    B.  The `-R` option creates a port forward and enables remote clients to connect. The `-L` option also creates a port forward but does not allow remote clients to connect. The `-P` and `-E` options are not valid for this scenario.
36. Which subcommand of `openssl` is used to create a Certificate Signing Request (CSR) for Secure Sockets Layer (SSL)/Transport Layer Security (TLS)?

    1. `req`
    2. `csr`
    3. `gencsr`
    4. `newcsr`

    Answer:

    A.  The `req` option begins the CSR generation process, typically also requiring `-new` as an additional option. The other subcommands are not valid.
37. Within which directory should scripts and other files to run at login be stored?

    1. `/etc/login`
    2. `/etc/profile`
    3. `/etc/bash.defs`
    4. `/etc/profile.d`

    Answer:

    D.  The `/etc/profile.d` directory can be used to store files and scripts that are then executed on login. Of the other answers, `/etc/profile` does exist, but it is a file and not a directory. The other answers are not valid directories.
38. Using udev to configure a network adapter for use with a firewall so that it has a specific and consistent name, you edit the udev rules file. Which option within the rules file ensures that the device will always have a name of `eth0`?

    1. `ATTR-NAME=“eth0”`
    2. `NAME=“eth0”`
    3. `DEV_NAME=“eth0”`
    4. `NAME_DEV=“eth0”`

    Answer:

    B.  The `NAME` parameter sets the name for the device. The other options shown are not valid udev parameters.
39. You are configuring a database service and need to open the default port for MySQL on the firewall. Which port is the default for MySQL?

    1. 6592
    2. 25
    3. 389
    4. 3306

    Answer:

    D.  Port 3306 is the default port for MySQL. Of the other options, 25 is SMTP, and 389 is typically used with LDAP.
40. When configuring Apache for a web server role, which of the following directives tells the server the location of the SSL private key?

    1. `SSLKeyFile`
    2. `SSLCertificatePrivateKey`
    3. `SSLCertificateKeyFile`
    4. `SSLPrivateKey`

    Answer:

    C.  The `SSLCertificateKeyFile` directive points to the location of the private key for an SSL configuration. The other options shown are not valid directives.
41. Which of the following commands will correctly change the group ownership of the file called `a.out` to users?

    1. `chgrp users a.out`
    2. `chgrp a.out users`
    3. `groupchg a.out users`
    4. `grpchg users a.out`

    Answer:

    A.  The `chgrp` command can be used to change group ownership of a file. The order is `chgrp <groupname> <target>`.
42. Which option to `umask` will display the permissions to be used in a POSIX format?

    1. `-P`
    2. `-p`
    3. `-S`
    4. `-v`

    Answer:

    C.  The `-S` option displays output in a format such as `u=rwx,g=rx,o=rx`. The other options listed do not exist.
43. Which option to `chown` recursively changes the ownership?

    1. `-f`
    2. `-R`
    3. `-a`
    4. `-m`

    Answer:

    B.  The `-R` option will perform the change ownership in a recursive manner.
44. Which option to `chgrp` will change group ownership of all files within a given directory?

    1. `-directory`
    2. `-d`
    3. `-R`
    4. `-V`

    Answer:

    C.  The `-R` option sets the recursive option, which means `chgrp` will traverse the given directory and perform the group ownership change operation throughout the specified hierarchy.
45. When sourcing a file in bash, which `chmod` command would be necessary to provide the minimum privileges in order for the file to be sourced correctly, assuming that your current user owns the file?

    1. `chmod 600`
    2. `chmod 755`
    3. `chmod 777`
    4. `chmod 400`

    Answer:

    D.  You minimally need to be able to read the file being sourced; therefore, `chmod 400` will correctly set the permissions. Any `chmod` that gives additional permissions is not necessary. When permissions are granted using octal notation, the number 4 is read, 2 is write, and 1 is execute. There are three permissions: user (owner), group, and other or world. Therefore, `chmod 400` grants “read” privileges to the owner and no permissions to group and other/world.
46. Which of the following commands removes an expiration from an account?

    1. `sudo chage -l username`
    2. `sudo chage -E -1 username`
    3. `sudo chage -E now username`
    4. `sudo chage --noexpire username`

    Answer:

    B.  The `chage` command will be used for this purpose, specifically with the `-E` option. When provided with a date, `chage` will expire the account on that date. When provided with `-1`, the expiration will be removed, thus removing the user lockout. The use of `sudo` in the options for this question notes the need for elevated privileges in order to run the command successfully.
47. You need to determine whether LDAP integration is working correctly. In order to do so, you would like to obtain a list of users, as read by `/etc/nsswitch.conf`. Which command can be used for this purpose?

    1. `getuser`
    2. `getent`
    3. `usermod`
    4. `userlist`

    Answer:

    B.  The `getent` command is used to display entries based on the `/etc/nsswitch.conf` file. One use case for `getent` is when integrating with Microsoft Active Directory or another LDAP service, to check whether the connection can be made to the LDAP server. The `usermod` command is valid but is not used for this purpose, and the other commands shown for this question are not valid.
48. A command has the following listing obtained with `ls -la`:

    `-rwsr-xr-x 1 suehring suehring 21 Nov 2 13:53 script.sh`

    What does the `s` denote within the user permissions in the listing?

    1. The `suid` bit has been set for this program.
    2. This is a symlink.
    3. The file will not be executable.
    4. The file is a special system file.

    Answer:

    A.  The `suid` bit enables the program to run as the user who owns the file, regardless of who executes the program. Using SUID typically is not recommended for security reasons. The other permissions allow read (`r`) and write (`w`) for the owner of the file. The group and “other” permissions include read (`r`) and execute (`x`) but not write.
49. Which system logging facility is used for messages from the kernel?

    1. `syslog`
    2. `kernel`
    3. `kern`
    4. `system`

    Answer:

    C.  The `kern` facility receives messages from the kernel for logging purposes. Of the other options, `syslog` is used for logging messages about `syslog` itself. The other two options shown are not valid `syslog` facilities. Kernel messages are sometimes placed in a separate log called `/var/log/kern.log`.
50. What is the name of the `systemd` service that provides logging facilities?

    1. `systemd-journald`
    2. `systemd-loggingd`
    3. `systemd-syslog`
    4. `systemd-logger`

    Answer:

    A.  The service used for logging on a computer managed by `systemd` is called `systemd`-`journald`. You use `journalctl` to view logged entries rather than the standard Linux toolset.
51. Which configuration option in `/etc`/`logrotate.conf` will cause the log to be emailed to [`admin@example.com`](mailto:admin@example.com) when the log rotation process runs for the selected log?

    1. `mail` [`admin@example.com`](mailto:admin@example.com)
    2. `sendmail` [`admin@example.com`](mailto:admin@example.com)
    3. `maillog` [`admin@example.com`](mailto:admin@example.com)
    4. `logmail` [`admin@example.com`](mailto:admin@example.com)

    Answer:

    A.  The `mail` command will send the log to the specified email address on completion of the `logrotate` process. The other options shown do not exist as options in `/etc/logrotate.conf`.
52. You are deploying an Exim server and need to work with the firewall to ensure that the proper incoming ports are open. Which protocol and port should you allow inbound for normal SMTP traffic?

    1. TCP/23
    2. TCP/25
    3. TCP/110
    4. TCP/143

    Answer:

    B.  SMTP operates on TCP port 25, and if other servers are contacting your SMTP server, you'll need to listen on this port and allow traffic to it as well. Port 23 is used for Telnet, port 110 is POP3, and port 143 is IMAP, none of which are necessary for SMTP traffic.
53. Which port(s) and protocol(s) should be opened in a firewall in order for the primary and secondary name servers to communicate for a given domain?

    1. `udp/53`
    2. Both `tcp/53 and udp/53`
    3. `tcp/53`
    4. `udp/53` and `tcp/503`

    Answer:

    B.  Traditionally, `udp/53` is used for DNS queries, but with a primary and secondary server, it is assumed that zone transfers may occur. DNS zone transfers typically take place over `tcp/53`.
54. When examining open ports on the server, you see that TCP port 3000 is listed with no corresponding protocol name, such as `smtp`, `imaps`, and so on. In which file would you find a list of port-to-protocol translations that could be customized to add this new port?

    1. `/etc/ports`
    2. `/etc/p2p`
    3. `/etc/ppp`
    4. `/etc/services`

    Answer:

    D.  The `/etc/services` file contains standard port-to-protocol information based on the well-known and assigned ports from IANA. If you'd like to provide a custom name for the service, you can do so by editing this file. There is no `/etc/ports` or `/etc/p2p` file by default, and `/etc/ppp` is usually a directory for the point-to-point protocol daemon and related services.
55. On which port does ICMP operate?

    1. TCP/43
    2. UDP/111
    3. UDP/69
    4. ICMP does not use ports.

    Answer:

    D.  ICMP is a layer 3 protocol, meaning it does not use ports for communication. TCP/43 is used for whois, while port 111 is used for sunrpc. UDP/69 is used for the TFTP protocol.
56. Which of the following commands displays account information such as expiration date, last password change, and other related details?

    1. `usermod -l`
    2. `userinfo -a`
    3. `chageuser -l`
    4. `chage -l`

    Answer:

    D.  The `chage` command is used for working with account aging information such as expiration date, password change, days between password changes, and so on. The `-l` command lists information for the given account. The `usermod` command is used to make changes to an account, and the other two commands are not valid.
57. Which command is used to create a public/private key pair for use with SSH?

    1. `ssh -k`
    2. `ssh-keygen`
    3. `ssh-genkey`
    4. `ssh -key`

    Answer:

    B.  The `ssh-keygen` command is used to create a key pair for use with SSH instead of a password. Of the other options, the `ssh` command does exist, but the `-k` option is used to disable GSSAPI credential forwarding and not for the purpose described.
58. Within which file should you place public keys for servers from which you will accept key-based SSH authentication?

    1. `~/.ssh/authorized_keys`
    2. `~/.ssh/keys`
    3. `~/.ssh/keyauth`
    4. `~/.sshd/authkeys`

    Answer:

    A.  The file `authorized_keys`, stored in the `.ssh` directory in your home directory, contains public keys that are authorized to log in to the server using their corresponding private key.
59. You need to execute a command as a specific user. Which of the following commands enables this to occur?

    1. `sudo -u`
    2. `sudo -U`
    3. `sudo -s`
    4. `sudo -H`

    Answer:

    A.  The `-u` option is correct for this purpose. An uppercase `-U` option sets the user context for listing privileges. The `-s` option sets the shell, and the `-H` option sets the home directory.
60. Which option in `/etc/sudoers` will cause the specified command to not prompt for a password?

    1. `PASSWORD=NO`
    2. `NOPASSWD`
    3. `NOPASSWORD`
    4. `NOPROMPT`

    Answer:

    B.  The `NOPASSWD` option causes `sudo` to not prompt for a password for a given `sudo` command. This is useful for scripted scenarios where a password prompt would cause problems.
61. Which of the following commands will display kernel parameters related to resource limits such as CPU time, memory, and other limits for the currently logged-in user?

    1. `reslimit`
    2. `limitres -a`
    3. `ulimit -a`
    4. `proclimit -n`

    Answer:

    C.  The `ulimit` command shows such limits, and the `-a` option shows all limits for the currently logged-in user. The other commands are not valid.
62. When working with TCP wrappers, which line within the `/etc/hosts.deny` file will prevent any host within the 192.168.1.0/24 network from accessing services that operate from `xinetd`?

    1. `BLOCK: 192.168.1.0/24`
    2. `REJECT: 192.168.1.0`
    3. `ALL: 192.168.1.0/255.255.255.0`
    4. `NONE: 192.168.1/255.255.255.0`

    Answer:

    C.  The syntax to block access to every service uses the `ALL` keyword followed by the address or network to which the policy will apply. This is important because you may notice attacks coming from certain IP blocks, and blocking with TCP wrappers provides a fast method for effective blocking.
63. You are using an RSA-based key pair for SSH. By default, what is the name of the private key file in `~/.ssh`?

    1. `id_rsa`
    2. `id_rsa.priv`
    3. `id_rsa.key`
    4. `rsa_key.priv`

    Answer:

    A.  The file is named `id_rsa` by default, and the public key is named `id_rsa.pub`. For DSA keys, the names are `id_dsa` and `id_dsa.pub`.
64. Which option to the `su` command will execute a single command with a non-interactive session?

    1. `-s`
    2. `-u`
    3. `-c`
    4. `-e`

    Answer:

    C.  The `-c` option executes a single command but does so without an interactive session. The `-s` option specifies the shell to be used. There is no `-u` or `-e` option for the `su` command.
65. When working with digital signatures, after specifying the key server, which option to `gpg` is used to specify the key to send to the key server?

    1. `key-name`
    2. `keyname`
    3. `send-key`
    4. `sendkey`

    Answer:

    C.  The `send-key` option followed by the name of the key sends the key to the key server specified by the `keyserver` option. This is a typical scenario for sending a locally generated public key to a public server for others to use. The other options shown as potential answers do not exist.
66. Which of the following commands should be used to edit the `/etc/sudoers` file?

    1. Any text editor such as Vi or emacs
    2. `editsudo`
    3. `visudo`
    4. `visudoers`

    Answer:

    C.  While any text editor can be used, it is highly recommended to use the `visudo` command to edit `/etc`/`sudoers`. Using `visudo` enables syntax checking, which will help prevent issues with an invalid configuration causing problems for those who rely on `sudo`.
67. Which file can be used to store a server-wide cache of hosts whose keys are known for SSH?

    1. `/etc/sshd_known_hosts`
    2. `/etc/ssh_known_hosts`
    3. `~/.ssh/known_hosts`
    4. `/root/ssh_known_hosts`

    Answer:

    B.  The file `ssh_known_hosts`, usually kept in either `/etc`/ or `/etc/ssh/`, is used for the purpose described. Note that on some systems, this file and other SSH-related configurations may be found in `/etc/sshd/`. The answers that indicated `~` or within `/root` are incorrect because the question specified a server-wide list. A `known_hosts` file found within `~/.ssh` would indicate the user's home directory.
68. Which option within `/etc/sshd/sshd.conf` (or `/etc/ssh/sshd_config`) can be changed to prevent password-based authentication?

    1. `PasswordAuthentication`
    2. `Passwords`
    3. `AllowPass`
    4. `AllowPasswords`

    Answer:

    A.  The option `PasswordAuthentication` configures whether users will be allowed to authenticate using a password rather than key-based or another form of authentication. The other options shown are not valid. Note that on some distributions, the configuration files are found in `/etc/sshd/`, while on other distributions, the configuration files are found in `/etc/ssh/`.
69. Which of the following commands generates a GnuPG key pair?

    1. `gpg --gen-key`
    2. `gpg --key`
    3. `gpg --send-key`
    4. `gpg --create-key`

    Answer:

    A.  The `--gen-key` subcommand is used for the purpose described and will generate a self-signed private and public key pair in a PKI scenario. The other options shown do not exist.
70. Which file is used as the default storage for public keyrings for `gpg`?

    1. `publickeys.gpg`
    2. `pubring.gpg`
    3. `public.gpg`
    4. `pubkeys.gpg`

    Answer:

    B.  The file `pubring.gpg`, found in `~/.gnupg`, contains the public keyring.
71. Which option to the `su` command is used to obtain the normal login environment?

    1. `-u`
    2. `-U`
    3. `-`
    4. `-login`

    Answer:

    C.  The `-` option is the typical option passed to `su` for login. There is no `-u` or `-U` option, and the `-login` option does not exist. There is a `--login` option with two dashes, but that is not what's shown.
72. Which option enables SSL configuration for a given website or server?

    1. `SSLEngine`
    2. `SSLDirect`
    3. `SSLEnable`
    4. `SSLConnect`

    Answer:

    C.  The `SSLEngine` option needs to be set to `On` for SSL to be enabled for a given site or server. The other options are not valid. Enabling SSL is important in order to provide a level of security such that the actual data within an HTTP transaction cannot be viewed.
73. When using the `net` command in an Active Directory single sign-on (SSO) environment, which option enables authentication using Kerberos?

    1. `-b`
    2. `-k`
    3. `-l`
    4. `-a`

    Answer:

    B.  The `-k` option enables Kerberos authentication for the `net` command. The `-a` option indicates that non-interactive mode should be used, and `-l` sets the log directory. There is no `-b` option.
74. Within which directory are individual configuration files stored for the Pluggable Authentication Module (PAM) mechanism?

    1. `/etc/pamd`
    2. `/etc/pam`
    3. `/etc/pam.d`
    4. `/etc/pam.conf.d`

    Answer:

    C.  The directory `/etc/pam.d` stores configuration files for individual PAM-aware services. Each service typically has its own file, which is managed for that service according to its usage of PAM. Of the other options, none of the directories are the default directories used for PAM.
75. On which port does the `slapd` LDAP daemon listen for connections?

    1. 389
    2. 3389
    3. 3306
    4. 110

    Answer:

    A.  The standard port for LDAP is 389, and that is the port on which `slapd` listens for connections. Port 3389 is RDP, while 3306 is MySQL. Finally, 110 is POP3.
76. Which PAM module prevents logins from accounts other than root when the file `/etc/nologin` exists?

    1. `pam_login.so`
    2. `pam_preventlogin.so`
    3. `pam_nologin.so`
    4. `pam_logindef.so`

    Answer:

    C.  The `pam_nologin.so` module facilitates a scenario whereby non-root logins are prevented when `/etc/nologin` exists. This module must be specified within a configuration file for a given service. For example, within the `sshd` PAM configuration file, the following line creates this configuration for SSH: `account required pam_nologin.so`.
77. Which PAM module is responsible for normal or standard password authentication?

    1. `pam_auth.so`
    2. `pam_login.so`
    3. `pam_unix.so`
    4. `pam_standardlogin.so`

    Answer:

    C.  The `pam_unix.so` module is used for standard login. The manpage for `pam_unix.so` indicates that it is for “traditional password authentication.” The other modules listed are not standard PAM modules, although there is a similar `pam_auth` or `squid_pam_auth` module for Squid.
78. Which PAM module provides a mechanism for checking and enforcing the strength of passwords in order to enforce a password policy?

    1. `pam_passwdstr.so`
    2. `pam_cracklib.so`
    3. `pam_libpasswd.so`
    4. `pam_strpass.so`

    Answer:

    B.  The `pam_cracklib.so` module enforces password strength options. The other files listed are not valid PAM modules.
79. Which format should the certificate and key be in for a Postfix TLS configuration?

    1. PKCS
    2. PEM
    3. TLS
    4. SSL

    Answer:

    B.  PEM format is used for public and private keys with a Postfix TLS configuration. The other methods listed are valid cryptographic algorithms or systems but not for the scenario described. As with Sendmail, system administrators should take steps to secure mail servers so that the servers are not used for sending unsolicited email. For many scenarios, a full mail server like Postfix or Sendmail is not required in order to simply relay mail from a server.
80. Which `iptables` chain is used to create a port redirect?

    1. `REDIRECT`
    2. `PREROUTING`
    3. `PORTREDIR`
    4. `ROUTING`

    Answer:

    B.  The `PREROUTING` chain, part of the nat table, contains rules that are applied as packets arrive. A common use for this chain is to apply redirect rules. Among the other answers, `REDIRECT` may appear valid but is in fact a target and not a chain. The other options shown are not valid.
81. Which of the following commands saves the current set of `iptables` rules into a file?

    1. `save-iptables`
    2. `iptables-create`
    3. `iptables-save`
    4. `ipt-save`

    Answer:

    C.  The `iptables-save` command sends the current `iptables` rules to `STDOUT`. The output can be saved to a file and then applied the next time the server is restarted. The other commands shown are not valid.
82. Which of the following commands lists the current `iptables` rules while not attempting to resolve host or port names?

    1. `iptables -L`
    2. `iptables -List -no-resolve`
    3. `iptables -a`
    4. `iptables -nL`

    Answer:

    D.  The `iptables -n` option causes `iptables` to not resolve host names or port names. The `-L` option lists current rules. There is no `-a` option and the other options are not valid.
83. Which of the following directories contains configuration files for the `fail2ban` system?

    1. `/etc/fail2ban.cfg`
    2. `/etc/fail2ban.d`
    3. `/etc/f2b`
    4. `/etc/fail2ban`

    Answer:

    D.  The `/etc/fail2ban` directory contains configuration files related to `fail2ban`. The other directories shown are not valid. The use of `fail2ban` is helpful for SSH when compared with other methods like the recently deprecated pam\_tally2 and faillock, both of which would not prevent key-based authentication for SSH.
84. Within an OpenSSH configuration, which option disables the use of empty passwords?

    1. `DisableEmptyPass`
    2. `PermitEmptyPasswords`
    3. `EmptyPasswordAuth`
    4. `PermitPasswordLength`

    Answer:

    B.  The `PermitEmptyPasswords` directive specifies whether empty passwords can be used for authentication. Enabling empty passwords would be a specialized use case and generally is not recommended. The other options shown are not valid.
85. Which of the following commands sets the default policy for the `INPUT` chain to discard packets that don't have a specific rule allowing them?

    1. `iptables INPUT DROP`
    2. `iptables chain INPUT policy DROP`
    3. `iptables -P INPUT DROP`
    4. `iptables POLICY=DROP CHAIN=INPUT`

    Answer:

    C.  The `-P` option sets the policy for a given chain in `iptables`. In this case, the chain is `INPUT` and the policy necessary is `DROP`.
86. When configuring VPN service through a firewall, on which port and protocol does OpenVPN listen?

    1. ICMP/1194
    2. UDP/1194
    3. TCP/1194
    4. VPN/1194

    Answer:

    B.  OpenVPN listens on UDP port 1194 by default. The other combinations are not the valid OpenVPN configuration.
87. Which of the following best describes the difference between the `DROP` and `REJECT` targets in `iptables`?

    1. Both `DROP` and `REJECT` do the same thing.
    2. `DROP` silently discards packets, while `REJECT` sends back an ICMP acknowledgment.
    3. `REJECT` silently discards packets, while `DROP` sends back an ICMP acknowledgment.
    4. `DROP` sends back a direct message, and `REJECT` sends a redirect.

    Answer:

    B.  The `DROP` target silently discards packets that match the rule. An ICMP unreachable message is sent back for `REJECT`. In general, `DROP` is preferred in order to reduce the chances of denial of service (DoS) or other information-gathering issues.
88. Which of the following partial `iptables` rules sets up a configuration that limits log entries to three per minute?

    1. `-m limit 3 -j LOG`
    2. `-m limit --limit 3/minute --limit-burst 3 -j LOG`
    3. `-m limit --limit 3`
    4. `-m limit --limit-minute 3 --burst 3 -j LOG`

    Answer:

    B.  The `-m` match limit, along with the configuration options shown including the `LOG` target, creates the scenario described. There will be three log entries per minute. This can be useful to prevent denial of service caused by filling up log files or overwhelming the server I/O while another attack is under way.
89. Which of the following partial `iptables` rules allows incoming ICMP traffic?

    1. `-A INPUT -p ICMP -j ACCEPT`
    2. `-A IN -P ICMP`
    3. `-A INPUT -P ACCEPT-ICMP`
    4. `-A IN -P ICMP -j ACCEPT`

    Answer:

    A.  The `INPUT` chain will be used. When used with the `-A` option, it will append a rule to the chain. The `-p` option specifies the protocol, ICMP in this case; the `-j` option specifies the target, `ACCEPT` in this case. The `-P` option specifies a policy and will not be used for this scenario.
90. Which of the following partial `iptables` rules blocks all traffic from source IP 192.168.51.50?

    1. `-A INPUT -p ALL 192.168.51.50 -j ACCEPT`
    2. `-A INPUT -p ALL -s 192.168.51.50 -j DROP`
    3. `-A INPUT -p ALL -s 192.168.51.50 -j BLOCK`
    4. `-A INPUT -p ALL -f 192.168.51.50 -j DISCARD`

    Answer:

    B.  The `INPUT` chain will be used, and a rule needs to be appended with `-A`. The `ALL` option, when specifying a protocol, means all protocols will be included in the rule. The `-s` option specifies the source, which in this case is a single IP address. Finally, the `DROP` target silently discards packets. There is no `BLOCK` or `DISCARD` target, and the `ACCEPT` target will not block but will accept all traffic.
91. Which of the following partial `iptables` rules will allow all hosts to connect to TCP port 2222?

    1. `-A INPUT -p TCP -s 0/0 --destination-port 2222 -j ACCEPT`
    2. `-A TCP -s ALL -p 2222 -j ACCEPT`
    3. `-A INPUT -p TCP -s *.* --destination-port 2222 -j ALLOW`
    4. `-A INPUT --destination-port */* -j ACCEPT`

    Answer:

    B.  A rule will be appended to the `INPUT` chain with `-A`. In this case, the protocol should be specified with `-p TCP` and a destination port of 2222. The source address indicated, `0/0`, applies the rule to all hosts. The `ACCEPT` target will be used.
92. Which of the following commands enables forwarding such as would be used for NAT?

    1. `echo “1” > /proc/sys/net/ipv4/nat`
    2. `echo “1” > /proc/sys/net/ipv4/ip_forward`
    3. `iptables --enable-forwarding`
    4. `ip-forward --enable`

    Answer:

    B.  Echoing a `1` to the `/proc/sys/net/ipv4/ip_forward` file enables forwarding of IP packets. This is necessary in order to utilize NAT and for other uses. There is a similar file for IPv6 at `/proc/sys/net/ipv6/ip_forward`. There is no `/proc/sys/net/ipv4/nat` file.
93. Within a jail configuration for `fail2ban`, which configuration option sets the name and location of the log file to monitor for failures?

    1. `logpath`
    2. `monitor`
    3. `logfile_mon`
    4. `monitor_log`

    Answer:

    A.  The `logpath` directive determines the log file that will be monitored for failures by `fail2ban`. This file is used as part of a larger configuration for a given jail. The other directives are not valid for `fail2ban`.
94. Which command sends a copy of the public key identity to another server for use with SSH?

    1. `ssh-key`
    2. `ssh-copy-key`
    3. `ssh-sendkey`
    4. `ssh-copy-id`

    Answer:

    D.  The `ssh-copy-id` command sends an identity to a remote server that can then be used for key-based authentication. The other commands shown are not valid.
95. Which option in `/etc`/`sudoers` sets the destination address for administrative and security emails related to `sudo`?

    1. `mail`
    2. `mailto`
    3. `secmail`
    4. `adminmail`

    Answer:

    B.  The `mailto` configuration option sets the destination for emails related to `sudo`. The other options listed are not valid for `sudo`.
96. Which port should be allowed through a firewall for NTP communication?

    1. Port 139
    2. Port 161
    3. Port 123
    4. Port 194

    Answer:

    C.  Port 123 is used for NTP communication by default. Port 161 is SNMP, while 139 is NetBIOS, and 194 is IRC.
97. You are looking for files related to the SSL configuration on the server. After looking in `/etc/ssl`, within which other directory might the files reside?

    1. `/etc/sslconfig`
    2. `/usr/share/ssl`
    3. `/etc/pki`
    4. `/etc/private`

    Answer:

    C.  Files related to SSL are typically stored in either `/etc/ssl` (or a subdirectory therein) or in the `/etc/pki` hierarchy. There is no `/etc/private` or `/usr/share/ssl` directory. The other directories shown as options do not exist.
98. Which OpenSSH configuration directive is used to specify the users who will be allowed to log in using SSH?

    1. `AllowUsers`
    2. `PermitUsers`
    3. `UsersAllowed`
    4. `AllowedUsers`

    Answer:

    A.  The `AllowUsers` directive is used to specify users who will be allowed to log in to the server. The other options shown are not valid.
99. Which option within a `LOG` target for `iptables` sets a string that will be prepended to log entries?

    1. `--log-prefix`
    2. `--prepend`
    3. `--log-prepend`
    4. `--log-str`

    Answer:

    A.  The `--log-prefix` option specifies the string that will be prepended when a log entry is created by `iptables`. The other options shown are not valid for use with `iptables`.
100.    Within the SELinux configuration, which option controls whether the policy will be targeted or strict?

        1. `SEPOLICY`
        2. `SELINUXTYPE`
        3. `SETARGET`
        4. `SELINUXPOLICY`

        Answer:

        B.  The `SELINUXTYPE` option can be set to targeted or strict. With targeted, only specific network daemons are protected.
101.    Which of the following best describes the status of SELinux when the command `getenforce` returns `Permissive`?

        1. A `Permissive` return means SELinux is enabled but rules are not enforced, although DAC rules are still in effect.
        2. A `Permissive` return means SELinux is not enabled.
        3. A `Permissive` return means SELinux is enabled, although rules are not enforced and DAC rules are not in effect.
        4. A `Permissive` return means SELinux is using an enforcing policy.

        Answer:

        A.  When `Permissive` is returned, SELinux is not enforcing rules but is using DAC rules. Other return outputs are `Enforcing` and `Disabled`.
102.    Which of the following describes the primary difference between the configuration files `ssh.conf` and `sshd.conf` (typically found in `/etc/sshd/` or `/etc/ssh/`)?

        1. `sshd.conf` is the configuration file for the system SSH, and `ssh.conf` is the options configuration file.
        2. `sshd.conf` is the configuration file for the system SSH daemon, and `ssh.conf` provides system-wide client SSH configuration.
        3. `sshd.conf` is used when SSH will be disabled, and `ssh.conf` is used when SSH is enabled.
        4. `sshd.conf` is the first configuration file read for a client connection, while `ssh.conf` is the first configuration read for a server configuration.

        Answer:

        B.  The `sshd.conf` file is used for server configuration. On some distributions, this file is called `sshd_config`. The `ssh.conf` file is used for client configuration at the system level.
103.    When you're working with PAM, a module that is marked as `required` has failed. Which of the following describes what happens to the other modules in that realm?

        1. Processing stops immediately when a failure of a required module occurs.
        2. Processing stops after all required modules are processed.
        3. Processing continues until another required module is encountered.
        4. Processing continues through other modules but ultimately fails.

        Answer:

        D.  When a required module returns a failure, other modules continue to process, but the authentication ultimately fails. This is done so that logging will occur and other modules have had a chance to handle the authentication attempt. If a failure should be immediate without processing other modules, then the `requisite` option should be used instead of `required`.
104.    What is the UID of the root account?

        1. 1000
        2. 0
        3. 100
        4. 65535

        Answer:

        B.  The root account has UID 0 on a Linux system. Typically, service accounts have UIDs below 1000, many times below 100. Normal user accounts usually begin at UID 1000.
105.    Using a system such as Google Authenticator to provide multifactor authentication is an example of which type of token?

        1. Hardware
        2. Software
        3. Virtual-based
        4. Usage-based

        Answer:

        B.  Although a hardware token may be available, the default option is software based. Note also that OTP solutions to generate a one-time passcode are similar in functionality to provide multifactor authentication.
106.    Within which directory are the predefined zones for `firewalld`?

        1. `/etc/firewalld/`
        2. `/usr/lib/firewalld/zones/`
        3. `/usr/firewalld/zones/`
        4. `/etc/firewall/zones`

        Answer:

        B.  The directory `/usr/lib/firewalld/zones/` contains predefined zones for use with `firewalld`. The files are copied to `/etc`/`firewalld/zones/` when modified.
107.    You need to set a bootloader password for GRUB. To do so, which of the following configuration options should be set in `/boot/grub/grub.conf`?

        1. `login`
        2. `prompt`
        3. `boot-passwd`
        4. `password`

        Answer:

        D.  The `password` configuration option is set in `/boot/grub/grub.conf`. The other options shown for this question are not valid for the scenario.
108.    Assuming that the output from the `sestatus` command indicates that SELinux is in `Permissive` mode, which of the following commands is used to change the mode to `Enforcing`?

        1. `setenforce en`
        2. `setenforce 1`
        3. `setenforce on`
        4. `setenforce --enable`

        Answer:

        B.  The `setenforce` command is used for this purpose and can be given an argument of the number `1` or the word `Enforcing` to enable `Enforcing` mode. This can be verified with the `sestatus` command.
109.    Your organization uses `ssh-agent` for authentication assistance with SSH. Which command can be used to add a private key to `ssh-agent`?

        1. `ssh-privkey`
        2. `ssh-agent-key`
        3. `ssh-add`
        4. `ssh-addkey`

        Answer:

        C.  The `ssh-add` command is used for this purpose. The other commands shown do not exist.
110.    When working with access control lists (ACLs), which of the following commands is used to display information about the access control list for a given file?

        1. `getfacl`
        2. `getacl`
        3. `acldisp`
        4. `showacl`

        Answer:

        A.  The `getfacl` command is used to display access control list information for a file. The `setfacl` command is used to set this information. The other commands shown are not valid Linux commands.
111.    You need to provide a special username and other parameters related to a specific host to which you connect using SSH. To which file should you add this information?

        1. `~/.ssh/hosts`
        2. `~/.ssh/known_hosts`
        3. `~/.ssh/config`
        4. `~/.ssh/hostconfig`

        Answer:

        C.  The file `~/.ssh/config` is the appropriate location for this type of configuration information. Of the other answers, only `~/.ssh/known_hosts` exists and contains public key information for hosts to which you have connected.
112.    You are using `chmod` in order to change several web-related files so that the web server/public can read them. Which option should you add to the `chmod` command in order for the permissions to inherit to other files?

        1. `-R`
        2. `-v`
        3. `-i`
        4. `-M`

        Answer:

        A.  The `-R` option is used to indicate recursive behavior. Of the other options, only `-v` is valid and provides verbose output.
113.    Which option to `setsebool` writes the current values to disk so that they will be applied at next reboot?

        1. `-A`
        2. `-P`
        3. `-D`
        4. `-M`

        Answer:

        B.  The `-P` option makes the values persistent across reboots for SELinux system booleans. The other options are not valid with `setsebool`.
114.    When working with AppArmor, within which directory are profiles and application permissions located?

        1. `/etc/apparmor/`
        2. `/etc/apparmor.d/`
        3. `/etc/appa.d/`
        4. `/etc/armor.d/`

        Answer:

        B.  The directory `/etc/apparmor.d/` is the location in which profiles and application permissions are located.
115.    When using Kerberos authentication, which of the following commands shows the ticket cache?

        1. `ktix`
        2. `ktel`
        3. `kcache`
        4. `klist`

        Answer:

        D.  The `klist` command shows the current tickets when using Kerberos authentication. Of the other answers, the `kinit` command is used to retrieve the initial ticket-granting ticket. The remaining answers are not valid commands.
116.    Which of the following options to the `ls` command displays ownership and permission information?

        1. `-m`
        2. `-l`
        3. `-b`
        4. `-f`

        Answer:

        B.  The `-l` option provides a long or detailed listing of files and directories, including ownership and permissions. The `-m`, `-b`, and `-f` options are not related to the scenario described.
117.    Which option to `getsebool` returns the entire list of SELinux booleans?

        1. `-a`
        2. `-b`
        3. `-c`
        4. `-d`

        Answer:

        A.  The `-a` option returns all booleans. The other options are not valid with `getsebool`.
118.    Which AppArmor command uses `netstat` to determine the network-related processes that do not have AppArmor profiles?

        1. `aa-profiles`
        2. `aa-netstat`
        3. `aa-unconfined`
        4. `aa-netlist`

        Answer:

        C.  The `aa-unconfined` command displays processes that are offering network ports but do not have an AppArmor profile. The other commands are not valid.
119.    Which group can be used to restrict access to execute the `su` command?

        1. `super`
        2. `admins`
        3. `wheel`
        4. `runsu`

        Answer:

        C.  The `wheel` group can be used to restrict access to the `su` command to those accounts that are members of the group. The other groups do not exist by default.
120.    You need to change the SELinux security context of a file. Which of the following commands should be used for this purpose?

        1. `setcontext`
        2. `sesecon`
        3. `chcon`
        4. `setcon`

        Answer:

        C.  The `chcon` command is used to change the security context.
121.    Which of the following is an advantage of using an SSL-based VPN client?

        1. The transport may be able to get around firewalls that otherwise block VPN traffic.
        2. The use of SSL makes default configuration easier.
        3. The use of SSL means keys do not need to be configured.
        4. The use of SSL makes no difference.

        Answer:

        A.  An SSL VPN can sometimes work around firewalls that otherwise block VPN traffic. SSL-based VPNs are not typically the default in Linux.
122.    When configuring PKI on a Red Hat system, which options are available as hashing algorithms when RSA is used as a key type?

        1. SHA256withRSA
        2. MD4
        3. SHA2048
        4. SHAwithEC

        Answer:

        A.  When RSA is chosen as the key type, SHA256withRSA is available along with SHA512withRSA. The other answers shown are not valid hashing algorithms with RSA.
123.    Which of the following passwords can be used to secure a system such that it will not boot, even if the attacker has physical access to place a USB boot disk in the computer?

        1. GRUB password
        2. UEFI/BIOS password
        3. Root password
        4. SHA1 password

        Answer:

        B.  A password set in the BIOS can be used to prevent the system from booting or handing off the boot process to a bootloader. Neither GRUB nor a root password will help with this scenario because physical access is available.
124.    Which option to the `restorecon` utility can be used to view the current contexts without making changes?

        1. `-n`
        2. `-r`
        3. `-g`
        4. `-p`

        Answer:

        A.  The `-n` option to `restorecon` shows current contexts without changing them. Of the other options that are valid, `-r` changes recursively, and `-p` shows progress.
125.    You need to view the SELinux contexts for various processes on the system. Which of the following commands will accomplish this task?

        1. `showcon`
        2. `proccon`
        3. `lcon -Z`
        4. `ps -Z`

        Answer:

        D.  The `ps` command shows processes. When the command is given the `-Z` option, SELinux contexts are shown.
126.    Which PAM module can be used to lock accounts after failed login attempts?

        1. `pam_lock`
        2. `pam_tally2`
        3. `pam_loginlock`
        4. `pam_watchlog`

        Answer:

        B.  The `pam_tally2` module keeps track of failed logins and can be used to lock out an account after a certain number of failed attempts. Note that `pam_faillock` provides similar functionality now that `pam_tally2` has been deprecated.
127.    Which of the following commands places all AppArmor profiles into complain mode?

        1. `aa-complain /etc/apparmor.d/*`
        2. `aa-enable -complain /etc/apparmor.d/*`
        3. `aa-enable -complain /etc/apparmor/*`
        4. `aa-complain /etc/apparmor/*`

        Answer:

        A.  The command `aa-complain` is used to place profiles into complain mode. Profiles are located in `/etc/apparmor.d/`, and thus the command shown places all profiles into complain mode.
128.    Which option within the `sshd_config` file sets per-user configuration?

        1. `UserConf`
        2. `Match User`
        3. `Per-User`
        4. `Conf User`

        Answer:

        B.  The `Match User` option is used to change the configuration for a specific user. The other options shown are not valid.
129.    Which option to the `firewall-cmd` command sets the current runtime configuration to be available on next reboot of the computer?

        1. `--set-perm`
        2. `--make-perm`
        3. `--runtime-to-permanent`
        4. `--current-to-persistent`

        Answer:

        C.  The `--runtime-to-permanent` option sets the current runtime configuration to become permanent and available on next boot.
130.    When working with `ufw`, you need to allow SSH traffic. Which of the following commands facilitates this scenario?

        1. `ufw allow tcp/22`
        2. `ufw enable ssh`
        3. `ufw allow ssh`
        4. `ufw enable tcp/21-22`

        Answer:

        A.  The `ufw allow` command is used to add rules, and SSH operates on TCP port 22.
131.    Which of the following is the name for the firewall control software associated with Netfilter?

        1. `iptables`
        2. `ipt`
        3. `netfw`
        4. `netfilterfw`

        Answer:

        A.  The software used to create firewalls found on most systems is `iptables`. Notably, later versions are called `nftables`, but `iptables` is still found on many systems in use today.
132.    When you're copying files using `scp`, which port needs to be open in the firewall?

        1. TCP/21
        2. TCP/22
        3. TCP/20 and TCP/21
        4. UDP/53

        Answer:

        B.  The `scp` utility uses SSH as transport and therefore requires TCP port 22. TCP ports 20 and 21 are used for legacy FTP, while UDP/53 is used for DNS queries.
133.    You are viewing the contents of a directory with the `ls` command but do not see files that begin with a single dot (`.`). Which option to `ls` shows those files?

        1. `-a`
        2. `-b`
        3. `-c`
        4. `-d`

        Answer:

        A.  The `-a` option shows files and directories that begin with a dot. The other options shown are not related to this scenario.
134.    Which option to `ssh` specifies the private key to use for authentication?

        1. `-m`
        2. `-i`
        3. `-k`
        4. `-a`

        Answer:

        B.  The `-i` option is used to specify a private key to use for authentication with SSH. Of the other options, `-a` is used to disable forwarding of the authentication agent, `-k` disables GSSAPI credentials, and `-m` specifies message authentication code (MAC) algorithms.
135.    You have found that the owner of the Apache process is `www-data`. Assuming that the file does not have read privileges, what command will change the ownership of a file, given as `<filename>`, such that `www-data` can write to the file?

        1. `chown www-data <filename>`
        2. `chown apache-www-data <filename>`
        3. `chmod www-data +w <filename>`
        4. `chmod www-data.apache <filename>`

        Answer:

        A.  The `chown` command changes ownership of a file or directory, and the `www-data` user was specified in the question, thus making option A the only correct option for this scenario.
136.    When using `sudo` in a scripted environment, which option can be used to specify a noninteractive mode?

        1. `-f`
        2. `-m`
        3. `-n`
        4. `-l`

        Answer:

        C.  Noninteractive mode for `sudo` is triggered with the `-n` option. The other options are not valid for this scenario.
137.    Which command is used to turn off AppArmor profiles?

        1. `aa-disable`
        2. `aa-turnoff`
        3. `aa-enable -d`
        4. `aa-off`

        Answer:

        A.  The `aa-disable` command is used to turn off profiles used with AppArmor. The other commands shown are not valid.
138.    Which command and option are used to view the SELinux security context of a given file?

        1. `ls -context`
        2. `file -Z`
        3. `ls -Z`
        4. `sel -context`

        Answer:

        C.  The `-Z` option to `ls` is used to view the SELinux security context. The `file` command is a valid command but does not have a `-Z` option.
139.    Digital signatures can be provided in Linux through which of the following commands?

        1. `gds`
        2. `gpg`
        3. `dmc`
        4. `gds2`

        Answer:

        B.  GnuPG can be used to provide digital signatures through its `gpg` command. The other answers shown are not valid.
140.    You need to make a change to the global behavior of AppArmor. To avoid editing the profiles directly, which directory contains common settings that can be changed instead?

        1. `/etc/apparmor.d/configs`
        2. `/etc/apparmor/globals`
        3. `/etc/apparmor/edits`
        4. `/etc/apparmor.d/tunables`

        Answer:

        D.  The directory `/etc/apparmor.d/tunables` contains parameters and configurations that are commonly changed.
141.    Which of the following directories contains configuration for UFW?

        1. `/etc/ufwd`
        2. `/etc/ufw.d`
        3. `/etc/ufw`
        4. `/etc/ufirewall`

        Answer:

        C.  The directory `/etc`/`ufw` typically contains configuration information for UFW. On many systems, `/etc/default/ufw` will also contain commonly changed default configuration items.
142.    Which software can be used in connection with `iptables` in order to more effectively block traffic from entire network ranges?

        1. `ipblock`
        2. `ipset`
        3. `iplist`
        4. `ipcoll`

        Answer:

        B.  The `ipset` project and software facilitates more effective rule management by helping to create sets of IP addresses to which common rules can be applied.
143.    You have created a public key and private key for use with SSH. The contents of which key should be copied to a remote host in order to enable authentication?

        1. The public key.
        2. The private key.
        3. Both the public and private keys.
        4. Neither the public nor the private key. It must be generated on the remote host.

        Answer:

        A.  The public key should be copied to the remote host. When it is copied and the contents placed into `~/.ssh/authorized_keys`, authentication will be allowed from anyone presenting the corresponding private key.
144.    What is the octal notation to specify that a directory should have read+write+execute permissions for the owner and read+execute permissions for the group and other?

        1. 711
        2. 644
        3. 755
        4. 777

        Answer:

        C.  When octal notation is used, the number 4 is read, 2 is write, and 1 is execute. User, group, and other permissions appear in that order with octal notation. Therefore, 7 grants the user read+write+execute, and 5 grants read+execute for group and other.
145.    Which option to `sestatus` shows the context of a file?

        1. `-f`
        2. `-v`
        3. `-m`
        4. `-a`

        Answer:

        B.  The `-v` option shows contexts of files listed in `/etc`/`sestatus.conf`. The other options are not valid for use with `sestatus`.
146.    Which option to `chage` sets the maximum days that a password is valid?

        1. `-v`
        2. `-m`
        3. `-M`
        4. `-d`

        Answer:

        C.  The `-M` option sets the maximum days for password validity, while `-m` sets the minimum days between password changes. The other options are not relevant to this scenario.
147.    Which option within an SSH server configuration enables authentication using Kerberos?

        1. `UseKerberos`
        2. `KerberosAuthentication`
        3. `EnableKerberos`
        4. `KerberosEnable`

        Answer:

        B.  `KerberosAuthentication` is the option within the SSH server configuration that controls whether users can authenticate using Kerberos.
148.    You are working with `iptables-save` to examine the contents of tables in a scripted environment. Which option to `iptables-save` can be used to specify the table name rather than outputting information for all tables?

        1. `-t`
        2. `-a`
        3. `-s`
        4. `-i`

        Answer:

        A.  The `-t` option, along with the table name, limits output to just the specified table rather than all. The other options are not valid for use with `iptables-save`.
149.    Ports below what number are considered to be the well-known ports?

        1. 256
        2. 512
        3. 1024
        4. 65535

        Answer:

        C.  Sometimes called privileged ports, well-known ports are considered to be those ports under 1024. These ports are usually made available by system daemons and system-level services and can be disabled if not in use.
150.    Which PAM module is responsible for enforcing limits such as the maximum number of logins and CPU time used?

        1. `pam_enforce.so`
        2. `pam_limittest.so`
        3. `pam_max.so`
        4. `pam_limits.so`

        Answer:

        D.  The `pam_limits.so` module is responsible for enforcement of limits such as those mentioned in the question as well as several others like the maximum size of files, memory usage, and so on. The other modules listed are not valid.
151.    When using LDAP for authentication, what will be logged with the `loglevel` set to 0×10 in a `slapd.conf` configuration file?

        1. No debugging
        2. Trace debugging
        3. Stats logging
        4. Packets sent and received

        Answer:

        D.  There are multiple ways to specify log levels and debugging for `slapd`, including by keyword, by integer, or, as shown in the question, by hex. All the values shown are valid for `loglevel`. No debugging is 0, trace is 1, stats logging is 256 or 512 depending on type, and packets sent and received is integer 16 or hex 0x10.
152.    On which port does LDAP over SSL listen for connections?

        1. 389
        2. 443
        3. 636
        4. 3128

        Answer:

        C.  LDAP over SSL uses port 636 by default. Of the other options, port 389 is LDAP but without SSL, port 443 is used for HTTPS communication, and 3128 is used for Squid proxy.
153.    Which of the following PAM modules can be used for authorization and authentication scenarios using external files?

        1. `pam_fileauth.so`
        2. `pam_listfiles.so`
        3. `pam_filesauth.so`
        4. `pam_fileauth.so`

        Answer:

        B.  The `pam_listfiles.so` module is used to create scenarios whereby you can create files that control authentication and authorization through the PAM system. The other files are not valid for the scenario described.
154.    Which option to `ssh-keygen` sets the type of key that will be created?

        1. `-k`
        2. `-t`
        3. `-e`
        4. `-i`

        Answer:

        B.  The `-t` option sets the key type for `ssh-keygen`. The other options do not set the key type but may be valid for other purposes.
155.    You are attempting to remove a software package from a Debian system. Which command removes the package?

        1. `apt-cache remove-update`
        2. `apt-cache remove`
        3. `apt-get remove`
        4. `apt-get delete`

        Answer:

        C.  The `apt-get remove` command is used to remove packages from a Debian system. There is no `remove-update` option or `remove` option to `apt-cache`. Likewise, there is no `delete` option for `apt-get`.
156.    Which of the following configuration options sets a hard limit of 25 processes for a user called suehring in `/etc/security/limits.conf`?

        1. `suehring hard proc 25`
        2. `suehring hard nproc 25`
        3. `suehring proc 25 hard-limit`
        4. `proc 25 suehring hard`

        Answer:

        B.  The format is username (or other specifier) followed by `hard` or `soft`, depending on the limit type, and then the keyword followed by the value for that given keyword.
157.    Which command is used to configure kernel parameters for a new GPU driver added to the system?

        1. `gpuctl`
        2. `gpuload`
        3. `sysconfig`
        4. `sysctl`

        Answer:

        D.  The `sysctl` command can be used for changing parameters within the running kernel. The changes are not saved between reboots, though, and need to be reapplied if the system is restarted. The other commands shown are not valid.
158.    Which type of module interface for PAM is used to set a policy such as the time of day that a user can log in?

        1. `auth`
        2. `account`
        3. `password`
        4. `policy`

        Answer:

        B.  The `account` module interface is where access verification occurs. Among the other options, the `auth` and `password` interfaces are used for different purposes, and there is no `policy` interface.
159.    Which command can be used to set file attributes such as making a file immutable?

        1. `chr`
        2. `fattr`
        3. `chattr`
        4. `fop`

        Answer:

        C.  The `chattr` command is used to change file attributes, including making them immutable. The other commands are not valid.
160.    Which range of UIDs is typically used by service accounts?

        1. 1 to 999
        2. 1 to 100
        3. 32,768 to 65,535
        4. 1,000 to 1,999

        Answer:

        A.  UIDs less than 1,000, not including 0, are typically used by service accounts. This is not required but is done by convention.
161.    Which message type(s) should be queried when looking for SELinux access denials or violations?

        1. `AVC`
        2. `DEN`
        3. `AVC,USER_AVC`
        4. `STOP,VIOL`

        Answer:

        A.  Looking for access vector cache (AVC) messages within the `ausearch` command can reveal information about policy violations. It's typical to also include `USER_AVC` within the query. The other options shown are not valid.
162.    Which option is used to display information about current file attributes?

        1. `lsfile`
        2. `lsattr`
        3. `showfile`
        4. `exattr`

        Answer:

        B.  The `lsattr` command can be used to show extended attribute information about a file, such as whether the file is immutable. The other options shown are not valid.
163.    Which of the following describes a key difference between a self-signed certificate and a certificate issued by a trusted certificate authority?

        1. A self-signed certificate is valid for only 30 days.
        2. A self-signed certificate will be automatically trusted by clients when attempting to connect.
        3. A self-signed certificate will need to be manually trusted by clients when attempting to connect to a service that uses the certificate.
        4. There is no practical difference between a self-signed certificate and one issued by a trusted certificate authority.

        Answer:

        C.  Self-signed certificates are not automatically trusted by clients when connecting, whereas a list of trusted certificate authorities enables certificates issued by those authorities to be automatically trusted. Both self-signed certificates and those issued by third parties can be valid for any length of time, making option A incorrect.
164.    Which of the following software packages can be used to scan a host for rootkits?

        1. rkfind
        2. wxps
        3. tmroot
        4. Chkrootkit

        Answer:

        D.  The Chkrootkit software package can be used for security scanning such as examining a host for signs of tampering often associated with a rootkit. The other commands shown as options do not exist.
165.    Within which file is the default umask set?

        1. `/etc/profile`
        2. `/etc/umask`
        3. `/defaults/umask`
        4. `/etc/user.defs`

        Answer:

        A.  The file `/etc/profile` is where the umask is typically set for most Linux distributions. The other files shown do not exist.
166.    After recovering from kernel panic, you would like to look at what might have happened. Which of the following files contains the kernel ring buffer messages?

        1. `/var/log/dmesglog`
        2. `/var/log/start.log`
        3. `/var/log/kern.log`
        4. `/var/log/bootlog.txt`

        Answer:

        C.  The file `/var/log/kern.log` contains kernel messages and can be used to troubleshoot a kernel panic.
167.    Which of the following commands is used to examine the `systemd` journal or log file?

        1. `journallist`
        2. `ctlj`
        3. `journalctl`
        4. `jctl`

        Answer:

        C.  The `journalctl` command is used to work with the `systemd` journal. On `systemd`-based systems, `journalctl` is a central command for debugging and troubleshooting.
168.    Assuming that the `$ModLoad imudp` configuration option has been set in the `/etc/rsyslog.conf` configuration file for `rsyslogd`, which of the following additional options is necessary to configure the port on which the server will listen?

        1. `$Port 514`
        2. `$UDPServerRun 514`
        3. `$Listen 514`
        4. `$UDPListen 514`

        Answer:

        B.  The `$UDPServerRun` option is used for the purpose described. The port on which the server should listen is then provided as the value for this option. The other options shown are not valid configuration items for `rsyslogd`.
169.    Which option in `journald.conf` controls the maximum file size for individual journal logs?

        1. `SystemMaxFileSize`
        2. `MaxFile`
        3. `LogFileSize`
        4. `LogSize`

        Answer:

        A.  The `SystemMaxFileSize` option controls the size of the journal log file to ensure that a log does not cause problems related to disk usage. The `SystemMaxUse` option controls overall size of journal files, and the default for `SystemMaxFileSize` is one-eighth of the `SystemMaxUse` setting to allow for rotation of files.
170.    Which option within a `logrotate` configuration file disables compression of the log file?

        1. `compressoff`
        2. `limitcompress`
        3. `nocompression`
        4. `nocompress`

        Answer:

        D.  The `nocompress` option is used to prevent the log file from being compressed or zipped as part of the rotation process. This might be needed on systems where compression negatively affects performance or where additional processing is necessary.
171.    Which of the following files should be used to display a message to users prior to logging in locally?

        1. `/etc/loginmesg`
        2. `/etc/logmessage.txt`
        3. `/etc/issue`
        4. `/etc/banner`

        Answer:

        C.  The `/etc/issue` file is used to provide a message to users, such as a login banner, prior to local login. The other files shown are not valid for the purpose described.
172.    Which file contains a message that is displayed after successful login?

        1. `/etc/loginbanner`
        2. `/etc/issue`
        3. `/etc/motd`
        4. `/etc/message`

        Answer:

        C.  The contents of the file `motd`, an abbreviation for Message of the Day, are displayed when a user logs in successfully. Among the other options, the contents of `/etc/issue` are displayed prior to local login. The other filenames are not valid for this purpose.
173.    When working with System Security Services Daemon (sssd), which command is used to discover and join an Active Directory domain for a single sign-on (SSO) authentication scenario?

        1. `joinad`
        2. `adjoin`
        3. `realm`
        4. `realm-ad`

        Answer:

        C.  The `realm` command is used to join a computer to an Active Directory domain. The other commands shown do not exist.
174.    You need to provide SSL certificates for several hosts within your organization, some of which are public-facing. Which type of certificate should be used for this purpose?

        1. Wildcard certificate
        2. Self-signed certificate
        3. Certificate-in-escrow
        4. Unchained certificate

        Answer:

        A.  A wildcard certificate is appropriate for this use case. The wildcard certificate is then valid for all hosts in the same domain. While a self-signed certificate could be used, the scenario specified public-facing hosts, which means that a trusted certificate authority will need to be used in order for public end users to automatically trust the certificate. The other two options are not valid.
175.    Within which file are values related to password aging defined on a system that uses `/etc/shadow`?

        1. `/etc/shadow.defaults`
        2. `/etc/shad.defs`
        3. `/etc/login.defs`
        4. `/etc/shadow.conf`

        Answer:

        C.  The file `/etc/login.defs` is where options related to shadow-based authentication are set. The other options shown are not valid.
176.    When working with nftables to maintain a stateful firewall, which connection state represents a packet or session that has not yet been established?

        1. `new`
        2. `unseen`
        3. `clear`
        4. `conn_new`

        Answer:

        A.  The new connection state indicates a communication path or session that has not yet been established between source and destination. The new connection state was also available in `iptables`. None of the other options shown are valid connection states in nftables.
177.    Which file sets the global or default values for the `ssh` command client behavior?

        1. `/etc/ssh/config`
        2. `/etc/ssh/client_config`
        3. `/etc/ssh/ssh_config`
        4. `/etc/ssh/sshd_config`

        Answer:

        C.  The file `/etc/ssh/ssh_config` contains default values for client behavior that can be overridden by `~/.ssh/config` values on a per-user basis. Of the other files, `/etc/ssh/sshd_config` is valid but defines server-related configuration.
178.    When using dynamic port forwarding with SSH, which type of proxy is used?

        1. Squid
        2. Internal
        3. Curb
        4. Socks

        Answer:

        D.  A Socks proxy is used when dynamic port forwarding is configured with SSH. Of the other answers, Squid can be used as a proxy server but is not associated with dynamic port forwarding for SSH. The other options shown are not valid.
179.    Which polkit function is used to create a rule?

        1. `addRule()`
        2. `createRule()`
        3. `NewRule()`
        4. `ruleAdd()`

        Answer:

        A.  Rules are added with a call to the `addRule()` function in polkit, which is the executable associated with PolicyKit and is used to create rules. The other options shown for this question are not valid functions.
180.    You need to relabel after changing SELinux policies. Which of the following commands triggers the autorelabel process?

        1. `autorel`
        2. `touch /.autorelabel`
        3. `selinux -rel`
        4. `systemd-relabel`

        Answer:

        B.  Using the `touch` command to touch the file `/.autorelabel` will trigger a relabel for SELinux. The other commands shown are not valid.
181.    Which command can be used to create a new SELinux policy using a logfile of actions that have been denied by SELinux policy ?

        1. `updatese --log`
        2. `selinux --audit`
        3. `audit2allow`
        4. `genserules --log`

        Answer:

        C.  The `audit2allow` command is used to create a new set of rules based on a logfile that contains actions that have been denied. Care should be taken when doing so in order to prevent allowing processes and permissions that should not be allowed. The other commands shown in this scenario are not valid.
182.    You have used `getenforce` to verify that the current mode is Enforcing and need to change certain rules in real time. Which command can be used for this purpose?

        1. `systemd-selinux`
        2. `sechange`
        3. `semanage`
        4. `setsepol`

        Answer:

        C.  The `semanage` command can be used to make changes such as ports, booleans, and contexts in order to keep a policy in Enforcing mode but still make changes. The other commands shown are not valid for this purpose.
183.    Assuming a Fedora system, which command can be used to change the policy, such as changing from minimum to targeted?

        1. `setse --policy`
        2. `system-selinux`
        3. `selinux-change`
        4. `system-config-selinux`

        Answer:

        D.  The `system-config-selinux` command is used to change policies on a Fedora system. The other commands shown are not valid.
184.    Which of the following is the correct syntax to remove the group ID (SGID) bit on a directory using the `chmod` command?

        1. `chmod group-sgid directory`
        2. `chmod g-s directory`
        3. `chmod sgid -r directory`
        4. `chmdo -r gs directory`

        Answer:

        B.  The `g-s` syntax removes the SGID bit from a directory. The other syntax is incorrect and invalid for `chmod`.
185.    When using `pkexec` with PolicyKit, which option specifies the user under which the program will be executed?

        1. `--username`
        2. `--account`
        3. `--user`
        4. `--login`

        Answer:

        C.  The `--user` option specifies the user under which the program will be executed. The other options are not valid for this purpose.
186.    Which of the following is the correct syntax to enable port forwarding so that connections to local port 5150 will be sent to `www.example.com` on port 80?

        1. `-L www.example.com:80->5150`
        2. `-L 5150:www.example.com:80`
        3. `-L 5150->www.example.com:80`
        4. `-F 5150->www.example.com:80`

        Answer:

        B.  Local forwarding is accomplished with `-L`. The first port is the local port, which is then followed by the destination hostname and port. The other answers do not use the correct syntax for this scenario.
187.    Which of the following represents an accurate statement about stateless firewalls?

        1. Stateless firewalls have three zones: internal, external, and DMZ.
        2. Stateless firewalls are the only type available in Linux.
        3. Stateless firewalls examine packet headers to connect related packets.
        4. Stateless firewalls examine source and destination.

        Answer:

        D.  A stateless firewall examines only the source and destination and does not inspect elements inside packets. Stateless firewalls are not typically associated with particular zones such as internal, external, or DMZ, thus making option A incorrect. Linux has firewalls that can be configured as stateful, thus making option B incorrect.
188.    Which configuration option within `/etc/login.defs` sets the minimum value for a user ID (UID)?

        1. `UID_MIN`
        2. `MIN_UID`
        3. `USERID_MIN`
        4. `UID_MINIMUM`

        Answer:

        A.  The UID\_MIN configuration option defines the lowest value that will be used when creating users. The other configuration options shown are not valid.
189.    Assuming that you own and operate the domain [`example.com`](http://example.com/), when viewing additional details about an SSL certificate, the valid hosts are shown as `*.`[`example.com`](http://example.com/). Based on this information, what can you tell about this certificate?

        1. It is a wildcard certificate.
        2. It is a self-signed certificate.
        3. It is invalid for [`example.com`](http://example.com/).
        4. It uses an invalid hostname.

        Answer:

        A.  The presence of an asterisk within the name `*.`[`example.com`](http://example.com/) indicates that this is a wildcard certificate. While the certificate may be self-signed, there is not enough detail within the given information to determine the chain of trust. An asterisk is not a valid hostname for DNS but is valid to indicate a wildcard certificate.
