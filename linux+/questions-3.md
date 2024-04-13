# Questions

1.  While troubleshooting a network service that does not appear to start, which option to the `ss` command shows the current TCP listening sockets?

    1. `-lt`
    2. `-ct`
    3. \-`m`
    4. \-`f`

    Answer:

    A.  The `-l` option displays listening ports and the `-t` option limits the ports to TCP only, thus making `-lt` correct. The `-m` option shows socket memory usage and `-f` is used to define the family to return. There is no `-c` option, thus making option B incorrect.
2.  You are examining a problem report where a USB disk is no longer available. Which command is used to obtain a list of USB devices?

    1. `usb-list`
    2. `lsusb`
    3. `ls-usb`
    4. `ls --usb`

    Answer:

    B.  The `lsusb` command is used to obtain a basic list of USB devices on a system. The other commands are not valid. In the case of option D, the `ls` command is valid, but there is no `--usb` option.
3.  You have lost the password for a server and need to boot into single user mode. Which option given at boot time within the GRUB configuration will start the system in single user mode to enable password recovery and/or reset?

    1. `single-user`
    2. `su`
    3. `single`
    4. `root`

    Answer:

    C.  The keyword `single` given on the Linux kernel command line will boot the system into single user mode. The other options are not valid.
4.  Which of the following is a good first troubleshooting step when a hard disk is not detected by the Linux kernel?

    1. Unplug the disk.
    2. Check the system BIOS.
    3. Restart the web server service.
    4. Run the `disk-detect` command.

    Answer:

    B.  Checking to ensure that the disk is detected in the BIOS is a good first step in troubleshooting. Option A, unplugging the disk, won't help it to be detected. Restarting the web server won't help detect the disk, and the `disk-detect` command does not exist.
5.  Which command and option are used to set the maximum number of times a filesystem can be mounted between running `fsck`?

    1. `tune2fs -c`
    2. `dumpe2fs`
    3. `tune2fs -m`
    4. `setmount`

    Answer:

    A.  The `tune2fs` command is used for this purpose, and the `-c` option sets the mount count for the specified partition. The `dumpe2fs` command is used to print the superblock and block group information.
6.  When checking filesystems with the `fsck` command, which option skips checking of the root filesystem?

    1. `-A`
    2. `-M`
    3. `-R`
    4. `-S`

    Answer:

    C.  The `-R` option skips the root filesystem when the `-A` option is used. The `-M` option does not check mounted filesystems. There is no `-S` option.
7.  You have connected a USB disk to the system and need to find out its connection point within the system. Which of the following is the best method for accomplishing this task?

    1. Rebooting the system
    2. Viewing the contents of `/var/log/usb.log`
    3. Connecting the drive to a USB port that you know the number of
    4. Running `dmesg` and looking for the disk

    Answer:

    D.  Of the options presented, running `dmesg` is a common way to find out the location to which the kernel has assigned the drive. Rebooting the system is not a good option, although it would work. There is no such thing as `/var/log/usb.log`, and the location of the drive may change regardless of port, depending on how the drive may be detected in the system.
8.  How many SCSI devices are supported per bus?

    1. 7 to 15
    2. 2 to 4
    3. 12
    4. 4

    Answer:

    A.  SCSI supports 7 to 15 devices per bus, depending on the type of SCSI.
9.  Within which folder are systemd unit configuration files stored?

    1. `/etc/system.conf.d`
    2. `/lib/system.conf.d`
    3. `/lib/systemd/system`
    4. `/etc/sysconfd`

    Answer:

    C.  Unit configuration files are stored in `/lib/systemd/system`. The other directory options for this question are not relevant or do not exist by default.
10. You are troubleshooting a service not starting on time. Which network unit target waits until the network is up, such as with a routable IP address?

    1. `network.target`
    2. `network-online.target`
    3. `network-up.target`
    4. `network-on.target`

    Answer:

    B.  The `network-online.target` is used to signify that the network is online and operational for services that depend on the network. Of the other options, `network.target` is a legitimate target but is typically used to help with an orderly shutdown to ensure that services are stopped prior to the network. The other options shown are not valid.
11. To which file should a unit file be symlinked in order to disable the unit file?

    1. `/etc/systemd/unit.disable`
    2. `/etc/systemd/disabled`
    3. `/tmp/disabled`
    4. `/dev/null`

    Answer:

    D.  Creating a symbolic link to `/dev/null` effectively disables the unit file so that the service cannot be started. The other options shown are not valid files.
12. You are troubleshooting a service that does not stop correctly. During troubleshooting, you find that the command to stop the service needs to be changed. Which configuration option specifies the command to execute for stopping a service?

    1. `StopCmd`
    2. `ExecStop`
    3. `StopScript`
    4. `StopSvc`

    Answer:

    B.  The `ExecStop` configuration option specifies the command that should be executed to stop the service. The other options shown are not valid for this purpose.
13. You are working with a service dependency issue where a service is starting even though it depends on a different service. The unit file currently lists the dependency with `Wants=`. To what should the `Wants=` be changed to in order to make the requirement stronger between the two services?

    1. `Needs=`
    2. `LoadFirst=`
    3. `Verify=`
    4. `Requires=`

    Answer:

    D.  Using `Wants=` creates a weak dependency between two services, while using `Requires=` creates a stronger dependency. The other options shown are not valid unit dependency directives.
14. When troubleshooting potential collisions for a network interface, which option to the `ip` command displays additional information that includes a count of collisions?

    1. `-s`
    2. `-c`
    3. `-o`
    4. `-f`

    Answer:

    A.  Using the `-s` option displays statistics including a count of collisions that have occurred for the interface. Of the other options, `-c` changes output colors, `-o` prints all information on one line, and `-f` changes the family.
15. Which of the following is true of Linux swap space?

    1. Swap is used to hold temporary database tables.
    2. Swap is used as additional memory when there is insufficient RAM.
    3. Swap is used by the mail server for security.
    4. Swap is used to scrub data from the network temporarily.

    Answer:

    B.  Swap space is used when there is insufficient RAM memory on a system.
16. You are running a Linux instance on a cloud provider and notice slow performance. Which CPU time metric helps to determine if cycles are being used by other instances on the same hypervisor?

    1. HyperV
    2. CircleTime
    3. Steal
    4. CrossProc

    Answer:

    C.  Steal is the metric used to measure the number of cycles being used by other virtual instances in either a cloud or virtualization scenario. The steal metric is abbreviated as `st` in the output of `top`. The other options are not valid for this scenario.
17. You need to examine the hardware to determine if the processor supports virtualization. Which command can be used to display the status of virtualization support?

    1. `cpustat`
    2. `cpuinfo`
    3. `lscpu`
    4. `brcxpu`

    Answer:

    C.  The `lscpu` command shows statistics about the CPU that include architecture, cache, speed, and other information. Among the other options, `cpuinfo` is not a command but rather the file `/proc/cpuinfo` contains the same information as `lscpu`. The other options are not valid commands.
18. When you're troubleshooting a file access issue for a user, which command can be run in order to determine if the issue is related to SELinux policy?

    1. `ls -P`
    2. `pol --info`
    3. `showpol`
    4. `ls -Z`

    Answer:

    D.  The `ls -Z` command shows information regarding the SELinux security context applied to a file and can help determine if the issue is policy/non-policy related. There is no `-P` option and the other commands shown are not valid.
19. Which of the following commands can be used to help troubleshoot an application crash that may be related to system calls?

    1. `strace`
    2. `systemt`
    3. `systemd-trace`
    4. `systemd-debug`

    Answer:

    A.  The `strace` command is vital to debugging system-call-related application crashes, especially when the daemon or service does not log any error but silently crashes. The other commands are not valid.
20. Which setting should be changed in journald.conf in order to ensure that journal log files are written to disk?

    1. `Location=`
    2. `Persistence=`
    3. `Storage=`
    4. `WriteTo=`

    Answer:

    C.  The `Storage=` option controls whether journal logs are written to disk, kept in memory, or not kept at all. The other options shown are not valid for journald.conf.
21. As part of troubleshooting services not starting on time, you need to add a service to be started before another to an already-existing systemd unit file. What delimiter is used to separate services with the `Before=` and `After=` configuration options in a systemd unit file?

    1. Comma
    2. Semicolon
    3. Colon
    4. Space

    Answer:

    D.  A space is used to separate services within a systemd unit file on the `Before=` and `After=` configuration lines. The other delimiters shown as options are not valid for this purpose.
22. When using the `du` command to diagnose which directories are large, you would like to summarize the output in a more human-friendly format. Which option(s) should be used?

    1. `--summarize`
    2. `-uh`
    3. `-h`
    4. `-sh`

    Answer:

    D.  The `-s` option summarizes the output by directory, while the `-h` option presents the output in a more human-friendly manner.
23. Which option to `tune2fs` forces the operation to complete in the event of a problem such as corruption?

    1. `-f`
    2. `-m`
    3. `-x`
    4. `-k`

    Answer:

    A.  The `-f` option forces the specified operation to complete and can sometimes be necessary if there is no other option to fix the issue. However, data loss can occur with this option so care must be taken when using it. The other options shown are not valid.
24. You have purchased new SSD hardware that uses the NVMe protocol, but you cannot find the disks in the normal `/dev/sd*` location where you have traditionally found such storage. In which location should you look for these drives?

    1. `/dev/nd*`
    2. `/dev/nvme*`
    3. `/dev/nv*`
    4. `/dev/nvme/*`

    Answer:

    B.  NVMe-capable drives are named as `/dev/nvme*`. No special drivers are needed other than those found in the native kernel on a modern system. The other answers do not exist as paths by default.
25. Which of the following commands mounts `/dev/sda1` in the `/boot` partition?

    1. `mount /dev/sda /boot`
    2. `mount /boot /dev/sda1`
    3. `mount /dev/sda1 /boot`
    4. `mount -dev sda1 /boot`

    Answer:

    C.  The format for the `mount` command is `[partition] [target]`, thereby making option C correct. The other options are not valid because the arguments are in the wrong order.
26. Using `vmstat` to examine the run queues on a single processor system with four cores reveals that there are six jobs in '`r`' status. Which of the following describes the current situation?

    1. There are four jobs running and two waiting in the run queue.
    2. There are six jobs running.
    3. There is one job running and there are five in the run queue.
    4. The '`r`' column describes regulated processes and not the run queue.

    Answer:

    A.  Each processor core can run a job, meaning that there are four available run queues on the system described in this scenario. Four of the six processes are therefore running while two are waiting in the run queue. Presence of high run queues can mean that additional processors are needed or that applications should be changed to utilize existing resources more efficiently.
27. Which command is used to search for physical volumes for use with LVM?

    1. `lvmcreate`
    2. `pvcreate`
    3. `lvmdiskscan`
    4. `lvmscan`

    Answer:

    C.  The `lvmdiskscan` command looks for physical volumes that have been initialized for use with LVM.
28. Which configuration option within a systemd timer unit file causes the program to execute a certain number of seconds or minutes after the system has booted?

    1. `OnBootSec`
    2. `StartupCommand`
    3. `StartCmdSec`
    4. `CmdSec`

    Answer:

    A.  The `OnBootSec` option defines the time to wait, in seconds, until launching the command specified within the unit file. It is notable that `OnBootSec` is an alias for `OnStartupSec`. The other options shown are not valid.
29. You are troubleshooting an issue reported by a user and suspect it may be related to their environment variables. What command should the user run in order to view the current settings for their environment when using Bash?

    1. `environment`
    2. `env`
    3. `listenv`
    4. `echoenv`

    Answer:

    B.  The `env` command will print the current environment variables from Bash. The `printenv` command will also perform the same operation. The other commands listed in this question do not exist.
30. Which command can be used to determine the default CPU scheduling priority for a given user?

    1. `nice`
    2. `sked`
    3. `pri`
    4. `sched`

    Answer:

    A.  The `nice` command displays the scheduling priority and can also be used to set the scheduling priority for a command to be executed. The other options shown are not valid.
31. Users are reporting that various programs are crashing on the server. Examining logs, you see that certain processes are reporting out-of-memory conditions. Which command can you use to see the overall memory usage, including available swap space?

    1. `tree`
    2. `pgrep`
    3. `uptime`
    4. `free`

    Answer:

    D.  The `free` command displays overall memory usage for both RAM and swap and can be used to determine when additional memory might be needed.
32. You suspect that there is high CPU utilization on the system and need to perform further troubleshooting. Which command can be used to determine the current load average along with information on the amount of time since the last boot of the system?

    1. `uptime`
    2. `sysinfo`
    3. `bash`
    4. `ls -u`

    Answer:

    A.  The `uptime` command shows basic information such as that described along with the number of users logged into the system and the current time. The `bash` command is a shell environment, and the `ls` command will not display the required information.
33. You need to start a long-running process that requires a terminal and foreground processing. However, you cannot leave your terminal window open due to security restrictions. Which command will enable you to start the process and return at a later time to continue the session?

    1. `fg`
    2. `bg`
    3. `kill`
    4. `screen`

    Answer:

    D.  The `screen` command starts a new terminal that can be disconnected and reconnected as needed. Processes running from within the `screen` session do not know that they are running in a `screen` session and therefore meet the criteria needed to satisfy this question. The `fg` and `bg` commands will not meet the criteria, and the `kill` command will stop a process.
34. You are troubleshooting an NFS filesystem that will not unmount. Which option within the mount point's systemd mount file can be used to force the mount point to be unmounted?

    1. `NFSUmount=`
    2. `Timeout=`
    3. `Options=`
    4. `ForceUnmount=`

    Answer:

    D.  The `ForceUnmount=` option is equivalent to passing the `-f` option to `umount` and forces the filesystem to be unmounted. The `Options=` directive is valid but not for this purpose. The other options shown are not valid.
35. You have backgrounded several tasks using `&`. Which command can be used to view the current list of running tasks that have been backgrounded?

    1. `procs`
    2. `plist`
    3. `jobs`
    4. `free`

    Answer:

    C.  The `jobs` built-in command shows the list of jobs running in the background. Its output includes both a job number and the status of the job.
36. You suspect there is a runaway process on the server. Which command can be used to kill any process by using its name?

    1. `killproc`
    2. `killname`
    3. `killall`
    4. `kill -f`

    Answer:

    C.  The `killall` command is used to terminate processes using their name.
37. You are using `top` to investigate a report of the system processing being slow. A developer reports that that the `id` column within `%Cpu(s)` output of `top` is reporting as 98.3 and they would like to know which PID is associated with that much CPU. What should you tell them?

    1. The `id` column represents the average delay for a process.
    2. The `id` column is CPU time related to user processes.
    3. The process ID will need to be found with the `ps` command to determine which PID corresponds to the `id` output.
    4. The number that corresponds to `id` represents idle time of the CPU and not the time used by a process ID.

    Answer:

    D.  The `id` output represents CPU idle time and therefore is telling for this scenario insofar as further investigation will be needed to determine the cause of reported slowdowns on the system. The `id` output is not associated with a process or user ID, and user processes are represented by `us` in the output of `top`.
38. When an `fsck` is running on an ext3 filesystem, the process is taking longer than expected and requiring input from the administrator to fix issues. What option could be added to `fsck` next time so that the command will automatically attempt to fix errors without intervention?

    1. `-o`
    2. `-V`
    3. `-y`
    4. `-f`

    Answer:

    C.  The `-y` option will attempt to repair automatically, essentially answering `y` or `yes` instead of prompting. Of the other options, only `-V` is valid and will produce verbose output.
39. You are using a storage area network (SAN) that keeps causing errors on your Linux system due to an improper kernel module created by the SAN vendor. When the SAN sends updates, it causes the filesystem to be mounted as read-only. Which command and option can you use to change the behavior of the filesystem to account for the SAN bug?

    1. `mount --continue`
    2. `tune2fs -e continue`
    3. `mkfs --no-remount`
    4. `mount -o remount`

    Answer:

    B.  The `tune2fs` command can be used for this purpose but should be used with care because it can result in data corruption.
40. Which command is used to format a swap partition?

    1. `fdisk`
    2. `mkswap`
    3. `formatswap`
    4. `format -s`

    Answer:

    B.  The `mkswap` command formats a swap partition. The `fdisk` command is used to create the partition but not format it. The other two options do not exist.
41. The system is running out of disk space within the home directory partition, and quotas have not been enabled. Which command can you use to determine the directories that might contain large files?

    1. `du`
    2. `df`
    3. `ls`
    4. `locate`

    Answer:

    A.  The `du` command will report on disk usage in a recursive manner, unlike the other commands shown here.
42. Which option is set on a filesystem in order to enable user-level quotas?

    1. `quotaon`
    2. `enquota=user`
    3. `usrquota`
    4. `userquota`

    Answer:

    C.  The `usrquota` option will enable user-level quotas on the given mount point. This is typically set within `/etc/fstab`.
43. Which option to `quotacheck` is used to create the files for the first time?

    1. `-f`
    2. `-u`
    3. `-m`
    4. `-c`

    Answer:

    D.  The `-c` option creates the files for the first time. The `-f` option is used for force checking, `-u` is used for user quotas, and `-m` is used to not attempt remounting read-only.
44. While troubleshooting a file permission issue, you wrote a Bash script containing an `if` conditional. Which of the following tests will determine whether a file exists and can be read by the user executing the test?

    1. `-e`
    2. `-s`
    3. `-a`
    4. `-r`

    Answer:

    D.  The `-r` test determines whether a given file exists and can be read by the current user. The `-e` test only checks to see if the file exists, while `-s` determines if the file exists and has a size greater than zero. There is no `-a` file test.
45. Which start-up type is the default for systemd services if no `Type=` or `BusName=` options are specified?

    1. `oneshot`
    2. `exec`
    3. `simple`
    4. `none`

    Answer:

    C.  The default type is `simple` if no other `Type=` or `BusName=` specification is found within the unit file. Of the other options, both `exec` and `oneshot` are valid but not for the scenario described.
46. Which command can be used as a means to elevate privileges to run a command as root?

    1. `asroot`
    2. `elev`
    3. `sudo`
    4. `runroot`

    Answer:

    C.  The `sudo` command can be used to execute a process as root. The other commands shown are not valid.
47. To which shell can a user account be set if they are not allowed to log in interactively to the computer?

    1. `/bin/bash`
    2. `/bin/tcsh`
    3. `/bin/zsh`
    4. `/bin/false`

    Answer:

    D.  Setting a user's shell to `/bin/false` will prevent them from logging in interactively to the system, such as with SSH. The other options shown for this question are all valid shells and would allow an interactive login.
48. When troubleshooting disk usage, which of the following commands is used to determine the amount of disk space used by systemd journal log files?

    1. `journalctl --disk`
    2. `journalctl -du`
    3. `journalctl --disk-usage`
    4. `journalctl -ls`

    Answer:

    C.  The `journalctl` command is used for this purpose, and the `--disk-usage` option displays the disk space used by journal log files, which are typically stored in `/var/log/journal`.
49. Which command can be used to determine the current time-zone setting while troubleshooting a time-zone configuration issue?

    1. `timedatectl status`
    2. `timedate --gettz`
    3. `tzdata --list`
    4. `timezone --show`

    Answer:

    A.  The command `timedatectl status` shows the current time zone along with other information about time and date on the device. The other commands shown are not valid for this purpose.
50. Which of the following is not used as a private address for internal, non-Internet use?

    1. 172.16.4.2
    2. 192.168.40.3
    3. 10.74.5.244
    4. 143.236.32.231

    Answer:

    D.  Private IP addresses are found within the 10.0.0.0/8, 172.16.0.0/12, and 192.168.0.0/16 ranges, thus making an address in the 143 range a public IP.
51. Which of the following commands adds a default gateway of 192.168.1.1 for interface `eth0`?

    1. `route add default gateway 192.168.1.1 eth0`
    2. `eth0 --dg 192.168.1.1`
    3. `route add default gw 192.168.1.1 eth0`
    4. `route define eth0 192.168.1.1`

    Answer:

    C.  The `route` command is used for this purpose, and adding a route is done with the `add` option. The default gateway is added using the `default gw` keywords followed by the IP of the gateway and the adapter.
52. Which option for the `host` command will query for the authoritative nameservers for a given domain?

    1. `-t ns`
    2. `-t all`
    3. `-n`s
    4. `-named`

    Answer:

    A.  The `host` command enables changing of the query type with the `-t` option. Using `ns` as the type will query for the nameservers for a given domain. There is no `all` type, and the other options are also invalid.
53. Which option for the `ping` command enables you to choose the interface from which the ICMP packets will be generated?

    1. `-i`
    2. `-I`
    3. `-t`
    4. `-a`

    Answer:

    B.  The `-I` option enables the choice of interface. A lowercase `-i` option sets the interval, while `-a` indicates an audible ping. Finally, `-t` enables a TTL-based `ping` only.
54. Which of the following commands queries for the mail servers for the domain [`example.com`](http://example.com/)?

    1. `dig` [`example.com`](http://example.com/) `mx`
    2. `dig` [`example.com`](http://example.com/)
    3. `host -t smtp` [`example.com`](http://example.com/)
    4. `dig` [`example.com`](http://example.com/) `smtp`

    Answer:

    A.  The `host` or `dig` command can be used for this purpose by setting the type to `mx`. The `mx` type will query for the mail exchanger for the given domain. There is no `smtp` type.
55. You need to test SSL connectivity to a web server at `www.example.com`. Which of the following commands accomplishes this task?

    1. `rd` `www.example.com` `-L`
    2. `curSSH` `https://www.example.com`
    3. `openssl` `https://www.example.com:443`
    4. `openssl s_client -connect` `www.example.com:443`

    Answer:

    D.  The `openssl s_client -connect` `www.example.com:443` command accomplishes the task described. The other commands shown are not valid.
56. Which command can be used to listen for netlink messages on a network?

    1. `ip monitor`
    2. `netlink -a`
    3. `ip netlink`
    4. `route`

    Answer:

    A.  The `ip` command with the `monitor` option/subcommand will display netlink messages as they arrive. There is no `netlink` subcommand for `ip`, and the `route` command will not work for this purpose.
57. Which of the following `dig` commands sends the query for [`example.com`](http://example.com/) directly to the server at 192.168.2.5 rather than to a locally configured resolver?

    1. `dig` [`example.com`](http://example.com/) `@192.168.2.5`
    2. `dig -t 192.168.2.5` [`example.com`](http://example.com/)
    3. `dig -s 192.168.2.5` [`example.com`](http://example.com/)
    4. `dig server=192.168.2.5` [`example.com`](http://example.com/)

    Answer:

    A.  The `@` symbol is used to indicate a server to which the query will be sent directly. This can be quite useful for troubleshooting resolution problems by sending the query directly to an authoritative name server for the domain. Of the other options, `-t` sets the type, and the remaining options are not valid.
58. Which of the following commands will enumerate the `hosts` database?

    1. `getent hosts`
    2. `gethosts`
    3. `nslookup`
    4. `host`

    Answer:

    A.  The `getent` command is used for working with NSS databases, and `getent hosts` will display the available hosts using the databases configured in `/etc/nsswitch.conf`.
59. Which of the following configuration lines will set the DNS server to 192.168.1.4 using `/etc/resolv.conf`?

    1. `dns 192.168.1.4`
    2. `dns-server 192.168.1.4`
    3. `nameserver 192.168.1.4`
    4. `name-server 192.168.1.4`

    Answer:

    C.  The configuration option is called `nameserver`, and the value for the option is the IP address of the desired nameserver. There are several options that affect how name resolution is performed, such as the number of attempts and timeout. See `resolv.conf(5)` for more information.
60. Which of the following commands adds a route to the server for the network 192.168.51.0/24 through its gateway of 192.168.51.1?

    1. `route add -net 192.168.51.0 netmask 255.255.255.0 gw 192.168.51.1`
    2. `route add -net 192.168.51/24 gw 192.168.1.51`
    3. `route -net 192.168.51.0/24 192.168.51.1`
    4. `route add 192.168.51.1 -n 192.168.51.0//255.255.255.0`

    Answer:

    A.  The `route` command can be used for this purpose; the syntax includes the network range, denoted with the `-net` option, followed by the word `netmask` and the masked bits, followed by the word `gw` and the IP of the gateway. The other options shown are invalid for a variety of reasons, including missing keywords and options and order.
61. Which of the following commands shows network services or sockets that are currently listening along with sockets that are not listening?

    1. `netstat -a`
    2. `netlink -a`
    3. `sockets -f`
    4. `opensock -l`

    Answer:

    A.  The `netstat` command is used for this purpose, and the `-a` option displays all sockets, listening and non-listening. Note that it's frequently helpful to add the `-n` option, or combine them as in `netstat –an`, in order to prevent name lookup. Doing so can significantly improve performance of the command.
62. Which of the following represents a correct configuration line for `/etc/hosts`?

    1. `192.168.1.4` `cwa.braingia.org` `cwa`
    2. `cwa.braingia.org` `cwa 192.168.1.4`
    3. `cwa.braingia.org` `192.168.1.8 alias cwa`
    4. `alias` `cwa.braingia.org` `cwa 192.168.1.4`

    Answer:

    A.  The correct format is IP address followed by canonical hostname and any aliases for the host. You can use entries in `/etc/hosts` to override DNS lookups, which can be useful to prevent those names from resolving or to provide a different resolution.
63. Which command can be used to determine how much time a Linux command takes?

    1. `time`
    2. `cmdtime`
    3. `timeproc`
    4. `proctime`

    Answer:

    A.  The `time` command includes timing information such as sys time, user time, and real time. The other commands are not valid.
64. Which of the following commands will change the default gateway to 192.168.1.1 using `eth0`?

    1. `ip route default gw 192.168.1.1`
    2. `ip route change default via 192.168.1.1 dev eth0`
    3. `ip route default gw update 192.168.1.1`
    4. `ip route update default 192.168.1.1 eth0`

    Answer:

    B.  The `ip route` command can be used for this purpose, and its syntax uses a `change` command and the `via` keyword. The same operation could be completed with the `route` command but would require deleting the existing gateway first and then re-adding a new default gateway.
65. Which option to `dumpe2fs` displays the bad blocks for a given partition?

    1. `-bb`
    2. `-C`
    3. `-b`
    4. `-f`

    Answer:

    C.  Bad blocks are shown with the `-b` option. The `-f` option forces `dumpe2fs` to perform the requested operation, and the other command options do not exist.
66. Which option to `xfs_check` is used to verify a filesystem that is stored in a file?

    1. `-v`
    2. `-a`
    3. `-f`
    4. `-d`

    Answer:

    C.  The `-f` option specifies that `xfs_check` should check the contents of the named file for consistency. The `-v` option sets verbosity, and there are no `-d` and `-a` options.
67. Which option within a systemd mount file specifies the filesystem to be mounted?

    1. `FSPath=`
    2. `Path=`
    3. `Where=`
    4. `What=`

    Answer:

    D.  The `What=` option specifies the filesystem to be mounted. The `Where=` option defines the destination to which the filesystem will be mounted. The other options shown are not valid.
68. Assume that you want to enable local client services to go to hosts on the network without needing to fully qualify the name by adding the domain for either [`example.com`](http://example.com/) or [`example.org`](http://example.org/). Which option in `/etc/resolv.conf` will provide this functionality?

    1. `search`
    2. `domain`
    3. `local-domain`
    4. `local-order`

    Answer:

    A.  The `search` option is used for this purpose and can be provided with multiple domain names, each separated by a space or tab. The `domain` option is valid within `/etc/resolv.conf` but does not allow for multiple domain names.
69. Which of the following commands prevents traffic from reaching the host 192.168.1.3?

    1. `route add -host 192.168.1.3 reject`
    2. `route -nullroute 192.168.1.3`
    3. `route add -null 192.168.1.3`
    4. `route add -block 192.168.1.3`

    Answer:

    A.  The `route` command can be used for this purpose, and in the scenario described, a `reject` destination is used for the route. The other options shown are invalid because they use invalid options to the `route` command.
70. Which of the following describes a primary difference between `traceroute` and `tracepath`?

    1. The `traceroute` command requires root privileges.
    2. The `tracepath` command provides the MTU for each hop, whereas `traceroute` does not.
    3. The `tracepath` command cannot be used for tracing a path on an external network.
    4. The `traceroute` command is not compatible with IPv6.

    Answer:

    B.  The `tracepath` command provides the Maximum Transmission Unit (MTU) of the hops, where possible. Both `traceroute` and `tracepath` can be used internally or externally, and both provide IPv6 capabilities. Certain options with the `traceroute` command can require root privileges, but not enough information was given in the question for that to have been the correct answer.
71. Which of the following commands will emulate the `ping` command in Microsoft Windows, where the `ping` is sent for four packets and then the command exits?

    1. `ping -n 4`
    2. `ping -t 4`
    3. `ping -p 4`
    4. `ping -c 4`

    Answer:

    D.  The `-c` option provides the count of the number of pings to send. The `-n` option specifies numeric output only, while `-p` specifies the pattern to use for the packet content. Finally, the `-t` option sets the TTL.
72. Which option to `journalctl` displays log messages as they are being logged?

    1. `--tail`
    2. `--du`
    3. `-f`
    4. `-m`

    Answer:

    C.  The `-f` follows the log much like `tail -f`. There is no `--tail` option for `journalctl`. Of the other options, `--du` dumps the catalog, and `-m` merges all available journals.
73. Which of the following commands should be executed after running `ip route change`?

    1. `ip route flush cache`
    2. `ip route reload`
    3. `ip route cache reload`
    4. `ip route restart`

    Answer:

    A.  The `ip route flush cache` command should be executed after changing the routes. The other commands shown for this question are not valid.
74. Which option should be used to send a DNS query for an SPF record with `dig`?

    1. `-t txt`
    2. `-t spf`
    3. `-t mx`
    4. `-t mailspf`

    Answer:

    A.  SPF records are stored in the `txt` record type in DNS, thereby making `-t txt` the correct option for this. Of the other answers, only `-t mx` is valid and returns the mail exchangers for the given domain.
75. When troubleshooting a connectivity issue, you have found that you can reach a server via the Web but cannot ping it and suspect that there are dropped packets. Which of the following best describes a possible cause for this scenario?

    1. TCP traffic has been blocked at the firewall.
    2. The DNS lookup is failing.
    3. ICMP traffic has been blocked.
    4. There is a reject route in place.

    Answer:

    C.  The only viable possibility of those listed is that ICMP traffic is blocked. TCP traffic is obviously passing because of the ability to get there using HTTP, and DNS must also be working.
76. When you're viewing the available routes using the `route` command, one route contains the flags `UG` and the others contain `U`. What does the letter `G` signify in the route table?

    1. The `G` signifies that the route is good.
    2. The `G` signifies that the route is unavailable.
    3. The `G` signifies that this is a gateway.
    4. The `G` signifies that the route is an aggregate.

    Answer:

    C.  The `G` signifies a gateway within the route table.
77. Which of the following commands requests a zone transfer of [`example.org`](http://example.org/) from the server at 192.168.1.4?

    1. `dig` [`example.org`](http://example.org/) `@192.168.1.4 axfr`
    2. `dig` [`example.org`](http://example.org/) `@192.168.1.4`
    3. `dig` [`example.org`](http://example.org/) `@192.168.1.4 xfer`
    4. `dig` [`example.org`](http://example.org/) `#192.168.1.4 xfer`

    Answer:

    A.  The `axfr` type is a zone transfer, and the `@` symbol signifies the server to which the query will be sent. There is no `xfer` type. Option B is just a normal query for the domain sent to the specified server.
78. You are troubleshooting a disk space issue and notice that the journal files are consuming too much space. Which option within journald.conf sets a limit on how much disk space can be used?

    1. `MaxDisk=`
    2. `SystemMaxUse=`
    3. `MaxSpace=`
    4. `SpaceLimit=`

    Answer:

    B.  The `SystemMaxUse=` option controls the amount of space that the journal can use. The other options shown are not valid.
79. Although no dependencies may appear in a unit file, a service with a `Type=dbus` depends on which service?

    1. `dbus.socket`
    2. `dbus.run`
    3. `dbus.dep`
    4. `dbus.svc`

    Answer:

    A.  A `Type=dbus` for a service file has implicit dependencies of `Requires=` and `After=` on `dbus.socket`. The other options are not valid.
80. Which of the following commands scans the IP address 192.168.1.154 for open ports?

    1. `nmap 192.168.1.154`
    2. `lsof 192.168.1.154`
    3. `netstat 192.168.1.154`
    4. `netmap 192.168.1.154`

    Answer:

    A.  The `nmap` command is used to scan for open ports. It will scan for open TCP ports to the address or addresses specified. The other commands shown do not scan for open ports to external (off-host) IP addresses.
81. You are troubleshooting an NFS filesystem that will not mount. Which option within the mount point's systemd mount file is used to specify the type of filesystem being mounted?

    1. `FSType=`
    2. `Type=`
    3. `App=`
    4. `MountType=`

    Answer:

    B.  The `Type=` option is used to specify the type of filesystem that will be mounted. It is similar to the types used with the `mount` command itself. The other options shown are not valid.
82. What is the file extension used with systemd unit files that provide time-based control of services?

    1. `.svc`
    2. `.cron`
    3. `.sked`
    4. `.timer`

    Answer:

    D.  The `.timer` file extension is used with systemd timer files that provide an alternative to `cron`. The other options are not valid.
83. You are using `nmap` to scan a host for open ports. However, the server is blocking ICMP echo requests. Which option to `nmap` can you set in order to continue the scan?

    1. `-P0`
    2. `-no-ping`
    3. `-s0`
    4. `-ping-0`

    Answer:

    A.  Setting `-P0` will cause no ping requests to precede the scan and is useful for the scenario described. There is a `-s` option, but it is not used for this purpose. The other options are not valid.
84. Which option within `/etc/security/limits.conf` is used to control the number of times a given account can log in simultaneously?

    1. `nlogins`
    2. `loginmax`
    3. `maxlogins`
    4. `loginlimit`

    Answer:

    C.  The `maxlogins` parameter is used to control the number of simultaneous logins for a given account.
85. Which option to `nmap` sets the scan to use TCP SYN packets for finding open ports?

    1. `-sS`
    2. `-sT`
    3. `-sY`
    4. `-type SYN`

    Answer:

    A.  The `-s` option sets the type of scan and, when followed by an uppercase `S`, sets the option to `SYN`. The `T` option is a `Connect()` scan. There is no `Y` option or `-type` option for `nmap`.
86. Which option to `tune2fs` enables the specification of various journal options such as specifying the location of the journal itself?

    1. `-a`
    2. `-J`
    3. `-x`
    4. `-A`

    Answer:

    B.  The `-J` option enables specification of various settings for the journal such as its location. The other options shown are not valid.
87. You are troubleshooting high latency and low throughput with a disk and using `iostat` to assess performance. Which option to `iostat` displays information on a per-partition basis for block devices?

    1. `-a`
    2. `-c`
    3. `-d`
    4. `-p`

    Answer:

    D.  The `-p` option to `iostat` displays information on devices and partitions. The `-c` option shows CPU utilization, and `-d` shows device utilization and can be used to display Input/Output Per Second (IOPS) information. There is no `-a` option.
88. Which of the following commands displays blocks in and blocks out as related to I/O?

    1. `iorpt`
    2. `iptraf`
    3. `vmswap`
    4. `vmstat`

    Answer:

    D.  The `vmstat` command is used to display extended information about performance, including blocks in and out. The `iptraf` command is used to provide network-level monitoring, and the other two commands listed are not valid.
89. Which of the following commands can be used to display a list of currently logged-in users along with the current load average and time since last reboot?

    1. `uptime`
    2. `w`
    3. `swap`
    4. `sysinfo`

    Answer:

    B.  The `w` command shows various useful information that includes load average, logged-in users, and other uptime information. The `uptime` command does not show who is currently logged in. There is no `swap` or `sysinfo` command.
90. You need to examine the hardware to determine the amount of memory on the system and the block size. Which command can be used for this purpose?

    1. `free`
    2. `memstat`
    3. `lsmem`
    4. `memx`

    Answer:

    C.  The `lsmem` command shows statistics about the memory in the system, including block size. Among the other options, `free` shows in-use memory information but not block size. The other options are not valid commands.
91. While troubleshooting high latency, you need to collect data on throughput. Which of the following monitoring tools can use SNMP and scripts to collect data for performance-related graphing such as throughput and bandwidth?

    1. `ptop`
    2. `pstree`
    3. Cacti
    4. Grafr

    Answer:

    C.  Cacti is a graphing tool that uses scripts for gathering performance data as well as SNMP. The graphs can help to visualize performance of networks and systems alike. The `pstree` command is used to show a tree-like structure of processes.
92. Which `swapon` option silently skips those swap partitions that do not exist?

    1. `-u`
    2. `-e`
    3. `-i`
    4. `-o`

    Answer:

    B.  The `-e` option causes `swapon` to skip those partitions that do not exist. The other options are not valid for this scenario.
93. Which of the following abbreviations is used to signify system time CPU percentage in the output of the `top` command?

    1. `sys`
    2. `us`
    3. `sy`
    4. `system%`

    Answer:

    C.  The `sy` abbreviation in the output of `top` represents the percentage of CPU time used by the system. Of the other options, `us` represents user CPU time. Options A and D are not valid for this scenario.
94. Which of the following commands deactivates swap space?

    1. `swapoff`
    2. `swap -off`
    3. `unmountswap`
    4. `uswap`

    Answer:

    A.  The `swapoff` command deactivates swap space, thereby making it unavailable as virtual memory on the system. The other commands shown as options are not valid.
95. Which of the following `swapon` options displays information on the size of swap space along with its used space?

    1. `--list`
    2. `-a`
    3. `--show`
    4. `-h`

    Answer:

    C.  The `--show` option displays information about the swap spaces on the computer, including how much swap is currently being used. The `-a` option activates all swap spaces. There is no `--list` option, and `-h` displays help.
96. Which of the following commands displays information about a given physical volume in an LVM setup?

    1. `pvdisp`
    2. `pvlist`
    3. `pvdisplay`
    4. `pvl`

    Answer:

    C.  The `pvdisplay` command shows information about a given physical volume. You can use `pvdisplay` to view the device on which the PV is built along with the extent size of the PV. The other commands shown are not valid.
97. Which of the following commands looks for LVM physical volumes and volume groups involved in an LVM configuration?

    1. `vgscan`
    2. `lvmscan`
    3. `lvlist`
    4. `pvlist`

    Answer:

    A.  The `vgscan` command looks for both physical volumes and volume groups related to an LVM configuration. The `vgscan` command is run at system startup but can also be run manually. The other commands are not valid.
98. Which of the following commands is used to display a list of physical volumes involved in LVM?

    1. `pvdisp`
    2. `pvlist`
    3. `pvscan`
    4. `pvmm`

    Answer:

    C.  The `pvscan` command displays a list of physical volumes on a given server. The PVs displayed are those that have been initialized with `pvcreate` for use with LVM.
99. While troubleshooting interface errors, you need to examine the protocol family supported by an interface. When you're using the `ip` command, which protocol family is used as the default if not otherwise specified?

    1. `tcpip`
    2. `ip`
    3. `inet`
    4. `arp`

    Answer:

    C.  The `ip` command defaults to the `inet` family if not otherwise specified with the `-f` option. The command will attempt to guess the correct family and fall back to `inet`. The other families listed as options for this command are not valid for use with the `ip` command.
100.    You are using the `route` command to view routes. However, name resolution is taking a long time and causing delay in the response from the `route` command. Which option to `route` can be added to cause it to not perform name resolution?

        1. `-d`
        2. `-e`
        3. `-f`
        4. `-n`

        Answer:

        D.  The `-n` option causes `route` to use numeric values only, performing no name resolution. This option is useful for the scenario described. The `-e` option causes the output to be in `netstat` format. There is no `-d` or `-f` option for the `route` command.
101.    You have replaced a device on the network but used the IP address from another active device. Which command can be run to remove the MAC address entry from your computer so that it performs the address resolution again?

        1. `arp -d`
        2. `netstat -rn`
        3. `hostname`
        4. `dig`

        Answer:

        A.  Because you're working with MAC addresses, the `arp` command will be used. The `-d` option removes or deletes an ARP entry, which would be appropriate here so that the MAC address resolution occurs again. The `netstat` command will not be used for this purpose. The `hostname` and `dig` commands work with name resolution but not for MAC addresses or the ARP table.
102.    When looking to parse the output of the `ip` command, which option can be set to remove newlines such that the output could be piped to the `grep` command?

        1. `-n`
        2. `-o`
        3. `-l`
        4. `-f`

        Answer:

        B.  The `-o` option removes newlines from the output, thereby making the output more suitable for the `grep` command. The `-l` option specifies the number of loops for the `ip addr flush` command. The `-f` option specifies the protocol family. There is no `-n` option.
103.    Which option to the `arp` command creates a new entry for a given IP address to MAC address pair?

        1. `-s`
        2. `-c`
        3. `-d`
        4. `--add`

        Answer:

        A.  The `-s` option creates an ARP table entry. The `-d` option removes an entry. The `-c` and `--add` options do not exist.
104.    Which option to `tcpdump` displays a list of available interfaces on which `tcpdump` can operate?

        1. `-a`
        2. `-d`
        3. `-D`
        4. `-i`

        Answer:

        C.  The `-D` option lists the interfaces on a given computer. The `-d` option dumps compiled matching code, and `-i` selects an interface. There is no `-a` option.
105.    Which option to `nmap` will cause it to always perform name resolution?

        1. `-n`
        2. `-R`
        3. `-b`
        4. `-a`

        Answer:

        B.  The `-R` option requires that an attempt at name resolution be performed. The `-n` option does the opposite: it disables name resolution. There is no `-b` or `-a` option.
106.    Which of the following commands provides a live `traceroute` of the route between two hosts, updating the information for each hop in near real time?

        1. `traceroute --live`
        2. `mtr`
        3. `route -update`
        4. `liveroute`

        Answer:

        B.  The `mtr` command provides a unique way to view real-time information about each hop in a route between hosts. Both the `traceroute` and `route` commands are valid, but the options shown for each are not. There is no `liveroute` command.
107.    You are using a local RAID array and investigating a performance issue. When using `mdadm` in monitor mode, which option sets the polling interval?

        1. `--delay`
        2. `--internal`
        3. `--interval`
        4. `--poll`

        Answer:

        A.  The `--delay` option sets the interval between checks of array health. The argument value is in seconds. The other options shown are not valid.
108.    When viewing the results of a `traceroute`, you see `!H`. To what does `!H` refer?

        1. Network unreachable
        2. Host available
        3. Host unreachable
        4. High length

        Answer:

        C.  The `!H` sequence indicates host unreachable. Network unreachable is `!N`.
109.    Assuming that policy routing has been enabled in the kernel, which option to the `ping` command can be used to mark the outgoing request appropriately in order to indicate that the packet should be processed according to a particular policy?

        1. `-m`
        2. `-a`
        3. `-p`
        4. `-k`

        Answer:

        A.  The `-m` option specifies how the packet should be marked or tagged. The `-a` option is an audible ping, and `-p` enables specification of custom padding. There is no `-k` option.
110.    When you're troubleshooting a possible issue with bad blocks on a disk, which option to `fsck` will report statistics such as CPU time used on completion of the `fsck` operation?

        1. `-s`
        2. `-r`
        3. `-l`
        4. `-f`

        Answer:

        B.  The `-r` option displays a report that includes CPU time and exit status about the just-completed `fsck` operation. The `-f` option forces whatever operation is being requested, `-s` serializes `fsck` operations, and `-l` creates an exclusive flock.
111.    Which of the following files provides information on memory utilization, including free memory, buffers, cache usage, and several additional items?

        1. `/proc/cpuinfo`
        2. `/proc/memtime`
        3. `/proc/memuse`
        4. `/proc/meminfo`

        Answer:

        D.  The file `/proc/meminfo` provides a wealth of information about memory usage and utilization. Much of this information is displayed by various commands, but the canonical source for those commands is usually found in this file. Of the other options, only `/proc/cpuinfo` is valid, and that file provides information on the CPU(s) for the computer.
112.    Which scan mode for `nmap` provides an Xmas scan?

        1. `-sT`
        2. `-sS`
        3. `-sP`
        4. `-sX`

        Answer:

        D.  An Xmas scan is available using the `-sX` mode of `nmap`. The `-sT` mode is a TCP connect, and `-sS` is TCP SYN. There is no `-sP` option.
113.    Which option to `tcpdump` sets the snapshot length of packets to capture?

        1. `-s`
        2. `-l`
        3. `-d`
        4. `-c`

        Answer:

        A.  The `-s` option sets the snapshot length, or snaplen, of the capture instead of its default of 65,535 bytes. The `-l` option provides line buffering, `-c` stops after the indicated count of packets are received, and `-d` dumps compiled packet-matching code into a format that is readable.
114.    On which port does the `ping` command operate for ICMP echo requests?

        1. 53
        2. 1337
        3. 33433
        4. No port

        Answer:

        D.  There is no port for ICMP. The protocol does not use ports.
115.    When running the `df` command, you need to change the scale such that the report shows terabytes instead of bytes. Which option will accomplish this task?

        1. `-ST`
        2. `-BT`
        3. `-j`
        4. `-T`

        Answer:

        B.  The `-B` option changes the format, and `T` sets the scale to terabytes. The other options do not exist.
116.    Which option to `mke2fs` is used to check for bad blocks during filesystem creation?

        1. `-a`
        2. `-b`
        3. `-c`
        4. `-d`

        Answer:

        C.  The `-c` option checks for bad blocks. The `-b` option sets the block size. There is no `-a` or `-d` option.
117.    Which option to the `ping` command shows latency rather than round-trip time?

        1. `-L`
        2. `-i`
        3. `-U`
        4. `-d`

        Answer:

        C.  The `-U` option shows latency. Of the other options, `-d` is used for debugging, `-L` suppresses multicast loopback packets, and `-i` sets the interval between packets.
118.    You suspect that bandwidth limitations may be preventing large files from transferring in a timely manner. Which of the following commands is used to measure network throughput?

        1. `tp`
        2. `iperf`
        3. `ith`
        4. `ithrough`

        Answer:

        B.  The `iperf` command can be used to measure throughput and can be used for troubleshooting latency issues. The other options are not valid commands.
119.    You would like to monitor interrupt usage in real time on a Linux server in order to troubleshoot communication ports usage. Which of the following commands can be used for this purpose?

        1. `int`
        2. `moni`
        3. `itop`
        4. `imon`

        Answer:

        C.  The `itop` command displays information about interrupt usage in real time, with a display that is somewhat like the `top` command. The other options shown for this question are not valid commands.
120.    You are configuring an RDMA interface. Which of the following commands displays information about InfiniBand devices?

        1. `ibmon`
        2. `ibstat`
        3. `rdmon`
        4. `rdstat`

        Answer:

        B.  The `ibstat` command shows information about InfiniBand devices. The other commands are not valid.
121.    You need to increase the performance of process ID 4382 by changing its priority. Which of the following commands will accomplish this task?

        1. `renice -5 -p 4382`
        2. `renice 5 -p 4382`
        3. `renice 100 4382`
        4. `renice 4382 +5`

        Answer:

        A.  The `renice` command is used to change priorities. The lower the number, the higher the priority. The correct syntax is shown in option A. Option B will set the priority lower. Options C and D are invalid syntax.
122.    Which option to `netstat` is used to disable DNS or hostname lookups?

        1. `-b`
        2. `-h`
        3. `-q`
        4. `-n`

        Answer:

        D.  The `-n` option is used with `netstat` to prevent hostname lookups, which can slow the output. The other options do not perform the required task.
123.    You would like to find all of the process IDs associated with the `sshd` process on an Ubuntu system. Which of the following commands accomplishes this task?

        1. `ps -sshd`
        2. `pidof sshd`
        3. `pids sshd`
        4. `ps --a=sshd`

        Answer:

        B.  The `pidof` command shows all of the processes associated with the given argument. In this case, option B shows the correct syntax. The `ps` command shown in other options is a valid command but not with the syntax shown.
124.    Which kill signal sends a hangup to a given process?

        1. 1
        2. 5
        3. 24
        4. 30

        Answer:

        A.  The number 1, or `SIGHUP`, is the signal that sends a hangup to the process. The other options shown are valid signals but not for the purpose described.
125.    Which of the following commands displays the current target runlevel on a systemd system?

        1. `ls -l /etc/systemd/system/default.target`
        2. `systemctl default-target`
        3. `systemd default-target`
        4. `ls -l /etc/systemd/system-default.target`

        Answer:

        A.  The command `ls -l /etc/systemd/system/default.target` shows the current target to which the system will boot. The other commands are not valid.
126.    You would like to change the byte-to-inode ratio on a new filesystem in order to prevent inode exhaustion. Which option to `mke2fs` accomplishes this task?

        1. `-b`
        2. `-r`
        3. `-i`
        4. `-u`

        Answer:

        C.  The `-i` option sets the byte-to-inode ratio. The `-b` option sets the block size, `-r` sets the filesystem revision, and there is no `-u` option for `mke2fs`.
127.    Which directory contains information on FibreChannel HBA ports?

        1. `/sys/fc/ports`
        2. `/sys/class/hba`
        3. `/sys/class/fc_host`
        4. `/sys/class/fc/ports`

        Answer:

        C.  The `/sys/class/fc_host` directory contains information on HBA adapter ports on the system. The other options are not valid directories.
128.    Which type of module interface for PAM is used to set a policy such as the time of day that a user can log in?

        1. `auth`
        2. `account`
        3. `password`
        4. `policy`

        Answer:

        B.  The `account` module interface is where access verification occurs. Among the other options, the `auth` and `password` interfaces are used for different purposes, and there is no `policy` interface.
129.    You need to create a restrictive access control list (ACL) on a server. Which policy should be the default for the `INPUT` chain within the firewall?

        1. `deny`
        2. `permit`
        3. `accept`
        4. `discard`

        Answer:

        A.  The default policy should be `deny`. A deny-by-default policy discards packets. It's notable that a `reject` policy might also be used, which would send a reject back to the sender. The other options are not appropriate for the task described.
130.    Which option to the `ls` command displays the ownership attributes, including user and group owners of a given file or directory?

        1. `-o`
        2. `-a`
        3. `-l`
        4. `-d`

        Answer:

        C.  The `-l` option displays ownership information, including user and group owners of a file or directory. The `-o` option only shows the user but does not display the group. The other options shown are not valid for this purpose.
131.    When creating a daemon process that will be used on the local server, which of the following communication methods should be used?

        1. Localhost/network
        2. Socket
        3. Message-passing
        4. RDP

        Answer:

        B.  The program should be created to use local sockets for communication. Socket-based programs do not need to incorporate network or protocol information, thus making them preferred over a network-based program for the purpose described. If the program needed network connectivity, then option A would be appropriate. The other options are not appropriate for this scenario.
132.    When using the `free` command to determine memory usage, which column shows the memory used by the kernel for things like kernel buffers?

        1. `used`
        2. `shared`
        3. `buffers`
        4. `cache`

        Answer:

        C.  The `buffers` column shows the amount of RAM allocated to kernel buffers. `Cache` indicates page cache usage, and `shared` usually indicates `tmpfs` usage.
133.    Which of the following commands provides a command-line interface into Network Manager?

        1. `nmc`
        2. `dmc`
        3. `nmcli`
        4. `netman`

        Answer:

        C.  The `nmcli` command provides a command-line interface into Network Manager. The other options shown are not valid commands.
134.    Which command displays network usage in a `top`-like interface?

        1. `iftop`
        2. `iptop`
        3. `ptop`
        4. `netcap`

        Answer:

        A.  The `iftop` command is used to display real-time network usage through an interface that is reminiscent of the `top` command. The other options given are not valid commands.
135.    You suspect saturation is affecting network performance with your Linux server. Which command can be used to help determine the amount of traffic being passed through a given interface?

        1. `netp`
        2. `sat`
        3. `iptraf`
        4. `ipsat`

        Answer:

        C.  The `iptraf` command shows cumulative network usage in real time for a given interface. The other options shown are not valid.
136.    You are looking to optimize the I/O scheduler for your Linux server. Which I/O scheduling algorithm is the default?

        1. `deadline`
        2. `noop`
        3. `cfq`
        4. `iqueue`

        Answer:

        C.  The `cfq` scheduler is the default for Linux systems. Of the other options shown, `deadline` and `noop` are valid but are not the default. There is no `iqueue` IO scheduler.
137.    You would like to efficiently manage firewall rules such that you can define a group of IP addresses to which a single rule can be applied. Which command enables you to create a group of IP addresses?

        1. `ipgroup`
        2. `iptables -group`
        3. `addrgroup`
        4. `ipset`

        Answer:

        D.  The `ipset` command can be used for the purpose described. It's worth noting that you could create a separate `iptables` rule for each IP address and rule, but doing so would be less efficient than using an `ipset` group and having a single rule applied to that group.
138.    You are receiving reports of timeouts from users attempting to SSH between servers. Which command should be used to help troubleshoot these reports?

        1. `tcptraceroute`
        2. `ping`
        3. `telnet`
        4. `ps`

        Answer:

        A.  The `tcptraceroute` command should be used for this purpose. This command attempts to connect to the destination on the TCP port specified. This method is preferred over a simple ping because ICMP may be filtered, thus giving an inaccurate diagnosis. The other commands would not be used for this purpose.
139.    Which command can be used to capture network traffic in `pcap` format for later analysis by a tool like Wireshark?

        1. `tcpcap`
        2. `pdump`
        3. `tshark`
        4. `pcapr`

        Answer:

        C.  The `tshark` command enables capture of network traffic into a file. The other commands shown are not valid.
140.    You need to determine the owner of an IP address. You have attempted to use `nslookup` to determine the hostname, but there was no PTR record for the IP. Which command can be used to determine who owns the IP address?

        1. `iplookup`
        2. `ipowner`
        3. `whois`
        4. `bg`

        Answer:

        C.  The `whois` command is used for lookups of domains and IP addresses, among other things, and would be used for this purpose. The other commands are not valid for this purpose.
141.    Which command can be used to help diagnose latency issues with a disk?

        1. `diskstat`
        2. `statd`
        3. `fdisk`
        4. `ioping`

        Answer:

        D.  The `ioping` command sends requests to a given disk and records the time taken for the request. Of the other commands, `fdisk` is valid but would not be used to determine performance-related issues. The other commands are not valid.
142.    Which command can be used to trigger the kernel to update the partition table?

        1. `ifdisk`
        2. `partup`
        3. `partprobe`
        4. `uppart`

        Answer:

        C.  The `partprobe` command causes a partition update for the kernel. The other options are not valid commands.
143.    Which of the following commands can be used to display historical performance data across several different parameters?

        1. `sar`
        2. `kernperf`
        3. `pkern`
        4. `perfshow`

        Answer:

        A.  The `sar` command can be used to display a wide variety of performance-related information, including that captured over time. The other commands are not valid.
144.    Which option to `sysctl` displays all of the available parameters?

        1. `-a`
        2. `-b`
        3. `-c`
        4. `-d`

        Answer:

        A.  The `-a` option shows all available parameters. The other options shown are not valid with `sysctl`.
145.    When examining output from the `state` column of the `ps` command, there is a process with a state of `D`. What state is that process currently in?

        1. Debug
        2. Interruptible sleep
        3. Uninterruptible sleep
        4. Dead

        Answer:

        C.  A state of `D` means uninterruptible sleep. There is no state for debug or dead processes, and interruptible sleep has a state of `S`.
146.    You are troubleshooting a system startup problem that prevents the system from fully booting into a graphical user interface (GUI). Which systemd target could be used to further troubleshoot the issue?

        1. Poweroff
        2. Multiuser
        3. Reboot
        4. SafeMode

        Answer:

        B.  The multiuser target is below (before) the graphical target and therefore could be used for further troubleshooting. The rescue target, not listed as an option, could also be used. The poweroff and reboot targets are valid systemd targets but will not help with troubleshooting. There is no SafeMode target.
147.    You are troubleshooting printer access on a Linux system. On which port does the CUPS printing daemon listen by default?

        1. 25
        2. 342
        3. 631
        4. 316

        Answer:

        C.  The default port is 631. The other ports listed for options are not used for CUPS.
148.    What is the required extension for systemd mount files?

        1. `.mount`
        2. `.service`
        3. `.fs`
        4. `.mountd`

        Answer:

        A.  The `.mount` extension is required for systemd mount files. Systemd frequently requires specific filenaming conventions in order to work correctly, and knowing the filenames, extensions, and special locations will be helpful for the exam.
149.    Which utility can be used to find SELinux context violations?

        1. `sestat`
        2. `secv`
        3. `convio`
        4. `ausearch`

        Answer:

        D.  The `ausearch` command can be used to find recent violations of an SELinux policy. The other commands are not valid.
150.    You have added a new RAID adapter to the system. Which command can be used to ensure that the adapter was detected by the kernel?

        1. `showraid`
        2. `lsadapt`
        3. `dmesg`
        4. `raidlist`

        Answer:

        C.  The `dmesg` command shows the kernel ring buffer and is a primary tool to determine whether the system has detected a new piece of hardware. The other options are not valid.
151.    Which option is used to send a signal to a process when using `pkill`?

        1. `-<SIGNAL>`
        2. `-s`
        3. `-i`
        4. `-h`

        Answer:

        A.  The signal number or symbolic name can be used and is prefaced with a single dash (`-`) as shown in option A. The other options are not valid for the purpose required in the question.
152.    You are troubleshooting a directory permission issue. The directory and all subdirectories are owned by root. Within the top-level directory there is another directory that has 755 permissions on it. However, a non-root user cannot obtain a directory listing of that subdirectory. Which of the following might be the issue?

        1. Directory permissions from a higher-level directory do not allow a directory listing.
        2. Directory permissions need to be 777 on the subdirectory.
        3. The write permission is needed for the subdirectory.
        4. The other permission needs to be 7 for the subdirectory.

        Answer:

        A.  Execute permissions for directories must be present, so the top-level directory must not allow the “other” permission to execute, which is needed for a directory listing within a subdirectory.
153.    What is the default request size for `ioping`?

        1. 4 bytes
        2. 4 KB
        3. 512 KB
        4. 1024 KB

        Answer:

        B.  The default size for `ioping` is 4 KB.
154.    Within which file can you determine the current I/O scheduler algorithm?

        1. `/sys/block/<device>/queue/scheduler`
        2. `/sys/block/<device>/iosch`
        3. `/etc/iostat.cfg`
        4. `/etc/default/ioscheduler`

        Answer:

        A.  The IO scheduler in use is found in `/sys/block/<device>/queue/scheduler`. The other options are not valid locations for this scenario.
155.    Which option to `iftop` prevents hostname lookups from occurring?

        1. `-d`
        2. `-a`
        3. `-t`
        4. `-n`

        Answer:

        D.  The `-n` option prevents hostname lookups from occurring with `iftop`. This is helpful for reducing the amount of noise or unnecessary information displayed within the `iftop` output. The other options do not accomplish the task required.
156.    Which command can be used within the `nslookup` CLI to change the server to which the query will be sent?

        1. `dest`
        2. `server`
        3. `srv`
        4. `auth`

        Answer:

        B.  The `server` command, when run within the `nslookup` interface, will set the server to which the query will be sent. The other options shown are not valid for this purpose.
157.    What are the minimum permissions needed for a user to write into a directory for which they are not the owner and are not in a group that owns the directory?

        1. Write
        2. Read/write/execute
        3. Read/execute
        4. Write/execute

        Answer:

        D.  A user would need write and execute permissions in order to write into a directory for which they are not the owner and do not have group ownership.
158.    Which of the following protocols provides a means for authentication to occur external to the Linux system?

        1. SSL
        2. SSH
        3. LDAP
        4. AD

        Answer:

        C.  LDAP can be used for external authentication scenarios with Linux and is frequently used to provide authentication in an integrated environment with Microsoft Windows and Active Directory. Of the other options, neither SSL nor SSH provides the external authentication, although SSH may be able to integrate with other authentication means. AD is frequently used as an abbreviation for Active Directory. While Active Directory has LDAP capabilities, it is different and separate from LDAP.
159.    When creating a file, a user is receiving an error. The file is very large. What command can the user execute in order to determine the file size limitation?

        1. `limit`
        2. `ulimit`
        3. `filelimit`
        4. `flimit`

        Answer:

        B.  The `ulimit` command shows the various limits that apply to a given user, including file size limitations. The other options are not valid.
160.    What are the minimum permissions for a Bash script so that it is executable by everyone without needing to prefix the command with the word _bash_?

        1. 755
        2. 644
        3. 777
        4. 222

        Answer:

        A.  The permissions should be 755 in order for a user to execute the script. The other options won't work for the purpose described or are too permissive.
161.    Which option within a systemd timer unit file is used to specify when a job should run?

        1. `OnCalendar=`
        2. `Time=`
        3. `RunAt=`
        4. `TimedEvent=`

        Answer:

        A.  The `OnCalendar=` configuration option is used to set the time when an event will run when using systemd timer unit files. The other options shown are not valid for use with systemd timer files.
162.    Which of the following abbreviations is used to signify time spent waiting for I/O in the output of the `top` command?

        1. `wi`
        2. `io`
        3. `wa`
        4. `iotime%`

        Answer:

        C.  The `wa` abbreviation in the output of `top` represents the percentage of time spent waiting for I/O operations such as disk or network. The other options are not valid for this scenario.
163.    Which of the following commands retrieves the current group membership list for a user?

        1. `groupmem`
        2. `groups`
        3. `lsgr`
        4. `getgr`

        Answer:

        B.  The `groups` command is used to retrieve a list of groups. The other commands are not valid.
164.    You have added a swap disk to a Linux server and have executed `mkswap`. However, on examination of the output from the `free` command, you see that the swap space is not being used. Which command do you need to execute?

        1. `swapon`
        2. `swap-en`
        3. `actswap`
        4. `swpact`

        Answer:

        A.  The `swapon` command activates the swap space for use. The other commands are not valid.
165.    Which option to `ioping` sets the size of the request?

        1. `-m`
        2. `-n`
        3. `-f`
        4. `-s`

        Answer:

        D.  The size of the request can be set using the `-s` option for `ioping`. The other options shown are not valid with `ioping`.
166.    Which option to the `dumpe2fs` command can be used to display blocks that are reserved because of being marked as bad?

        1. `-v`
        2. `-f`
        3. `-b`
        4. `-m`

        Answer:

        C.  The `-b` option prints known bad blocks. The `-f` option is used to force the display of information, and the other options don't exist.
167.    Which command can be used to obtain extended hardware and device information, including information about the motherboard?

        1. `mbhw`
        2. `lsmb`
        3. `dmidecode`
        4. `lsallhw`

        Answer:

        C.  The `dmidecode` command shows extended information about hardware and devices within a Linux system. The other options shown are not valid commands.
168.    You have found that a SATA disk within a RAID array has gone bad. Which option to `mdadm` removes the disk from the RAID array, placing it into a degraded state?

        1. `rm`
        2. `fail`
        3. `rem`
        4. `del`

        Answer:

        B.  The `fail` option to `mdadm` indicates that the disk has failed. The other options shown are not valid.
169.    Which option to `whois` suppresses the legal disclaimer information from certain registries?

        1. `-L`
        2. `-q`
        3. `-H`
        4. `-s`

        Answer:

        C.  The `-H` option suppresses the legal disclaimer when possible. The other options do not complete the task described in this scenario.
170.    Which option to `iftop` sets the interface on which `iftop` will listen?

        1. `-m`
        2. `-i`
        3. `-l`
        4. `-a`

        Answer:

        B.  The `-i` option sets the interface for `iftop`. The other options shown are not valid for the required task.
171.    To which file can you echo “`- - -`” in order to cause a scan of a SCSI host adapter for new disks?

        1. `/sys/bus/scsi/hostscan`
        2. `/sys/class/scsi_host/hostN/scan`
        3. `/sys/class/<host>/scan`
        4. `/etc/scsiadm`

        Answer:

        B.  The file `/sys/class/scsi_host/hostN/scan` is used for this purpose, where `N` is the adapter number. The other paths are not valid for the purpose described in this scenario.
172.    A local user is having password issues. When local authentication is performed, which file provides encrypted password information?

        1. `/etc/passwd`
        2. `/etc/shadow`
        3. `/etc/encrpass`
        4. `/etc/passen`

        Answer:

        B.  The `/etc/shadow` file stores encrypted passwords. The `/etc/passwd` file does not store encrypted passwords, and the other options are not valid.
173.    Which option within a systemd unit file sets the user that a service will run as?

        1. `RunAs=`
        2. `User=`
        3. `UID=`
        4. `ID=`

        Answer:

        B.  The `User=` option sets the process to run as the given user. The other options are not valid.
174.    The out-of-memory killer has been killing some processes on the system and you suspect that there are memory leaks. Which columns within `ps` output are helpful for determining current memory usage for a given process?

        1. `size` and `rss`
        2. `mem` and `swap`
        3. `free` and `cache`
        4. `phy` and `vir`

        Answer:

        A.  The `size` and `rss` columns within `ps` output are helpful for determining memory usage for a given process. The other options are not valid for process-level troubleshooting.
175.    Which signal number corresponds to `SIGKILL`?

        1. 1
        2. 5
        3. 9
        4. 12

        Answer:

        C.  `SIGKILL` corresponds with signal number 9. The other numbers shown are valid signal numbers but are not `SIGKILL`.
176.    Which of the following classes is the default class type queried by the `host` command?

        1. `EX`
        2. `HS`
        3. `FO`
        4. `IN`

        Answer:

        D.  The `IN` class, or Internet class, is the default type of class queried with the `host` command. This can be changed by using the `-c` option for the `host` command.
177.    Which option to the `netstat` command displays the current routing table?

        1. `-r`
        2. `-t`
        3. `-a`
        4. `-l`

        Answer:

        A.  The routing table is displayed with the `-r` option. The other options do not display the routing table.
178.    Which option to the `du` command provides summary output?

        1. `-o`
        2. `-h`
        3. `-s`
        4. `-u`

        Answer:

        C.  The `-s` option displays summary output for the arguments given. The other options shown do not accomplish the required task.
179.    Which of the following commands can be used to find zombie processes?

        1. `ps -Z`
        2. `ps | grep Z`
        3. `ps | grep zombie`
        4. `ps -a -z`

        Answer:

        B.  The `ps` command lists processes, and using `grep` for the state of `Z` will show zombie processes. Of the other options, there is a `-Z` option for `ps` but it is not used for the purpose described.
180.    Which command can be used to list all of the detected hardware within a system?

        1. `lshw`
        2. `showhw`
        3. `lspic`
        4. `slist`

        Answer:

        A.  The `lshw` command shows all hardware within a system, giving detailed information about many aspects of that hardware. The other commands shown are not valid.
181.    Which option to the `ioping` command sets the number of requests to send?

        1. `-r`
        2. `-c`
        3. `-n`
        4. `-a`

        Answer:

        B.  The `-c` option sets the number of requests to send with `ioping`. The other options given are not valid for use with `ioping`.
182.    Which process state indicates that the process is currently running?

        1. `C`
        2. `R`
        3. `T`
        4. `V`

        Answer:

        B.  The `R` state indicates a process is running. The other options do not indicate a running state.
183.    A device mismatch is reported by `pvs`. Which command rescans volume groups after resolving the mismatch?

        1. `pv -scanvl`
        2. `vgscan`
        3. `rescanvg`
        4. `vg -scan`

        Answer:

        B.  The `vgscan` command can be used to resolve mismatch issues between volume groups with LVM. The other commands shown are not valid.
184.    Which setting disables automatic power state management on an NVMe drive?

        1. `ps_max_latency_us`
        2. `apst_ps_latency`
        3. `apst_off`
        4. `ps_apst_enable`

        Answer:

        A.  The `ps_max_latency_us` setting, typically set as part of the GRUB configuration within `nvme_core`, can be used to disable power save functions on an NVMe drive. The other options shown are not valid configuration options.
185.    Which timer expression configures a systemd timer unit file to execute once a week?

        1. `OnCalendar=*/7`
        2. `Time=Week`
        3. `OnCalendar=weekly`
        4. `TimedEvent=Sunday`

        Answer:

        C.  The `OnCalendar=weekly` expression will cause the event to run weekly. The other options shown are not valid for this scenario. It is notable that Option A contains `OnCalendar`, and asterisks or wildcards are valid when configuring event timing with systemd timers. However, that option is not correct because the syntax of the wildcard is wrong.
186.    Assuming that `/var/log/journal` exists, which type of storage is used when the `Storage=` option is set to `auto` within `journald.conf`?

        1. `none`
        2. `journal`
        3. `persistent`
        4. `volatile`

        Answer:

        C.  The `persistent` option is the default when `auto` is configured and `/var/log/journal` exists. Of the other options, `none` is valid and will not log but will forward to other targets and `volatile` will use memory. There is no journal setting for the `Storage=` option in journald.conf.
187.    You need to determine the score at which a process will be killed by the out-of-memory killer. Which file can be examined to determine the current setting for that process?

        1. `oom_score`
        2. `oom_setting`
        3. `outofmem_num`
        4. `ooe-l`

        Answer:

        A.  The `oom_score` file, found in `/proc/<pid>/`, contains the number at which the process will be considered within the out-of-memory killer process. A higher number means that there is an increased chance of the process being killed.
188.    Which option can be set for a systemd mount point in order to cause the boot process to continue even if the filesystem cannot be mounted?

        1. `bootcon`
        2. `nowait`
        3. `nofail`
        4. `skip`

        Answer:

        C.  The `nofail` option is used to indicate that the boot process should continue even if the mount point is not available. The other options are not valid.
189.    You need to send a command-line argument into the command started with `ExecStart=` within a systemd service file. Which character is used to indicate that a command-line argument will be passed?

        1. `@`
        2. `^`
        3. `>`
        4. `$`

        Answer:

        A.  The `@` character prefixed to the command indicates that the first argument after the command will be sent as `argv[0]`. The other options are not valid.
190.    Which option to the `su` command enables the user to log in as a different user?

        1. `-e`
        2. `-u`
        3. `-l`
        4. `-m`

        Answer:

        C.  The `-l` option enables login as a different user. The other options are not valid.
191.    Which option to `lscpu` produces output in JSON format?

        1. `-J`
        2. `-o`
        3. `--output`
        4. `-s`

        Answer:

        A.  The `-J` option produces output in JSON format. Of the other options, `-s` is used to change the sysroot directory. The other options are not valid.
192.    When troubleshooting certificate issues you need to view the entire certificate chain. Which option to `openssl s_client` displays the certificate chain?

        1. `-chain`
        2. `-certchain`
        3. `-showchain`
        4. `-showcerts`

        Answer:

        D.  The `-showcerts` option displays the certificate chain for the connection. The other options are not valid.
193.    You are examining a login issue for a user and you need to determine where their home directory is located. Within which file can you find their home directory?

        1. `/etc/passwd`
        2. `/etc/homedirs`
        3. `/etc/user.conf`
        4. `/etc/defaults/user`

        Answer:

        A.  The `/etc/passwd` file contains user information, including their home directory. The other options are not valid.
194.    Which option is used to configure how to reload a service using a systemd unit file?

        1. `ExecReload=`
        2. `Reload=`
        3. `ConfRel=`
        4. `ExecRes=`

        Answer:

        A.  The `ExecReload=` option is used to configure the command that will be executed when the service is reloaded. The other options are not valid.
195.    Which expression is used to define a timer that should be executed every minute with a systemd timer?

        1. `permin`
        2. `per_min`
        3. `minute`
        4. `minutely`

        Answer:

        D.  The `minutely` expression is used to signify a job that should run once per minute. The other options are not valid.
196.    Which option to `chage` is used to set the number of days of inactivity after password expiration until an account is locked?

        1. `-I`
        2. `-X`
        3. `-EX`
        4. `-S`

        Answer:

        A.  The `-I` option sets the number of days after password expiration until the account is locked. The other options are not valid.
197.    Which option within `/etc/login.defs` is used to configure the maximum number of days until a password change is required?

        1. `MAX_PASS_AGE`
        2. `PASSWORD_AGE`
        3. `PASS_MAX_DAYS`
        4. `DAYS_PASSEXP`

        Answer:

        C.  The `PASS_MAX_DAYS` option sets the number of days that a password is valid until it needs to be changed. The other options are not valid.
198.    You are troubleshooting I/O-related issues and need extended information about disk performance. Which option to `iostat` displays additional information?

        1. `-u`
        2. `-l`
        3. `-x`
        4. `-e`

        Answer:

        C.  The `-x` option shows additional statistics. The other options are not valid.
199.    Which option to `tune2fs` displays the current inode size of a filesystem?

        1. `-n`
        2. `-l`
        3. `-a`
        4. `-f`

        Answer:

        B.  The `-l` option shows several properties of the filesystem, including the inode size. The `-f` option causes `tune2fs` to force completion of the specified operation. The other options are not valid.
200.    Which `systemctl` command needs to be executed after making a change to a systemd-related configuration file?

        1. `systemctl daemon-reload`
        2. `systemctl reconfig`
        3. `systemctl regen`
        4. `systemctl setup`

        Answer:

        A.  The `systemctl daemon-reload` command executes the generators that re-create links and other systemd-related items. Even after running `daemon-reload`, you still typically need to restart the service too. The other options are not valid.
201.    Within the `[Timer]` section of a systemd timer file, which configuration directive is used to specify the process or service to start?

        1. `Service=`
        2. `Unit=`
        3. `Proc=`
        4. `Startup=`

        Answer:

        B.  The `Unit=` directive specifies the command that will be run when the timer is used. The other options are not valid.
202.    When managing a service with a `Type=exec` setting in its unit file, what needs to happen in order for systemd to mark it as successfully started?

        1. The process needs to return from its `execve()` call.
        2. The process needs to return from its `fork()` call.
        3. The process needs to send a signal to `systemfork()`.
        4. The process needs to send the `running()` signal to `systemctl`.

        Answer:

        A.  The process needs to return from `execve()`, meaning that the actual daemon has started successfully. This is a primary difference from the `Type=simple` configuration where only the `fork()` needs to happen (option B). The other options are not valid.
203.    Which configuration option is used within a systemd unit file to configure how to handle an out-of-memory killer?

        1. `OOMSetting=`
        2. `OOM=`
        3. `OOMPolicy=`
        4. `OOMSignal=`

        Answer:

        C.  Out-of-memory configuration is controlled by `OOMPolicy` within a service file or can be set to a default value in a systemd configuration file. The other options are not valid.
204.    Which option to `renice` will increase the priority for all processes by the `apache` user?

        1. `renice -1 -A apache`
        2. `renice -1 -u apache`
        3. `renice -1 -UA apache`
        4. `renice apache -a -1`

        Answer:

        B.  The `-u` option to `renice` completes the task successfully. The other options are not valid.
205.    Which option to `repquota` does not resolve UIDs and GIDs to their names?

        1. `-n`
        2. `-b`
        3. `-d`
        4. `-m`

        Answer:

        A.  The `-n` option will not resolve UIDs and GIDs to their names and can be used to speed up the report. The other options are not valid.
206.    Which command is used to change the SELinux type for a file?

        1. `chcon`
        2. `settype`
        3. `typeset`
        4. `setype`

        Answer:

        A.  The `chcon` command is used to change the SELinux type of a file and can be helpful when troubleshooting file access issues. The other options are not valid.
207.    While troubleshooting a file access issue, you find that the permissions allow the `accounting` group but that the user is not a member of the group. Which option to the `usermod` command adds a user to a group?

        1. `-ag`
        2. `-groupadd`
        3. `-a -G`
        4. `-addgr`

        Answer:

        C.  Using `-a -G` appends the group onto the user's list of groups. The other options are not valid to accomplish the necessary task.
208.    When working with a virtual machine on a hypervisor that handles I/O scheduling, which scheduling mechanism is suggested for virtual machines?

        1. `cfq`
        2. `noop`
        3. `timed`
        4. `vm-opt`

        Answer:

        B.  The `noop` scheduling algorithm is recommended for virtual machines on a hypervisor host that performs the I/O scheduling. Of the other options shown, `cfq` is the default scheduling algorithm. The other two options are not valid.
209.    When you're using `journalctl` to investigate an issue, which entries are shown first?

        1. Newest entries are shown first.
        2. Oldest entries are shown first.
        3. Failed entries are shown first.
        4. Smallest entries are shown first.

        Answer:

        B.  The oldest entries are shown first when running `journalctl`, thus making the other options incorrect.
210.    While troubleshooting a script that runs via `cron`, you find that the script needs elevated privileges through `sudo` but there will not be a way to enter a password through the script. Which option within `/etc/sudoers` enables the command to be executed without prompting for a password?

        1. `PASS=NO`
        2. `SKIPPASS`
        3. `NOPASSWD`
        4. `NOPASS`

        Answer:

        C.  Using the `NOPASSWD` option causes `sudo` to not prompt for the password. The other options shown are not valid with `sudo`.
211.    Services are not starting in the correct order. Which configuration option can be used within a systemd service unit file to delay a service from starting until another has started?

        1. `Before=`
        2. `Dep=`
        3. `Order=`
        4. `Prior=`

        Answer:

        A.  Using `Before=` and `After=` ensures ordering of services, thus making option A correct. The other options are not valid for ordering of systemd unit files.
212.    You are starting a containerized service through systemd but need to ensure that enough memory has been allocated to the container. Which option within a systemd unit file verifies that the specified amount of memory is available?

        1. `MinRAM=`
        2. `VerifyMem=`
        3. `VerMem=`
        4. `ConditionMemory=`

        Answer:

        D.  Using `ConditionMemory=` defines the amount of memory that needs to be available. Mathematical operators such as greater-than, equal, less-than, and others are available. The other options are not valid for specifying the amount of memory within a systemd unit file.
213.    You are looking for systemd-related unit files that have been created locally on the system. Within which directory are administrator-created unit files found?

        1. `/etc/systemd/system`
        2. `/etc/systemd/admin`
        3. `/etc/systemd/adminunit`
        4. `/etc/systemd.admin`

        Answer:

        A.  Administrator-created unit files are stored in `/etc/systemd/system`. The other locations specified are not valid.
214.    Which systemd target stops the system but does not power it down?

        1. `poweroff.target`
        2. `stop.target`
        3. `offline.target`
        4. `halt.target`

        Answer:

        D.  Using `halt.target` stops the system but does not power it down. Of the other options, `poweroff.target` exists and stops the system and also powers it down. The other options are not valid targets.
215.    When formatting the `Type=` option in a systemd mount file, you need to examine the man page referred to as `mount(8)`. Which of the following commands ensures that you're viewing the 8th level man page for `mount`?

        1. `man mount 8`
        2. `man mount_8`
        3. `man 8 mount`
        4. `man -n 8 mount`

        Answer:

        C.  Using `man 8 mount` ensures that the 8th level man page is viewed. The other options are not valid for this purpose.
216.    Which of the following commands can be used to determine if an interface link is operational?

        1. `ip link`
        2. `ip state`
        3. `eth state`
        4. `int state`

        Answer:

        A.  Looking for the `state` field within the output of the `ip link` command shows whether an interface is considered up or down. The other commands shown are not valid.
217.    Which target in iptables can be used to log packets that are dropped and can be helpful in determining the cause of packets being lost or blocked?

        1. `INV`
        2. `DEBUG`
        3. `LOG`
        4. `CHAIN`

        Answer:

        C.  The `LOG` target is used to log packets within iptables. The other targets presented as options are not valid in iptables.
218.    When you're troubleshooting a system that won't boot, which of the following lines can be placed on the kernel command line in order to invoke a debugging shell?

        1. `debug,shell`
        2. `systemd.debug-shell=1`
        3. `shell=debug`
        4. `emerg=debug`

        Answer:

        B.  Using `systemd.debug-shell=1` on the kernel command line results in a debug shell being made available early in the boot process. The other options are not valid for this purpose.
219.    When you're rebooting a system for diagnosis of an issue, the system appears to hang. Which option can be sent to the `reboot` command in order to bypass some of the normal shutdown process?

        1. `-b`
        2. `-now`
        3. `-f`
        4. `-f0`

        Answer:

        C.  Using `-f` forces the reboot, although the shutdown process is still noted as clean. The other options shown are not valid for this purpose.
220.    Which option to `systemctl` can be used to help find stuck jobs?

        1. `-stuck`
        2. `list-jobs`
        3. `stuck-jobs`
        4. `--hung-jobs`

        Answer:

        B.  Using `list-jobs` shows the state of jobs in progress. The other options shown are not valid for this purpose.
221.    You need to examine which services are started at a given `<target>`. Which command will accomplish this task?

        1. `systemctl show <target>`
        2. `systemctl serdep <target>`
        3. `systemctl <target> list-dep`
        4. `systemctl list-dep <target>`

        Answer:

        A.  The `systemctl show` command is used for this purpose. The output can be further refined through the use of the `-p` option. The other options shown are not valid for this purpose.
222.    Which systemd-related daemon is responsible for name resolution?

        1. `systemd-dns`
        2. `systemd-resolver`
        3. `systemd-nameservice`
        4. `systemd-resolved`

        Answer:

        D.  The `systemd-resolved` service is responsible for name resolution on systemd-enabled systems. Troubleshooting for `systemd-resolved` name resolution follows the same pattern as that of troubleshooting other systemd services. The other options shown are not valid.
223.    Which option to the dig command follows the DNS lookup recursively starting at the root?

        1. `+trace`
        2. `+fol`
        3. `+x`
        4. `+all`

        Answer:

        A.  Using `+trace` causes dig to follow recursively through the lookup process. The other options shown are not valid for this purpose.
224.    When using `journalctl` to investigate an issue, which option shows the messages related to the specified unit?

        1. `-k`
        2. `-u`
        3. `-p`
        4. `-S`

        Answer:

        B.  Using the `-u` option shows entries related to the unit file specified. The `-k` option displays kernel messages. The `-p` option is used to specify priority and the `-S` option displays messages since the specified time.
225.    Which command can be used to display all of the timers that are currently active with systemd?

        1. `systemctl timers`
        2. `systemctl show-timers`
        3. `systemctl list-timers`
        4. `systemctl --timers`

        Answer:

        C.  The `systemctl list-timers` command shows the timers that are active on the system. The other options are not valid.
226.    You are working with an SSD to run `fstrim` and receive the return code 64 when complete. What does 64 mean as a return code?

        1. Trim not supported.
        2. Trim succeeded.
        3. Trim succeeded on some filesystems and failed on others.
        4. Trim failed on all filesystems.

        Answer:

        C.  A return code of 64 indicates that trim succeeded on some filesystems and failed on some filesystems, so further investigation will be required. Trim succeeded is return code 0 and all failed is return code 32. The `fstrim` command won't run on an unsupported filesystem, making option A incorrect.
227.    Which systemd target can be used to boot into a minimal system that contains a shell and basic services?

        1. `comp.target`
        2. `emergency.target`
        3. `init.target`
        4. `small.target`

        Answer:

        B.  The `emergency.target` provides minimal boot with the service manager and facilitates starting individual unit files for further troubleshooting. The other targets shown are not valid.
228.    In order to see more verbose boot messages, which keywords should be removed from the kernel boot line?

        1. `verbose`
        2. `quiet splash`
        3. `silent`
        4. `littleboot`

        Answer:

        B.  Removing the combination of `quiet splash` results in additional verbosity being displayed on the console, which is needed for many troubleshooting scenarios. The other targets shown are not valid.
229.    Which of the following addresses is outside of the subnet defined by 192.168.1.0/25?

        1. `192.168.1.56`
        2. `192.168.1.1`
        3. `192.168.1.100`
        4. `192.168.1.200`

        Answer:

        D.  The address `192.168.1.200` falls outside the 192.168.1.0/25 address range, which ends at 192.168.1.127. The other options shown fall within the range.
230.    Which option changes the amount of time that grub waits before booting into the default operating system?

        1. `wait`
        2. `timeout`
        3. `waiter`
        4. `hold`

        Answer:

        B.  The `timeout` setting is used to configure the length of the pause before grub boots into the default operating system. The other answers are not valid for this purpose.
231.    While troubleshooting network congestion, which option to the `ss` command shows the overall number of network connections?

        1. `-s`
        2. `-c`
        3. \-`w`
        4. \-`h`

        Answer:

        A.  The `-s` option displays summary numbers of connections. The `-h` option displays help and `-w` displays raw sockets. There is no `-c` option.
232.    You are troubleshooting a storage problem, and a Serial ATA (SATA) disk or mount point may be missing. Which of the following identifiers is used by SATA disks?

        1. `/dev/hdX`
        2. `/dev/sataX`
        3. `/dev/sdX`
        4. `/disk/sataX`

        Answer:

        C.  SATA disks are addressed as `/dev/sdX`, just like a SCSI disk. `/dev/hdX` is a traditional ATA disk. The other options do not exist.
233.    Which file within `/etc/systemd/resolved.conf.d/` can be used to configure custom DNS servers on a system that uses systemd-resolved for name resolution?

        1. `dns_servers.conf`
        2. `resolverd.conf`
        3. `nss.conf`
        4. `dns.conf`

        Answer:

        A.  The `dns_servers.conf` file configures the DNS servers that will be used. The other options shown are not valid files.
234.    You need to configure additional logging in order to troubleshoot a daemon startup issue. Which of the following is the correct syntax and setting for `/etc/systemd/system.conf` to facilitate additional logging?

        1. `Log=All+Debug`
        2. `LogLevel=Max`
        3. `LogLevel=Debug`
        4. `Logging=all`

        Answer:

        C.  Setting `LogLevel=Debug` configures the maximum logging level for daemon processes started by systemd. The other options shown are not valid for this purpose.
235.    Which option to `systemctl` can be used to stop one or more jobs that are in progress?

        1. `cancel`
        2. `cancel-jobs`
        3. `--kill-jobs`
        4. `--job-kill`

        Answer:

        A.  The `cancel` option stops jobs in progress using their job ID as an argument. If no argument is given, then all jobs will be canceled. The other options shown are not valid for this purpose.
236.    Which command is used to change the state of the interface `eth0` to UP?

        1. `ip link set eth0 up`
        2. `bringup eth0`
        3. `ip up eth0`
        4. `ip ifup eth0`

        Answer:

        A.  The `ip link set <device> up` command attempts to bring an interface online. The other commands shown are not valid.
237.    Which character, when prefixed within an `ExecStart=` option, causes a failure exit status to be recorded but otherwise ignored?

        1. `I`
        2. `%`
        3. `#`
        4. `-`

        Answer:

        D.  A `-` prefixed to a filename causes failure status codes to be effectively ignored and instead just recorded or logged. The other characters have no effect and would likely cause errors themselves.
238.    Of the following, which is a required section within a systemd service unit file?

        1. `[Service]`
        2. `[Sys]`
        3. `[RunTimeConfig]`
        4. `[Svc]`

        Answer:

        A.  The `[Service]` section is required within a systemd service unit file. The other options shown are not valid for use in a systemd service unit file.
239.    A user is using `sudo` to run a command and typed their password in wrong. They reported receiving a rude message from the system as a result. Which option has likely been enabled within `/etc/sudoers`?

        1. `fixusers`
        2. `insults`
        3. `failme`
        4. `rude`

        Answer:

        B.  The `insults` option, disabled by default, has been enabled in sudoers, thus causing the message when a user types their password in wrong. The other options shown are not valid within sudoers.
240.    When you're using `journalctl` to investigate an issue, which option reverses the display of entries so that newest are shown first?

        1. `-a`
        2. `-r`
        3. `-g`
        4. `-t`

        Answer:

        B.  Using the `-r` option causes entries to be displayed in reverse order. The `-a` option displays all entries and the `-t` option is used to specify the syslog identifier to display. The `-g` option searches (greps) for the specified message.
241.    Due to inode exhaustion, you would like to change the size of inodes on a filesystem. Which option to `tune2fs` can be used for this purpose?

        1. `-I`
        2. `-i`
        3. `-s`
        4. `-v`

        Answer:

        A.  The `-I` option changes the inode size. The `-i` option changes the interval between checks. The `-s` and `-v` options are not used.
242.    Another administrator has asked you for help with a machine where user quotas are not working on the root filesystem. While you're troubleshooting the issue, which file should be present to indicate that quotas are enabled?

        1. `/user.quotas`
        2. `/root/aquota.user`
        3. `/etc/userpol.aquota`
        4. `/aquota.user`

        Answer:

        D.  The file /`aquota.user` indicates that quotas have been enabled on this filesystem. The other options are not valid to indicate that quotas have been enabled.
243.    Systemd is not recognizing that a service is starting correctly even though it is running. Attempts to stop the service through systemd have failed. Which configuration option in the service unit file can be used to set the command to run for this situation?

        1. `ExecStopPost=`
        2. `ExecKill=`
        3. `ExecStopReally=`
        4. `ExecReallyStop=`

        Answer:

        A.  The `ExecStopPost=` configuration option is recommended for these situations. The other options are not valid.
244.    You are troubleshooting a systemd mounted filesystem that does not appear to be working. The configuration file, `mount-snd.mount`, appears to have the correct configuration for both `What=` and `Where=` and other options. The filesystem should be mounting an NFS filesystem to `/var/snd`. Which of the following is a likely cause of this issue?

        1. The configuration file itself needs to be named in a special way, `var-snd.mount`.
        2. The dependencies are not set up correctly.
        3. The systemd journal is corrupt.
        4. The mount point needs to also be in `/etc/fstab.mount`.

        Answer:

        A.  Systemd requires special naming for filesystems managed through the systemd process. In addition to needing `.mount` file extensions, the name of the file itself needs to reflect the mount point but have dashes. Though there could be other reasons for the filesystem not mounting, making systemd happy is the first issue to address.
245.    When troubleshooting disk-related errors you need to change the behavior of the system so that a kernel panic is not triggered. You will use `tune2fs -e` to change the error behavior. Which of the following are available options for the error behavior?

        1. `resched-io` and `mailadmin`
        2. `offline` and `background`
        3. `continue` and `remount-ro`
        4. `ignore` and `redress`

        Answer:

        C.  The two behaviors aside from `panic` are `continue` and `remount-ro`. The other options shown are not valid error behaviors.
246.    When working with a systemd timer, what is the best possible accuracy setting for the `AccuracySec=` option?

        1. `1m`
        2. `1ms`
        3. `1s`
        4. `1us`

        Answer:

        D.  A setting of `1us` for the `AccuracySec=` option is the best accuracy setting with a systemd timer. The other options are less accurate than `1us`.
247.    Which environment variable contains the primary process ID within a systemd service unit file?

        1. `$DPID`
        2. `$MAINPID`
        3. `$PID`
        4. `$PRIMARY_PID`

        Answer:

        B.  The `$MAINPID` variable contains the process ID of the primary process associated with the service. The other options are not valid.
248.    Which configuration option is used within `/etc/fstab` as the equivalent of the `Requires=` option in a systemd mount file?

        1. `x-systemd.requires`
        2. `requires`
        3. `systemd-requires`
        4. `require-sys`

        Answer:

        A.  The `x-systemd.requires` option is used within `/etc/fstab` and parsed into systemd as `Requires=`. The other options are not valid.
249.    You need to change the startup arguments for a service managed by systemd. Which line within the unit file is used for this purpose?

        1. `Command`
        2. `ExecStart`
        3. `Startup`
        4. `StartCmd`

        Answer:

        B.  The `ExecStart` configuration option is used to provide the command line of the service that should be started. The other options shown are not valid.
250.    Which file contains information on currently mounted filesystems, including their mount options?

        1. `/etc/mtab`
        2. /`etc/fstab`
        3. `/tmp/files`
        4. `/etc/filesystems`

        Answer:

        A.  The `/etc/mtab` file contains currently mounted filesystems. Note that `/etc/fstab` contains filesystem information but not about which filesystems are currently mounted.
251.    Which command and option are used to display the number of times a filesystem has been mounted?

        1. `tune2fs`
        2. `cat /etc/fstab`
        3. `mount -a`
        4. `less /etc/fsmnt`

        Answer:

        A.  The `tune2fs` command displays a lot of information about filesystems, including the number of times the filesystem has been mounted. The number of mounts is not shown in `/etc/fstab` and `mount -a` simply mounts all filesystems shown in `/etc/fstab`. There is no `/etc/fsmnt` file.
252.    When you're using `lsblk --discard`, which columns should have nonzero values to indicate that SSD trim support is enabled?

        1. `DISC-GRAN` and `DISC-MAX`
        2. `TRIM-EN` and `TRIM-BYTES`
        3. `FSTRIM` and `NUMBYTES`
        4. `TRIM-BYTES` and `FSTRIM`

        Answer:

        A.  Nonzero values for the `DISC-GRAN` and `DISC-MAX` columns indicate that trim support is enabled. The remaining options do not contain valid column names for `lsblk` output.
