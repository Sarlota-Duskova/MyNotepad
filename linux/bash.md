# Bash

|      Command      |             Full name             |            Purpose           |
| :---------------: | :-------------------------------: | :--------------------------: |
|       touch       |               touch               |          create file         |
|       mkdir       |           make directory          |        create a folder       |
|         cp        |                copy               |     copy a file or folder    |
|         mv        |                move               |     move a file or folder    |
|         rm        |               remove              |    remove a file or folder   |
|        file       |                file               | determine the type of a file |
|       man ls      |             manual ls             |           manual ls          |
|       ls -a       |     list files and directories    |        list all files        |
|     su -user2     |            switch user            |        switch to user2       |
|        PID        |   process identification number   |        PID process ID        |
|       ps aux      | snapshot of the current processes |       running processes      |
| Find . -name ‘\*’ |               find                |       shows all folders      |



systemctl => this command allows us to interact with the systemd process/daemon.

systemctl \[option] \[service] We can do four options with systemctl:

* Start
* Stop
* Enable
* Disable



* cmd+d => split terminal into 2
* shif+cmd+d => undo split
* ctrl+z => background a process
* fg => bring the process back to focus screen
* sigterm => kill the process, but allow it to do some cleanup tasks beforehand
* sigkill => kill the process, doesn't do any cleanup tasks
* sigstop => stop/ susspend a process kill
* ping google.com
* traceroute google.com => map the path your request takes as it heads to the target machine
* whois google.com => info about google IP
* nc => telnet find which port is open
* pdfinfo exiftool
* **`curl -s google.com`**
* `curl -s http://10.10.10.10/whatever`
* `echo -n "neco==" | base64 -d`

`http -v GET https://949e28ad57a200b65ef6eeb47841e4d8.ctf.hacker101.com/s3cr3t-4dm1n/ X-Forwarded-For:8.8.8.8`



## Raspberry Pi

`cd LCD-show/`

`./LCD35B-show-v2`

## GIT

`git init`

`git add .`

`git commit -m "first commit"`

`git remote add origin https://github.com/Sarlota-Duskova/freecodecamp.git`

`git pull --rebase origin main`

`git push -f origin main`

