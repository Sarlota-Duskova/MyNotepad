# POP3

* Is a protocol used to download the email messages from a Mail Delivery Agent (MDA) server.
* Default **port 110**.

```bash
pentester@TryHackMe$ telnet 10.10.81.251 110
Trying 10.10.81.251...
Connected to MACHINE_IP.
Escape character is '^]'.
+OK MACHINE_IP Mail Server POP3 Wed, 15 Sep 2021 11:05:34 +0300 
USER frank
+OK frank
PASS D2xc9CgD
+OK 1 messages (179) octets
STAT
+OK 1 179
LIST
+OK 1 messages (179) octets
1 179
.
RETR 1
+OK
From: Mail Server 
To: Frank 
```

* `USER frank`
* `PASS D2xc9CgD`
* Using the command `STAT`, we get the reply `+OK 1 179`; based on RFC 1939
  * a positive response to `STAT` has the format `+OK nn mm`
    * _nn_ is the number of email messages in the inbox.
    * _mm_ is the size of the inbox in octets (byte).
* The command `LIST` provided a list of new messages on the server.
* The command `RETR 1` retrieved the first message in the list.

### Difference between  POP and IMAP

* POP, or "Post Office Protocol" and IMAP, "Internet Message Access Protocol" are both email protocols who are responsible for the transfer of email between a client and a mail server.
* The main differences is in POP's more simplistic approach of downloading the inbox from the mail server, to the client.
* Where IMAP will synchronise the current inbox, with new mail on the server, downloading anything new.
