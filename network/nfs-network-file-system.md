# NFS (Network File System)

* Allows a system to share directories and files with others over a network.
* First, the client will request to mount a directory from a remote host on a local directory just the same way it can mount a physical device.
* The mount service will then act to connect to the relevant mount daemon using RPC (Remote procedure call).

`sudo mount -t nfs IP:share /tmp/mount/ -nolock`

|    Tag   |                                   Function                                   |
| :------: | :--------------------------------------------------------------------------: |
|   sudo   |                                  Run as root                                 |
|   mount  |                           Execute the mount command                          |
|  -t nfs  |            Type of device to mount, then specifying that it's NFS            |
| IP:share | The IP Address of the NFS server, and the name of the share we wish to mount |
|  -nolock |                       Specifies not to use NLM locking                       |
