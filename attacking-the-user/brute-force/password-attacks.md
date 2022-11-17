# Password Attacks

## Password profiling

Tools such as `Cewl` can be used to effectively crawl a website and extract strings or keywords.

`cewl -w list.txt -d 5 -m 5 http://thm.labs`

`-w` will write the contents to a file. In this case, list.txt.

`-m 5` gathers strings (words) that are 5 characters or more

`-d 5` is the depth level of web crawling/spidering (default 2)

`http://thm.labs` is the URL that will be used



`crunch 8 8 0123456789abcdefABCDEF -o crunch.txt`&#x20;

crunch also lets us specify a character set using the `-t` option to combine words of our choice.

Here are some of the other options that could be used to help create different combinations of your choice:

`@` - lower case alpha characters

`,` - upper case alpha characters

`%` - numeric characters

`^` - special characters including space

## Offline attacks

### Dictionary attack

Let's say that we obtain the following hash f806fc5a2a0d5ba2471600758452799c, and want to perform a dictionary attack to crack it.

First, we need to know the following at a minimum:

1. What type of hash is this?
2. What wordlist will we be using? Or what type of attack mode could we use?

To identify the type of hash, we could a tool such as `hashid` or `hash-identifier`.

`hashcat -a 0 -m 0 f806fc5a2a0d5ba2471600758452799c /usr/share/wordlists/rockyou.txt --show`

`-a 0`  sets the attack mode to a dictionary attack

`-m 0`  sets the hash mode for cracking MD5 hashes; for other types, run hashcat -h for a list of supported hashes.

`f806fc5a2a0d5ba2471600758452799c` this option could be a single hash like our example or a file that contains a hash or multiple hashes.

`/usr/share/wordlists/rockyou.txt` the wordlist/dictionary file for our attack

`--show` option to show the cracked value if the hash has been cracked:

### Brute-Force attack

`hashcat -a 3 -m 0 05A5CF06982BA7892ED2A6D38FE832D6 ?d?d?d?d --stdout`

`-a 3`  sets the attacking mode as a brute-force attack

`?d?d?d?d` the ?d tells hashcat to use a digit. In our case, ?d?d?d?d for four digits starting with 0000 and ending at 9999

`--stdout` print the result to the terminal



