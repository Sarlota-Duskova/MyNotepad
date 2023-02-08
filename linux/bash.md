# Bash

Stabilize shell:

`python -c 'import pty;pty.spawn("/bin/bash/")'`

Spawn a process, and connect its controlling terminal with the current process’s standard io. This is often used to baffle programs which insist on reading from the controlling terminal.

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

**ctrl + shift + c** - copy text

**ctrl + shift + v** - past text

**ctrl + a** - jumps to the beginning of line

**ctrl + e** - jumps to the end of line

**ctrl + shift + "+"** - zoom in

**ctrl + "-"** - zoom out

**ctrl + u** - deletes everything before cursor

**ctrl + k** - deletes everything after cursor

**ctrl + y** - put it back

**alt + backspace** - delete lasr word

**ctrl + x + e** - put line into editor

**ctrl + r** - find command in history



systemctl => this command allows us to interact with the systemd process/daemon.

systemctl \[option] \[service] We can do four options with systemctl:

* Start
* Stop
* Enable
* Disable

How to stop process:

`ctrl+c`

`ctrl+z` - sleep

`jobs` - find what jobs are sleeping

`bg 1` - background process

`fg 1` - back to foreground&#x20;

`wc` - word count

Found what processes is running with `jobs` and `ps` and then:

`kill -2 21345`

`pkill -9 ping kill` all ping processes





Save IP address:

`export IP=10.10.120.2`

then:

`$IP`



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

using redirection: `<command> < <file_name>`

There’s two types of output, `stdout` (standard out) for when a command is successful, and `stderr` (standard error) for when it’s not.

You can redirect `stderr` with `2>`

use `1>` to redirect `stdout`

`stdin` (standard in) is the third thing commands can use and is for getting input.&#x20;

&#x20;you can redirect `stdin` as well. Here's an example: `<command> < <filename_for_stdin>`

&#x20;Another way to set the `stdin` is by using the pipe (`|`). It will use the output from one command as input for another. Here's an example: `<command_1> | <command_2>`. This will take the `stdout` from `command_1` and use it as the `stdin` for `command_2`.&#x20;

``

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

