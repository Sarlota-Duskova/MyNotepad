# John the Ripper

### Automatic Cracking

`john --wordlist=[path to wordlist] [path to file]`

#### Identifying Hashes

`wget https://gitlab.com/kalilinux/packages/hash-identifier/-/raw/kali/master/hash-id.py` then: `python3 hash-id.py`

### Format-Specific Cracking

`john --format=[format] --wordlist=[path to wordlist] [path to file]`

`--format=raw-md5`

check the format: `john --list=formats`

### Unshadowing

`unshadow [path to passwd] [path to shadow]`

* `unshadow` - Invokes the unshadow tool
* `[path to passwd]` - The file that contains the copy of the /etc/passwd file you've taken from the target machine
* `[path to shadow]` - The file that contains the copy of the /etc/shadow file you've taken from the target machine

Or past credential of one user into file:

`root:x:0:0::/root:/bin/bash root:$6$Ha.d5nGupBm29pYr$yugXSk24ZljLTAZZagtGwpSQhb3F2DOJtnHrvk7HI2ma4GsuioHp8sm3LJiRJpKfIf7lZQ29qgtH17Q/JDpYM/:18576::::::`

`john --wordlist=/usr/share/wordlists/rockyou.txt --format=sha512crypt unshadowed.txt`

### Word Mangling

If we take the username: Markus Some possible passwords could be:

* Markus1, Markus2, Markus3 (etc.)
* MArkus, MARkus, MARKus (etc.)
* Markus!, Markus$, Markus\* (etc.)

### GECOS

* In /etc/shadow each field is seperated by a colon ":".
* Each one of the fields that these records are split into are called Gecos fields.
* John can take information stored in those records, such as full name and home directory name to add in to the wordlist it generates when cracking /etc/shadow hashes with single crack mode.

### Using Single Crack Mode

`john --single --format=[format] [path to file]`

hash.txt will look like: -mike:1efee03cdcb96d90ad48ccc7b8666033

### Custom Rules

`john --wordlist=[path to wordlist] --rule=PoloPassword [path to file]`

`[List.Rules:PoloPassword]` `cAz"[0-9] [!£$%@]"` In order to:

* Capitalise the first letter - `c`
* Append to the end of the word - `Az`
* A number in the range 0-9 - `[0-9]`
* Followed by a symbol that is one of `[!£$%@]`

Add all capital letters to the end of the word: `Az"[A-Z]"`

### Zip2John

`zip2john [options] [zip file] > [output file]`

### Rar2John

`rar2john [rar file] > [output file]`

### SSH2John

* If ssh2john is not installed, you can use ssh2john.py, which is located in the /opt/john/ssh2john.py

`python3 /opt/ssh2john.py` or on Kali `python /usr/share/john/ssh2john.py id_rsa > id_rsa_hash.txt`

`ssh2john [id_rsa private key file] > [output file]`

* `[id_rsa private key file]` - The path to the id\_rsa file you wish to get the hash of
* `>` - This is the output director, we're using this to send the output from this file to the...
* `[output file]` - This is the file that will store the output from
