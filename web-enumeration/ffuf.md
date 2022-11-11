# FFUF

Tool used for web enumeration, fuzzing, and directory brute forcing.

Search for index.extension:

`ffuf -u http://10.10.80.249/indexFUZZ -w /usr/share/seclists/Discovery/Web-Content/web-extensions.txt`

Then find directories with extensions:

`ffuf -u http://10.10.80.249/FUZZ -w /usr/share/seclists/Discovery/Web-Content/raft-medium-words-lowercase.txt -e .php,.txt`

