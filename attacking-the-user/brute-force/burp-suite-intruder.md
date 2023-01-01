# Burp Suite - Intruder

List of Unicode Characters

abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789!"#$%&'()\*+,‐./:;<=>?@\[]^\_\`{|}\~

**Attack type:**

* Sniper
  * Username and password and list with 3 words make 6 request.

| Request Number |              Request Body             |
| :------------: | :-----------------------------------: |
|        1       |   username=burp\&password=Expl01ted   |
|        2       |   username=suite\&password=Expl01ted  |
|        3       | username=intruder\&password=Expl01ted |
|        4       |   username=pentester\&password=burp   |
|        5       |   username=pentester\&password=suite  |
|        6       | username=pentester\&password=intruder |

* Battering ram
  * Use same word for two possition (username, password).

| Request Number |             Request Body             |
| :------------: | :----------------------------------: |
|        1       |     username=burp\&password=burp     |
|        2       |    username=suite\&password=suite    |
|        3       | username=intruder\&password=intruder |

* Pitchfork
  * It is usefull when passwords leaked.

| Request Number |             Request Body            |
| :------------: | :---------------------------------: |
|        1       |     username=joel\&password=J03l    |
|        2       | username=harriet\&password=Emma1815 |
|        3       |    username=alex\&password=Sk1ll    |

* Cluster bomb
  * Will iterate through every combination of the provided payload sets to ensure that every possibility has been tested.

| Request Number |             Request Body            |
| :------------: | :---------------------------------: |
|        1       |     username=joel\&password=J03l    |
|        2       |   username=harriet\&password=J03l   |
|        3       |     username=alex\&password=J03l    |
|        4       |   username=joel\&password=Emma1815  |
|        5       | username=harriet\&password=Emma1815 |
|        6       |   username=alex\&password=Emma1815  |
|        7       |    username=joel\&password=Sk1ll    |
|        8       |   username=harriet\&password=Sk1ll  |
|        9       |    username=alex\&password=Sk1ll    |
