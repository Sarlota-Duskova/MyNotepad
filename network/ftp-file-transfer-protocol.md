# FTP (File Transfer Protocol)

* FTP server, which listens on **port 21** by default.
* Was developed to make the transfer of files between different computers with different systems efficient.
* FTP also sends and receives data as cleartext; therefore, we can use Telnet (or Netcat) to communicate with an FTP server and act as an FTP client.

**In the example below, we carried out the following steps:**

1. We connected to an FTP server using a Telnet client. Since FTP servers listen on port 21 by default, we had to specify to our Telnet client to attempt connection to port 21 instead of the default Telnet port.
2. We needed to provide the username with the command `USER frank`.
3. Then, we provided the password with the command `PASS D2xc9CgD`.
4. Because we supplied the correct username and password, we got logged in.

* `STAT` command can provide some added information.
* The `SYST` command shows the System Type of the target (UNIX in this case).
* `PASV` switches the mode to passive. It is worth noting that there are two modes for FTP:
  * **Active:** In the active mode, the data is sent over a separate channel originating from the FTP server’s port 20.
  * **Passive:** In the passive mode, the data is sent over a separate channel originating from an FTP client’s port above port number 1023.
* The command `TYPE A` switches the file transfer mode to ASCII.
* The command `TYPE I` switches the file transfer mode to binary.

**Examples of FTP server software include:**

* vsftpd
* ProFTPD
* uFTP
