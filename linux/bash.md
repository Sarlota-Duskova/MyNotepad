# Bash

| Command |    Full name   |            Purpose           |
| :-----: | :------------: | :--------------------------: |
|  touch  |      touch     |          create file         |
|  mkdir  | make directory |        create a folder       |
|    cp   |      copy      |     copy a file or folder    |
|    mv   |      move      |     move a file or folder    |
|    rm   |     remove     |    remove a file or folder   |
|   file  |      file      | Determine the type of a file |

split terminal into 2 => cmd+d undo split => shif+cmd+d

systemctl => this command allows us to interact with the systemd process/daemon. systemctl \[option] \[service] We can do four options with systemctl:

* Start
* Stop
* Enable
* Disable

ctrl+z => background a process fg => bring the process back to focus screen sigterm => kill the process, but allow it to do some cleanup tasks beforehand sigkill => kill the process, doesn't do any cleanup tasks sigstop => stop/ susspend a process kill PID => PID process ID ps aux => running processes Find . -name ‘\*’ => shows all folders man ls => manual ls -a => show hidden files su -user2 => switching to user2 ping google.com traceroute google.com => map the path your request takes as it heads to the target machine whois google.com => info about google IP nc => telnet find which port is open pdfinfo exiftool **curl -s google.com** `curl -s http://10.10.10.10/whatever` `echo -n "neco==" | base64 -d`

`http -v GET https://949e28ad57a200b65ef6eeb47841e4d8.ctf.hacker101.com/s3cr3t-4dm1n/ X-Forwarded-For:8.8.8.8`

### nmap

nmap -sV 10.10.34.74 => show nginx version

## Raspberry Pi

nmap 192.168.0.0/24 -p22 -Pn -n -v --open = v nastavení sítě najdu ip addresu a tu tam opíšu ssh pi@192.168.0.134 at home 10.0.1.15 pinout = zobrazí piny a info o Raspberry Pi ssh -i \~/.ssh/raspberry pi@192.168.0.134 192.168.0.32 Příbram domov 192.168.154.101 Příbram práce

cd LCD-show/ ./LCD35B-show-v2

## GIT

git init = bude sledovat danou složku například git status = vypíše mi provedené změny git log = vypíše kdy byli provedeny změny git add index.html = přidá do sledování soubor git commit -m "create index.html" = zpráva co jsem udělala za změnu, uložím soubor na GIT git add . = přidá do sledování vše git checkout = vrátím se k původnímu před změnou git checkout = podívám se na původní verzi git branch = abych se vrátila k původní git checkout master = vrátím se k původnímu git merge něco = spojím master s jiným stromem událostí git push = uložit GIT commit na GITHUB git pull = stáhnout z GITHUBU změny v souboru do počítače git clone = stáhne úložiště z githubu do počítače

git init git add . git commit -m "first commit" git remote add origin https://github.com/Sarlota-Duskova/freecodecamp.git git pull --rebase origin main git push -f origin main

git init git rm -r /Users/sarlot/Desktop/Programming/GitHub/freecodecamp/9-Information-Security/1-Stock-price-checker\
git commit -m "remove folder" git remote add origin https://github.com/Sarlota-Duskova/freecodecamp.git git pull --rebase origin main git push -f origin main

git add /Users/sarlot/Desktop/Programming/GitHub/freecodecamp/docs git commit -m "add folder" git remote add origin https://github.com/Sarlota-Duskova/freecodecamp.git git pull --rebase origin main git push -f origin main
