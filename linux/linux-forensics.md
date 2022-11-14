# Linux Forensics

## OS and account information

### OS release information

`cat /etc/os-release`

### User accounts

`cat /etc/passwd`

### Group Information

`cat /etc/group`

### Sudoers list

`sudo cat /etc/sudoers`

### Login information

In the `/var/log` directory, we can find log files of all kinds including `wtmp`and `btmp`.

The `btmp` file saves information about failed logins, while the `wtmp` keeps historical data of logins.

These files are not regular text files that can be read using `cat`, `less` or `vim`; instead, they are binary files, which have to be read using the `last` utility.

### Authentication logs

Every user that authenticates on a Linux host is logged in the auth log.

The auth log is a file placed in the location `/var/log/auth.log`.

It can be read using the `cat` utility, however, given the size of the file, we can use `tail`, `head`, `more` or `less` utilities to make it easier to read.

## System configuration

### Hostname

`cat /etc/hostname`

### Timezone

`cat /etc/timezone`

### Network configuration

`cat /etc/network/interfaces`

`ip address show`

### Active network connections

&#x20;We can use the `netstat` utility to find active network connections on a Linux host.

`netstat -natp`

### Running processes

`ps aux`

### DNS information

`cat /etc/hosts`

`cat /etc/resolv.conf`

## Persistence mechanisms

### Cron jobs

`cat /etc/crontab`

### Service startup

`ls /etc/init.d`

### .Bashrc

`cat ~/.bashrc`

## &#x20;Evidence of execution

### Sudo execution history

`cat /var/log/auth.log* |grep -i COMMAND|tail`

### Bash history

`cat ~/.bash_history`

### Files accessed using vim

`cat ~/.viminfo`

## Log files

### Syslog

The Syslog contains messages that are recorded by the host about system activity.

We can use the `cat` utility to view the Syslog, which can be found in the file `/var/log/syslog`.

Since the Syslog is a huge file, it is easier to use `tail`, `head`, `more` or `less` utilities to help make it more readable.

### Auth logs

The auth logs contain information about users and authentication-related logs.

`cat /var/log/auth.log* |head`

### Third-party logs

Similar to the syslog and authentication logs, the `/var/log/` directory contains logs for third-party applications such as webserver, database, or file share server logs. We can investigate these by looking at the`/var/log/`directory.
