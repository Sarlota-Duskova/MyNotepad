# Questions

1.  Which command enables you to view the current IRQ assignments?

    1. `view /proc/irq`
    2. `cat /proc/interrupts`
    3. `cat /dev/irq`
    4. `less /dev/irq`

    Answer:

    B.  Current interrupt (IRQ) assignments are contained in the file `/proc/interrupts`. Therefore, viewing the contents of the file with a command such as `cat` will work. There is no `view` command, thus making option A incorrect. Likewise, there is no `/dev/irq` file, making options C and D incorrect.
2.  Configuration of udev devices is done by working with files in which directory?

    1. `/udev/devices`
    2. `/devices/`
    3. `/udev/config`
    4. `/etc/udev`

    Answer:

    D.  Configuration files for udev are found in `/etc/udev`, which makes option D correct. The other options do not exist.
3.  Which command is used to automatically load a module and its dependencies?

    1. `modprobe`
    2. `lsmod`
    3. `insmod`
    4. `rmmod`

    Answer:

    A.  The `modprobe` command loads the module and its dependencies, if applicable. The `lsmod` command is used to list currently loaded modules, making option B incorrect. The `insmod` command will load a given module but not its dependencies. Option D, `rmmod`, is used to remove a module from memory.
4.  During boot of a system with GRUB, which key can be pressed to display the GRUB menu?

    1. Shift
    2. E
    3. V
    4. H

    Answer:

    A.  The Shift key, if pressed when control has first been handed to GRUB, will cause the GRUB menu to be displayed.
5.  Which command can be used to view the kernel ring buffer in order to troubleshoot the boot process?

    1. `lsboot`
    2. `boot-log`
    3. `krblog`
    4. `dmesg`

    Answer:

    D.  The `dmesg` command displays the contents of the kernel ring buffer. On many Linux distributions, this log is also saved to `/var/log/dmesg`. The other options shown for this question are not valid commands.
6.  Which statement best describes the following, displayed using the `ls -la` command?

    `lrwxrwxrwx. 1 root root 35 Jul 8 2014 .fetchmailrc -> .configs/fetchmail/.fetchmailrc`

    1. It is a file called `.fetchmailrc` that is linked using a symbolic link.
    2. It is a file called `.configs/fetchmail/.fetchmailrc` that is owned by lrwxrwxrwx.
    3. It is a directory called `.fetchmailrc` that is owned by user Jul.
    4. It is a local directory called `.configs/fetchmail/.fetchmailrc`.

    Answer:

    A.  The listing shows a symbolic linked file located in the current directory, linked to `.configs/fetchmail/.fetchmailrc`. The file is owned by the root user and root group and was created on July 8, 2014.
7.  Which command is used with systemd in order to list the available service units?

    1. `systemd list-units`
    2. `systemctl list-units`
    3. `systemd unit-list`
    4. `systemctl show-units`

    Answer:

    B.  The `systemctl` command is used to work with services and targets. The `list-units` command is used to list targets. The other commands are not used for this purpose or do not exist with the required option.
8.  Which option to `lspci` is used to display both numeric codes and device names?

    1. `-numdev`
    2. `-n`
    3. `-nn`
    4. `-devnum`

    Answer:

    C.  The `-nn` option displays both numbers and device names, thus making option C correct. The `-n` option (option B) displays only numbers. The other two options do not exist.
9.  Which command and option can be used to determine whether a given service is currently loaded?

    1. `systemctl --ls`
    2. `telinit`
    3. `systemctl status`
    4. `sysctl -a`

    Answer:

    C.  Out of the options given, the `systemctl status` command and option are the most appropriate. The `telinit` and `sysctl` commands are not used for this purpose. Likewise, the `--ls` option is not valid for `systemctl`.
10. When partitioning a disk for a mail server running Postfix, which partition/mounted directory should be the largest in order to allow for mail storage?

    1. `/etc`
    2. `/usr/bin`
    3. `/mail`
    4. `/var`

    Answer:

    D.  The partition containing `/var` should be the largest for a mail server because mail spools are stored within this hierarchy. The `/etc/` hierarchy is usually small, as is `/usr/bin`. The `/mail` directory does not exist by default.
11. Which YUM option displays the dependencies for the package specified?

    1. `list`
    2. `deplist`
    3. `dependencies`
    4. `listdeps`

    Answer:

    B.  The `deplist` option displays the dependencies for the given package. The `list` option displays information about a specific package, while the other two options are not valid.
12. Which options for an `rpm` command will display verbose output for an installation along with progress of the installation?

    1. `-ivh`
    2. `-wvh`
    3. `--avh`
    4. `--ins-verbose`

    Answer:

    A.  The `-ivh` options will install a file using `rpm`, displaying both verbose output and hash marks for progress. The other options presented do not exist or do not accomplish the specified task.
13. Which command will search for a package named `zsh` on a Debian system?

    1. `apt-cache search zsh`
    2. `apt-get search zsh`
    3. `apt-cache locate zsh`
    4. `apt-search zsh`

    Answer:

    A.  The `apt-cache` command is used to work with the package cache, and the `search` option is used to search the cache for the supplied argument, in this case `zsh`. The `apt-get` command is used to work with packages themselves, while the `apt-search` command does not exist.
14. Which `rpm` option can be used to verify that no files have been altered since installation?

    1. `-V`
    2. `-v`
    3. `--verbose`
    4. `--filesum`

    Answer:

    A.  The `-V` or `--verify` option will check the files in a given package against versions (or checksums) in the package database. If no files have been altered, then no output is produced. Note that output may be produced for files that are changed during installation or for other reasons. Note also the use of an uppercase `V` for this option as opposed to the lowercase `v` for `verbose`.
15. Which of the following command lines would monitor a single process called nagios in a continuous manner?

    1. `top -n 1`
    2. `top -p 23`
    3. `ps -nagios`
    4. `top -p‘pidof nagios’`

    Answer:

    D.  The `top` command is used to continuously monitor things like CPU and memory usage, and the `-p` option monitors a single process. By using the runquotes with the `pidof` command, the process ID is provided as input to the `-p` option. It's worth noting that this only works if there's a single instance of the process.
16. Which option to `xfs_metadump` displays a progress indicator?

    1. `-g`
    2. `-p`
    3. `-f`
    4. `-v`

    Answer:

    A.  The `-g` option displays the progress of the dump. The other options listed do not exist.
17. The SAN has crashed again, and one of the filesystems in a Linux server has become significantly corrupt as a result. Which command and option can be used to attempt to examine the contents of the drive without causing more damage?

    1. `fdisk -f`
    2. `mke2fs -c`
    3. `debugfs -c`
    4. `ls -a`

    Answer:

    C.  The `debugfs` command can be used for this purpose. When the filesystem is opened with `–c`, it opens in catastrophic mode, meaning that it will be read-only and will not read inodes when opening.
18. Which of the following commands helps you to determine information about a given window within an X session, including information on the window size and its position?

    1. `xkbinfo`
    2. `xdspy`
    3. `xwininfo`
    4. `xver`

    Answer:

    C.  The `xwininfo` command displays information about a given window within an X session. The other commands listed are not valid.
19. Which file is used to indicate the local time zone on a Linux server?

    1. `/etc/timez`
    2. `/etc/timezoneconfig`
    3. `/etc/localtime`
    4. `/etc/localtz`

    Answer:

    C.  The file `/etc/localtime`, which can be an actual file or a symbolic link, is used to indicate the local time zone. The other files listed as options do not exist.
20. Within which directory will you find files related to the time zone for various regions?

    1. `/etc/timezoneinfo`
    2. `/etc/zoneinfo`
    3. `/var/zoneinfo`
    4. `/usr/share/zoneinfo`

    Answer:

    D.  Within the `/usr/share/zoneinfo` hierarchy, you will find information on the various regions and time zones available. The files within this hierarchy can be symlinked to `/etc/localtime`.
21. Within which directory should you place files in order for the files to be copied to a user's home directory when the user is created?

    1. `/etc/skel`
    2. `/etc/homedir`
    3. `/home/usertemplate`
    4. `/etc/template`

    Answer:

    A.  The `/etc/skel` directory contains files that are automatically copied to a user's home directory when that user is created. The other directories listed for this question do not exist by default.
22. Which command displays a list of jobs currently scheduled with `at`?

    1. `atlist`
    2. `atq`
    3. `atl`
    4. `at --jobs`

    Answer:

    B.  The `atq` command shows a list of jobs that have been scheduled with the `at` command. The other commands don't exist, with the exception of option D, which shows the `at` command but with an invalid option (`--jobs`).
23. Which of the following encodings provides a multibyte representation of characters?

    1. ISO-8859
    2. UTF-8
    3. ISO-L
    4. UFTMulti

    Answer:

    B.  UTF-8 provides multibyte character encoding and is generally accepted as the standard for encoding moving forward. ISO-8859 is single-byte encoded. The other options are not valid.
24. On which port does LDAP over SSL operate?

    1. Port 53
    2. Port 389
    3. Port 636
    4. Port 443

    Answer:

    C.  LDAP over SSL (LDAPS) operates on port 636. Port 53 is used for DNS; port 389 is used for normal, non-SSL LDAP; and port 443 is used for HTTP over SSL.
25. Which of the following commands will set an account to expire based on the number of days elapsed since January 1, 1970?

    1. `passwd -e`
    2. `chage -E`
    3. `usermod -l`
    4. `chguser`

    Answer:

    B.  The `chage` command can be used for this purpose, and the `-E` option accepts days since 1/1/1970. There is no `-e` option to `passwd`, and `-l` for `usermod` will not perform the action described. There is no `chguser` command.
26. Which option to SSH enables the use of a key for authentication?

    1. `-i`
    2. `-k`
    3. `-f`
    4. `--key`

    Answer:

    A.  The `-i` option for SSH is followed by the private key to use for authentication. Doing so implies that the public key is in the `authorized_keys` file on the remote host. The `-k` option disables the sending of GSSAPI credentials, while `-f` is used to request backgrounding of SSH. There is no `--key` option.
27. In a scripting scenario, you need to prevent `sudo` from prompting for credentials or for any other reason. Which option to `sudo` is used to indicate this?

    1. `-n`
    2. `--noprompt`
    3. `-i`
    4. `-q`

    Answer:

    A.  The `-n` option facilitates the scenario described and will exit nonzero rather than prompting. The `-i` option sets the login name and is not valid for this scenario. The `-q` and `--noprompt` options do not exist.
28. Which runlevel is typically used for single user mode, as indicated in `/etc/inittab`?

    1. 1
    2. 2
    3. 5
    4. 6

    Answer:

    A.  Single-user mode is typically runlevel 1. In runlevel 1, no network services are started, and it is known as `rescue.target` in systemd. Runlevel 2 has networking but typically not services. Runlevel 5 is full multiuser with networking, and runlevel 6 is reboot.
29. Which of the following commands provides an overview of the current memory usage along with swap space and its current utilization?

    1. `mem`
    2. `free`
    3. `pstat`
    4. `swap`

    Answer:

    B.  The `free` command shows current memory usage for both RAM and swap space, including total available, current amount used, and current amount free. The other commands shown as options do not exist.
30. Which of the following commands can be used to display the current disk utilization, including free space?

    1. `df`
    2. `du`
    3. `diskutil`
    4. `diskuse`

    Answer:

    A.  The `df` command displays information on disk usage and can help with planning disk utilization over time. For example, if you note that the disk utilization is increasing significantly, preparations can be made to bring more disks online or even to change the log-rotation schedule such that logs are rotated faster, thereby freeing up space.
31. Which of the following commands displays CPU-related performance information a total of 10 times gathered every 2 seconds?

    1. `sar -u 2 10`
    2. `sar -u 10 2`
    3. `sar -u 2`
    4. `uptime -t`

    Answer:

    A.  The `sar` command can be used for this purpose and, when provided with numbers in the format displayed, will update every X seconds for Y executions.
32. Which option to `iostat` causes the display to output in megabytes?

    1. `-k`
    2. `-l`
    3. `-m`
    4. `-o m`

    Answer:

    C.  The `-m` option causes the disk-related statistics to use megabytes as the scale rather than the default kilobytes.
33. You are working with a legacy CentOS 5 system and need to re-create the initial RAM disk. Which of the following commands is used for this purpose?

    1. `mkinitrd`
    2. `mkramdisk`
    3. `mkdisk --init`
    4. `mkfs.init`

    Answer:

    A.  The `mkinitrd` command is used on older systems to create the initial RAM disk. The initial RAM disk is used to load, some might say preload, essential modules for things like disks and other vital components needed for booting.
34. Which compression method is used for creation of a bzImage?

    1. zip
    2. bzip3
    3. gzip
    4. Cannot be determined

    Answer:

    D.  A bzImage can mean that `bzip` was used to compress the image but can also mean simply “Big zImage” and compressed with `gzip`. bzImage is typically used for kernel images that can go above the 512 K limit that normally applies to a zImage.
35. Which options to the `fsck` command will find errors and automatically assume that it should repair them?

    1. `-ry`
    2. `-vy`
    3. `-my`
    4. `-xy`

    Answer:

    A.  The `-r` option repairs the filesystem, while the `-y` option causes `fsck` to assume Yes instead of prompting. The `-v` option is verbosity. There is no `-m` or `-x` option for `fsck`.
36. What is the name of the unit to which a `systemd` system is booted in order to start other levels?

    1. `default.target`
    2. `init.target`
    3. `initial.target`
    4. `load.target`

    Answer:

    A.  The `default.target` is the default target unit that is activated by `systemd` on boot. The default target then starts other services based on the dependencies.
37. Which command is used to format a swap partition?

    1. `mkfs -swap`
    2. `mkswap`
    3. `format -swap`
    4. `mksw`

    Answer:

    B.  The `mkswap` command is used to format a swap partition. The other commands are not valid.
38. You see the word `defaults` within `/etc/fstab`. Which options are encompassed within the defaults?

    1. `ro`, `exec`, `auto`
    2. `rw`, `suid`, `dev`, `exec`, `auto`, `nouser`, `async`
    3. `rw`, `exec`, `auto`, `nouser`, `async`
    4. `rw`, `exec`, `nouser`, `async`, `noauto`, `suid`

    Answer:

    B.  A filesystem with the word `defaults` for its mount options will be mounted read-write (`rw`), `suid`, with the ability to have executables (`exec`). The filesystem will be auto-mounted (`auto`), but users will not be able to mount it (`nouser`). Character and block special devices will be interpreted (`dev`), and operations on the disk will be performed in an asynchronous manner (`async`).
39. Which command is used to remove unused filesystem blocks from thinly provisioned storage?

    1. `thintrim`
    2. `thtrim`
    3. `fstrim`
    4. `fsclean`

    Answer:

    C.  The `fstrim` command is used to remove blocks that are not in use. The `fstrim` command is frequently used in a SAN configuration to give back unused storage to the SAN. The `fstrim` command can also be used with solid-state drives for the same purpose. The other commands shown are not valid.
40. Which option to `mdadm` is used to create a new array?

    1. `--create`
    2. `--start`
    3. `--begin`
    4. `--construct`

    Answer:

    A.  The `--create` option enables creation of a RAID array that will use `md`. The typical argument is the `/dev/mdN` device. The other options listed are not valid for `mdadm`.
41. Which of the following commands creates a logical volume with LVM?

    1. `lvc`
    2. `lvcreate`
    3. `lvlist`
    4. `lvmake`

    Answer:

    B.  The `lvcreate` command is used to create a logical volume from previously created physical devices and volume groups. Using `lvcreate` is the final of three steps in the process for using LVM prior to actually using the logical volume.
42. Which of the following commands shows network sockets and their allocated memory?

    1. `ss -m`
    2. `mpas`
    3. `mem`
    4. `free`

    Answer:

    A.  The `ss` command provides many of the same functions as `netstat` but can show some extended information, such as memory allocation for a given socket. The `free` command shows memory usage but not by socket, and the other two commands do not exist.
43. When troubleshooting a potential hardware problem, you need to determine which physical interface is being used for a certain address. One way to accomplish this is with the `ping` command in order to monitor the activity lights on the device. Which of the following options to `ping` will flood the interface with `ECHO_REQUEST` packets?

    1. `-e`
    2. `-a`
    3. `-c`
    4. `-f`

    Answer:

    D.  The `-f` option is a flood ping. This will effectively cause the interface to send and receive large amounts of traffic, usually making it easier to find on a switch. The `-a` option is an audible ping, emitting a sound on `ping`. The `-c` option sends a certain count of pings, and there is no `-e` option.
44. Which of the following `dd` commands reads and writes bytes one megabyte at a time?

    1. `dd bsl=1024M`
    2. `dd size=1M`
    3. `dd bs=1M`
    4. `dd rw=1M`

    Answer:

    C.  The `bs` option is used to specify block size. Various suffixes are possible, such as `M`, which is equivalent to megabytes, and `K`, which is equivalent to kilobytes.
45. Which option to the `rsync` command examines only the file size as a means of determining whether the file should be synchronized?

    1. `--filesize`
    2. `--size-only`
    3. `--list-size`
    4. `--file-size`

    Answer:

    B.  The `--size-only` option examines whether the files being synchronized are the same size. This can be helpful for situations where there may be significant time skew or other issues preventing the normal differencing mechanisms from working properly. The other options shown are not valid for `rsync`.
46. When creating MX records for a zone, which of the following is the highest-priority mail exchanger?

    1. 0
    2. 10
    3. 20
    4. 100

    Answer:

    A.  The lowest-priority number wins for MX records, thereby making 0 the highest-priority MX record for the domain.
47. On which protocol and port are zone transfer requests sent?

    1. UDP/53
    2. ICMP/53
    3. TCP/143
    4. TCP/53

    Answer:

    D.  DNS typically uses UDP port 53 except for zone transfers, in which case TCP port 53 is used due to the size of the request for most zones.
48. Which type can be used with the `dig` command to test a zone transfer?

    1. `xfr`
    2. `transfer`
    3. `zxfr`
    4. `axfr`

    Answer:

    D.  The `axfr` type can be used with `dig` to request a zone transfer. The client from which you request the zone transfer will need to be authorized to initiate a transfer.
49. Which of the following files is used to define the filesystems shared by NFS?

    1. `/etc/nfs.cfg`
    2. `/etc/nfs.conf`
    3. `/etc/export.nfs`
    4. `/etc/exports`

    Answer:

    D.  The file `/etc/exports` contains definitions of filesystems to be shared using NFS. The other files are not valid for use with NFS.
50. Which option in `dhcpd.conf` specifies the maximum amount of time that a client is allowed to have a DHCP lease?

    1. `max-time`
    2. `max-lease-time`
    3. `lease-max`
    4. `maximum-lease-duration`

    Answer:

    B.  The `max-lease-time` directive, followed by the number of seconds, specifies the amount of time that a given host can have a lease before it is purged. The other options shown are not valid in a `dhcpd.conf` configuration file.
51. You are troubleshooting an authentication issue for a user. You believe the system uses local files and LDAP for authentication. Which of the following lines in `/etc/nsswitch.conf` shows those authentication mechanisms?

    1. `passwd: files ldap`
    2. `passwd [files ldap]`
    3. `auth: local ldap`
    4. `auth: localfiles ldap`

    Answer:

    A.  Within `nsswitch.conf`, the `passwd` line contains information about authentication. The format is as shown in the correct answer. Local authentication is accomplished using the `files` keyword for the normal `passwd` file. There is typically a similar line called `shadow`, assuming that the server is using shadow passwords. The `shadow` line follows a similar format.
52. Which of the following commands can be used to generate a private and public key pair for authentication with SSH?

    1. `ssh-createkey`
    2. `sshkey`
    3. `ssh-key`
    4. `ssh-keygen`

    Answer:

    D.  The `ssh-keygen` command generates a public and private key pair that can be used for user authentication between a client and server. The other commands shown are not valid.
53. Which file contains a list of keys that will be accepted for authentication for a given user?

    1. `~/ssh/keys`
    2. `~/.ssh/pubkeys`
    3. `~/.ssh/keyauth`
    4. `~/.ssh/authorized_keys`

    Answer:

    D.  The file `authorized_keys` contains keys that can be used for authentication when the corresponding private key is sent by the client. The other files are not valid.
54. A newly added SATA disk is not showing up during the boot process. Where can you check to begin troubleshooting this issue?

    1. Using system logging
    2. Using `debugfs`
    3. Within the `fdisk` utility
    4. Within the computer BIOS or firmware

    Answer:

    D.  A logical location to begin troubleshooting is within the system BIOS or firmware to ensure that the drive is being detected by the computer.
55. Which of the following commands will set the environment variable `JAVA_PATH` equal to `/home/user/java2` when using the Bash shell?

    1. `invoke JAVA_PATH=/home/user/java2`
    2. `export JAVA_PATH=/home/user/java2`
    3. `envvar JAVA_PATH=/home/user/java2`
    4. `echo JAVA_PATH=/home/user/java2`

    Answer:

    B.  The `export` command is used for this purpose and accepts a `name=value` pair, as shown in the answer. The other commands are not valid, with the exception of the `echo` command, which will simply echo the argument to the console.
56. Which option in `.bashrc` sets the number of commands to keep in the `.bash_history` file?

    1. `HISTLIMIT`
    2. `HISTORYFILE`
    3. `HISTFILESIZE`
    4. `HISTNUM`

    Answer:

    C.  The `HISTFILESIZE` option configures the number of commands to keep in the history file. The other variables are not valid within Bash.
57. You are creating a Bash script of user information. Which of the following commands prints the username and real name of all users in `/etc/passwd` in a tab-separated format?

    1. `cut -d: -f 1,6 /etc/passwd`
    2. `sed 's/://' /etc/passwd`
    3. `awk -F: '{print $1,$5}' OFS=“\t” /etc/passwd`
    4. `cat -o “\t” /etc/passwd`

    Answer:

    C.  The `awk` command shown can be used for this purpose. The `-F` option sets the field separator, and the `OFS` option sets the output field separator.
58. Which `git clone` command will clone a repository called `portalutils` into a directory called `utils`?

    1. `git clone ssh://sourcehost/portalutils -d utils`
    2. `git clone ssh://sourcehost:portalutils utils`
    3. `git clone ssh://sourcehost/:portalutils utils`
    4. `git clone ssh://sourcehost::portalutils -d utils`

    Answer:

    B.  The `git clone` command will clone into a different directory if that directory is passed on the command line, as shown in option B. The other options shown are not valid `git clone` syntax.
59. Which of the following commands is necessary for making a variable defined in your current shell available to child processes?

    1. `export`
    2. `source`
    3. `let`
    4. `def`

    Answer:

    A.  The `export` command is necessary so that any variables that are manually defined in your current session become available to child processes. The `source` command executes the file and can be used for the purpose described but requires an additional argument. The `let` and `def` commands are not valid.
60. You are watching another administrator perform some work on a server. As part of that work, the admin uses the following command:

    `. variables.sh`

    Which of the following is the equivalent of `. variables.sh`?

    1. `let variables.sh`
    2. `set variables.sh`
    3. `source variables.sh`
    4. `var variables.sh`

    Answer:

    C.  The `source` command is the functional equivalent of a single dot (`.`). The `set` command exists but is not used for this purpose. The other commands are not valid.
61. Which of the following shows a valid Bash function called `sayHello`?

    1. `function sayHello() { echo “hello”; }`
    2. `function sayHello{}`
    3. `function sayHello() { echo Hello }`
    4. `function sayHello() { echo Hello } ;`

    Answer:

    A.  The correct syntax is as shown. Note that a semicolon is required when the commands are included on one line, as shown in the correct answer.
62. Which option to `useradd` sets the number of days between password expiration and when the account is disabled?

    1. `-n`
    2. `-f`
    3. `-e`
    4. `-g`

    Answer:

    B.  The `-f` option sets the days between expiration and disabled for an account. The `-g` option is used to set the group ID, while `-e` is used to set the overall expiration date.
63. Which command option can be used to remove all cron jobs for a given user using the `crontab` command?

    1. `-d`
    2. `-e`
    3. `-r`
    4. `-l`

    Answer:

    C.  The `-r` option to the `crontab` command removes all cron entries for a given user. The `-l` option lists cron jobs, while the `-e` option edits the `crontab`. There is no `-d` option.
64. Which command is used to parse log-file entries on a `systemd`-based system?

    1. `logger`
    2. `journalentry`
    3. `jrnctl`
    4. `journalctl`

    Answer:

    D.  The `journalctl` command is used to view and parse log file entries on `systemd`-based systems that maintain logs in a special format. The `logger` command can be used to create log entries, and the other commands shown do not exist.
65. Which of the following syslog facilities captures messages from the `lp` printing facility?

    1. `auth`
    2. `messages`
    3. `lpr`
    4. `root`

    Answer:

    C.  The `lpr` syslog facility sends messages from the `lp` subsystem to syslog. The `auth` facility is used for security-related messages. The other listed options are not syslog facilities.
66. Which port needs to be allowed through the firewall for standard LDAP traffic to be received by the server?

    1. TCP port 25
    2. TCP port 443
    3. TCP port 143
    4. TCP port 389

    Answer:

    D.  Standard LDAP traffic is TCP port 389 on the server. TCP port 25 is SMTP, 443 is HTTPS, and 143 is IMAP.
67. Which of the following is the correct syntax to connect to `host.example.com` using SSH on port 2200?

    1. `ssh -l 2200` `host.example.com`
    2. `ssh host;` [`example.com`](http://example.com/)
    3. `ssh` `host.example.com:2200`
    4. `ssh host:2200 -d` [`example.com`](http://example.com/)

    Answer:

    C.  When connecting to an alternate port, you can use the `-p` option to set the port or use a colon to separate the host from the port.
68. Which option to the `tar` command preserves permissions?

    1. `-x`
    2. `-v`
    3. `-z`
    4. `-p`

    Answer:

    D.  The `-p` option preserves permissions. The `-x` option extracts while `-z` unzips with `gzip`. The `-v` option is `verbose`.
69. When working with a patch file, which option can be used to have the patching process ignore white space?

    1. `-w`
    2. `-i`
    3. `-e`
    4. `-p`

    Answer:

    B.  The `-i` option tells `patch` to ignore white space. This might be necessary when the patch file doesn't match exactly what's needed. The `-p` option sets the level of directory for the patch, while `-e` informs `patch` to interpret as an ed script. There is no `-w` option for `patch`.
70. When using the `dm-crypt` command, which type of encryption is used by default?

    1. plain
    2. SHA-256
    3. LUKS
    4. loop

    Answer:

    C.  LUKS encryption is the default mode for the `dm-crypt` command. Other modes include plain, loopaes, and tcrypt.
71. Which option to `journalctl` displays the output in reverse, with newest entries first?

    1. `-n`
    2. `-r`
    3. `-f`
    4. `-b`

    Answer:

    B.  The `-r` option reverses the journal, displaying the newest entries first. The `-n` option shows the most recent N events, `-f` is `follow`, and `-b` tells `journalctl` to show a message from a specific boot ID.
72. Which `systemd` target can be used as an alternative to rescue mode when recovery is not possible in rescue mode?

    1. `emerg`
    2. `recover`
    3. `control-recover`
    4. `emergency`

    Answer:

    D.  The `emergency` target can be used in situations where rescue mode cannot recover the system. The other targets are not valid.
73. When performing an `rsync` across devices, you receive errors that file ownership cannot be preserved, likely due to missing users or groups on the destination system. Which option should be removed from the `rsync` options in order to not preserve user and group ownership?

    1. `-go`
    2. `-o`
    3. `-no-ownership`
    4. `-remove-owners`

    Answer:

    A.  As specified in the question, you need to remove both group and user ownership, therefore both `-g` and `-o` are needed. The other options are not valid, although you can remove individual options from an archive process with `--no-g` and `--no-o`, which would be equivalent to removing the `-g` and `-o` options from the command.
74. Which option to `ping` enables the bypass of the routing tables?

    1. `-q`
    2. `-r`
    3. `-b`
    4. `-A`

    Answer:

    B.  The `-r` option bypasses the routing tables and enables sending packets directly using an interface. The `-A` option is adaptive `ping`, while `-b` enables sending pings to a broadcast address. The `-q` option is quiet output.
75. Which option to the `patch` command makes a backup of files?

    1. `-d`
    2. `-b`
    3. `-s`
    4. `-c`

    Answer:

    B.  The `-b` option makes a copy of the original file before patching. This can be particularly useful in a scripted scenario where several files are patched in succession. The `-d` option causes a change directory prior to patching, while `-c` tells `patch` to interpret the patch file as a normal diff file. The `-s` option causes `patch` to work in silent mode.
76. A piece of software on client machines that listens for connections and executes commands on behalf of the server in an orchestration is commonly known as which of the following?

    1. Executor
    2. Runner
    3. Agent
    4. Host

    Answer:

    C.  Orchestration software can use an agent, which is described as part of the question, or the orchestration software could also be agentless, not requiring special software to be installed on each client machine.
77. Which escape characters represent a carriage return and newline in Bash?

    1. `\enter`
    2. `\r`
    3.
    4. `\c`

    Answer:

    B.  The  escape sequence is a carriage return, and  is newline. The `\c` sequence invokes a control character and is not related to this question.
78. Which file test within a Bash script checks to see if the file exists?

    1. `-f`
    2. `-o`
    3. `-l`
    4. `-p`

    Answer:

    A.  The `-f` file test checks to see if the file exists and is useful in a scripting scenario as described.
79. Which of the following will execute a Bash script called `test.sh` even if the execute bit is not set?

    1. `./test.sh`
    2. `test.sh --execute`
    3. `bash test.sh`
    4. `run test.sh`

    Answer:

    C.  By invoking a shell specifically for the commands in the script, you can execute the contents of the script. Option A requires the execute bit to be set. The other options won't work.
80. When testing an exclude pattern for a `.gitignore` file, which `git` command and option can be used to see the results of what will be ignored?

    1. `git ls-files -i --exclude-standard`
    2. `git ls-files --ignored`
    3. `git show-ignored`
    4. `git -ls ignored`

    Answer:

    A.  The `ls-files` command will be used for this purpose, and `-i` or `--ignored` will be used, along with a required exclusion pattern, thus making option A correct. Option B is missing the required exclusion pattern.
81. Which of the following characters is used to redirect `STDIN`, sending the contents of a file called `file.txt` into a script called `script.sh`?

    1. `script.sh < file.txt`
    2. `script.sh | file.txt`
    3. `file.txt | script.sh`
    4. `./script.sh > file.txt`

    Answer:

    A.  Redirecting input from a file uses the less-than sign. Option B takes the output from `script.sh` and sends it to `file.txt`. Option C tries to use `file.txt` as input but without any way to send the contents to `STDOUT`. Option D executes `script.sh` and sends the contents to `file.txt`, which is opposite of the scenario.
82. Which option to the `tune2fs` command sets the maximum mount count before the system will automatically run `fsck` on the partition on boot?

    1. `-b`
    2. `-c`
    3. `-C`
    4. `-a`

    Answer:

    B.  The `-c` option sets the maximum mount count. The `-C` option sets the current number of mounts. The `-b` and `-a` options do not exist.
83. Which option to the `mount` command can be used to simulate the mount process without actually mounting the filesystem?

    1. `-q`
    2. `-v`
    3. `-l`
    4. `-f`

    Answer:

    D.  The `-f` option, also known as `fake`, is helpful for situations where you need to debug the mount process or when you need to add an entry to `/etc/mtab` for a previously mounted filesystem. The `-l` option shows labels, and `-v` is `verbose`. There is no `-q` option.
84. Which of the following commands shows the current default route without performing DNS lookups on the IP address(es) involved?

    1. `netstat -rn`
    2. `netstat -n`
    3. `netstat -r`
    4. `netstat -f`

    Answer:

    A.  The `netstat` command can be used for this purpose, and the `-r` option displays the current routes. The addition of `-n` prevents DNS lookups, which can help with performance.
85. Which tool can be used to measure the memory usage of individual processes in order to aid in capacity planning?

    1. `ps`
    2. `iotop`
    3. `iostat`
    4. `ifconfig`

    Answer:

    A.  The `ps` command provides information on processor and memory usage for individual processes. You can use this information to predict capacity.
86. When you're viewing statistics with `vmstat`, which statistic represents the time that the CPU spent waiting for I/O?

    1. `sy`
    2. `us`
    3. `wa`
    4. `io`

    Answer:

    C.  The `wa` statistic shows time spent waiting for I/O and can be used to measure or find a bottleneck related to disk. The `us` statistic is time spent on userspace processes, while `sy` is time spent on kernel processes. There is no statistic called `io` within `vmstat`.
87. What time intervals are represented by the three numbers in the load-average output obtained with the `uptime` command?

    1. 1, 5, and 15 minutes
    2. 5, 10, and 15 minutes
    3. 10, 30, and 60 seconds
    4. 1, 3, and 5 minutes

    Answer:

    A.  Load average with the `uptime` command is displayed in 1-, 5-, and 15-minute increments.
88. Which option to `sysctl` displays all values and their current settings?

    1. `-a`
    2. `-b`
    3. `-d`
    4. `-c`

    Answer:

    A.  The `-a` option displays all values and their current settings for `sysctl`. The `-b` option is `binary` and displays values without any newlines. The `-d` option is an alias for `–h`, which displays help. There is no `-c` option.
89. When you're using `systemctl` to kill a process, what is the default signal sent to a process?

    1. `SIGKILL`
    2. `SIGTERM`
    3. `SIGINT`
    4. `SIGCALL`

    Answer:

    B.  The `SIGTERM` signal is the default signal sent with the `systemctl kill` command.
90. You are having difficulty with shared libraries on the system. Which of the following commands will print the current directories and libraries in the cache?

    1. `ldconfig -C`
    2. `ldd -f`
    3. `ldconfig -p`
    4. `ldd -b`

    Answer:

    C.  The `ldconfig` command is used to work with the library cache, and the `-p` option prints the directories and libraries in the cache. The `-C` option informs `ldconfig` to use a different cache. The `ldd` command prints the library dependencies for a given command, but the options given don't exist for `ldd`.
91. Which flag should be found within `/proc/cpuinfo` in order to determine if a host can be configured with hypervisor support?

    1. `rob`
    2. `vmx`
    3. `run`
    4. `dmc`

    Answer:

    B.  The `vmx` flag is an indication that hypervisors will be supported on the host. The other options shown are not relevant flags for this purpose.
92. When using `ss` to determine listening sockets, you need to turn off name resolution. Which option should be passed to `ss` in order to disable name resolution?

    1. `-n`
    2. `-x`
    3. `-a`
    4. `-r`

    Answer:

    A.  The `-n` option disables name resolution, including hostnames and service names. The other options shown are not relevant flags for this purpose.
93. Which option to `systemctl` shows the current target to which the system will boot?

    1. `show`
    2. `get-default`
    3. `show-target`
    4. `get-target`

    Answer:

    B.  The `get-default` option shows the current target runlevel to which the system will boot. Of the other options, `show` displays information about configuration but not the target runlevel.
94. If you suspect there is an active memory leak on the system, which option to the `free` command displays the output every N seconds apart?

    1. `-b`
    2. `-v`
    3. `-d`
    4. `-s`

    Answer:

    D.  The `-s` option displays the output of `free` every N seconds in order to track memory usage over time while troubleshooting. The other options are not relevant for this scenario.
95. Which `docker` command displays detailed information about a container?

    1. `mine`
    2. `inspect`
    3. `show`
    4. `list`

    Answer:

    B.  The `inspect` command shows detailed information about a Docker container. The other options are not relevant for this scenario.
96. You are working with an image created by `dracut`. Which command can be used to display the contents of the image?

    1. `dsl`
    2. `dracutls`
    3. `lsinitrd`
    4. `drat`

    Answer:

    C.  The `lsinitrd` command shows information about an image created with `dracut`. The other options are not real commands.
97. Which of the following commands verifies the current status of a chronyd implementation?

    1. `chronyd info`
    2. `chronyc tracking`
    3. `chrony --info`
    4. `chrony --detail`

    Answer:

    B.  The `chronyc tracking` command shows information about the current status of time synchronization. The other options are not real commands.
98. You are troubleshooting network issues and notice a potential attack originating from a single IP address. Which command can be used to determine the owner of that IP address?

    1. `whoip`
    2. `ip-owner`
    3. `ip info`
    4. `whois`

    Answer:

    D.  The `whois` command shows information about domains and IP block ownership and would be appropriate in this scenario. Of the other options, there is an `ip` command but no `info` subcommand. The other options are not real commands.
99. When you're working with the `nftables` command to build a web front end, which option to `nftables` prints output in JSON format?

    1. `-j`
    2. `-i`
    3. `-m`
    4. `-s`

    Answer:

    A.  The `-j` option returns output in JSON format. Of the other options, `-i` is used for interactive command-line interface, `-s` shows statistics, and there is no `-m` option.
100.    Which of the following commands displays only IPv6-related connections?

        1. `ss -o 6`
        2. `ss 6-ip`
        3. `ss ipv6`
        4. `ss -6`

        Answer:

        D.  The `-6` option to the `ss` command displays IPv6 connections. The other options shown are not valid.
101.    Within which directory will you find configuration files for the Postfix mail server on a Debian-based Linux server?

        1. `/etc/postfixd`
        2. `/var/postfix`
        3. `/etc/postfix`
        4. `/var/postfixd`

        Answer:

        C.  The configuration files for Postfix are stored in /etc/postfix on a Debian server. Of the other answers, none of the directories exist by default.
102.    A developer is reporting that their webpage called index.html cannot be viewed on the web. While re-creating the issue, you receive the error “Forbidden” in a web browser and you notice that the file's permissions appear as `-rw-------` on the server. Using this information, which of the following describes the problem and its solution and, if applicable, the command to correct this issue?

        1. The developer did not load the file into the correct location. Move the file with the command `mv /var/web/`
        2. The file's permissions do not allow the file to be read and the chmod 644 command will correct the issue.
        3. The file does not exist. Have the developer upload the file to the server.
        4. The file has the wrong extension. Rename the file with `ren index.html index.htm`

        Answer:

        B.  Given the Forbidden error and the permissions shown, chmod 644 will change the permissions to allow the file to be world-readable. Of the other options, the scenario did not describe the directories; thus there isn't enough information and also the mv command shown is incomplete. Option C cannot be true based on the scenario showing the permissions for the file. Option D might be correct but renaming a file in Linux requires the use of the mv command.
