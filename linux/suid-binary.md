# SUID binary

| user | group | others |
| :--: | :---: | :----: |
|  rwx |  rwx  |   rwx  |
|  421 |  421  |   421  |

{% hint style="info" %}
r - read

w - write

x - execute

u - user

g - group

o - others

a - all
{% endhint %}

Example: `chmod` as `755`, then it will be: `rwxr-xr-x`.

Example: `chmod` as `4744`, then it will be: `-rwsr--r--`.

SETUID = 4\
SETGID = 2\
STICKY = 1\
NONE = 0\
READ = 4\
WRITE = 2\
EXECUTE = 1

SUID (Set user ID): `rws rwx rwx`

* the special permission for the user access level has a single function
* if the owning group does not have execute permissions, then an uppercase **S** is used.

SGID (Set Group ID)

* it runs as if it were a member of the same group in which the file is a member.

GUID: `rwx rws rwx`

* if it’s an executable, then it runs with the permissions of the group. If it’s a directory, it results in all new files and directories created to belong to the group.

Other + t (sticky): `rwx rwx rwt`

* Only the **owner** (and **root**) of a file can remove the file within that directory

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
