# NETCAT

* Netcat supports both TCP and UDP protocols.

`nc -vnlp 1234`

| option |                           meaning                          |
| :----: | :--------------------------------------------------------: |
|   -l   |                         Listen mode                        |
|   -p   |                   Specify the Port number                  |
|   -n   |      Numeric only; no resolution of hostnames via DNS      |
|   -v   | Verbose output (optional, yet useful to discover any bugs) |
|   -vv  |                   Very Verbose (optional)                  |
|   -k   |           Keep listening after client disconnects          |
