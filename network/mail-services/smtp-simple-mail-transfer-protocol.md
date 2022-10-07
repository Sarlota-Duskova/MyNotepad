# SMTP (Simple Mail Transfer Protocol)



**The SMTP server performs three basic functions:**

* It verifies who is sending emails through the SMTP server.
* It sends the outgoing mail
* If the outgoing mail can't be delivered it sends the message back to the sender

1. The mail user agent, which is either your email client or an external program. connects to the SMTP server of your domain, e.g. smtp.google.com. This initiates the SMTP handshake. This connection works over the SMTP port- which is usually 25. Once these connections have been made and validated, the SMTP session starts.
2. The process of sending mail can now begin. The client first submits the sender, and recipient's email address- the body of the email and any attachments, to the server.
3. The SMTP server then checks whether the domain name of the recipient and the sender is the same.
4. The SMTP server of the sender will make a connection to the recipient's SMTP server before relaying the email. If the recipient's server can't be accessed, or is not available- the Email gets put into an SMTP queue.
5. Then, the recipient's SMTP server will verify the incoming email. It does this by checking if the domain and user name have been recognised. The server will then forward the email to the POP or IMAP server, as shown in the diagram above.
6. The E-Mail will then show up in the recipient's inbox.



**Email delivery over the Internet requires the following components:**

* Mail Submission Agent (MSA)
* Mail Transfer Agent (MTA)
* Mail Delivery Agent (MDA)
* Mail User Agent (MUA)

**Five steps that an email needs to go through to reach the recipient’s inbox:**

1. A Mail User Agent (MUA), or simply an email client, has an email message to be sent. The MUA connects to a Mail Submission Agent (MSA) to send its message.
2. The MSA receives the message, checks for any errors before transferring it to the Mail Transfer Agent (MTA) server, commonly hosted on the same server.
3. The MTA will send the email message to the MTA of the recipient. The MTA can also function as a Mail Submission Agent (MSA).
4. A typical setup would have the MTA server also functioning as a Mail Delivery Agent (MDA).
5. The recipient will collect its email from the MDA using their email client.

#### Mail User Agent (MUA)

* A mail client application used by an end user to access a mail server to read, compose, and send email messages. Common MUAs include Microsoft Outlook and Mozilla Thunderbird.

#### Mail Transfer Agent (MTA)

* A program running on a mail server that receives messages from mail user agents or other MTAs and either forwards them to another MTA or, if the recipient is on the MTA, delivers the message to the local delivery agent (LDA) for delivery to the recipient. Common MTAs include Microsoft Exchange and sendmail.

**The protocols (protocols to talk with an MTA and an MDA) are:**

1. Simple Mail Transfer Protocol (SMTP)
2. Post Office Protocol version 3 (POP3) or Internet Message Access Protocol (IMAP)

**Simple Mail Transfer Protocol (SMTP)** is used to communicate with an MTA server. SMTP uses cleartext, where all commands are sent without encryption.

* SMTP server listens on **port 25**.
* Telnet client can be use to connect to an SMTP server and act as an email client (MUA) sending a message.

```
pentester@TryHackMe$ telnet 10.10.81.251 25
Trying 10.10.81.251...
Connected to MACHINE_IP.
Escape character is '^]'.
220 bento.localdomain ESMTP Postfix (Ubuntu)
helo telnet
250 bento.localdomain
mail from: 
250 2.1.0 Ok
rcpt to: 
250 2.1.5 Ok
data
354 End data with .
subject: Sending email with Telnet
Hello Frank
....
```

* `helo hostname` and then start typing our email.
* `mail from:`
* `rcpt to:` to indicate the sender and the recipient. When we send our email message, we issue the command `data` and type our message. We issue `<CR><LF>.<CR><LF>` (or `Enter . Enter` to put it in simpler terms).
