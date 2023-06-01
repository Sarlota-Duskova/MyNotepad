# NFS (Network File System)

* Allows a system to share directories and files with others over a network.
* First, the client will request to mount a directory from a remote host on a local directory just the same way it can mount a physical device.
* The mount service will then act to connect to the relevant mount daemon using RPC (Remote procedure call).

`sudo mount -t nfs IP:share /tmp/mount/ -nolock`

<table><thead><tr><th width="115.5" align="center">Tag</th><th align="center">Function</th></tr></thead><tbody><tr><td align="center">sudo</td><td align="center">Run as root</td></tr><tr><td align="center">mount</td><td align="center">Execute the mount command</td></tr><tr><td align="center">-t nfs</td><td align="center">Type of device to mount, then specifying that it's NFS</td></tr><tr><td align="center">IP:share</td><td align="center">The IP Address of the NFS server, and the name of the share we wish to mount</td></tr><tr><td align="center">-nolock</td><td align="center">Specifies not to use NLM locking</td></tr></tbody></table>
