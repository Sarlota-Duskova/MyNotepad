# SUID binary

| user | group | others |
| :--: | :---: | :----: |
|  rwx |  rwx  |   rwx  |
|  421 |  421  |   421  |

{% hint style="info" %}
r - read

w - write

x - execute
{% endhint %}

Example: `chmod` as `755`, then it will be: `rwxr-xr-x`.

SUID (Set user ID): rws-rwx-rwx&#x20;

SGID (Set Group ID)

GUID: rwx-rws-rwx

Special Permissions (first bit in permissions) has the following options:

1. \_ - no special permissions set
2. d – directory
3. l – file has symbolic links
4. s – setuid or setgid is set
5. t – sticky bit set





`find / -perm -u=s -type f 2>/dev/null`

* `find` - Initiates the "find" command
* `/` - Searches the whole file system
* `-perm` - searches for files with specific permissions
* `-u=s` - Any of the permission bits mode are set for the file. Symbolic modes are accepted in this form
* `-type f` - Only search for files
* `2>/dev/null` - Suppresses errors
