# Burp Suite - Intruder

List of Unicode Characters

abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789!"#$%&'()\*+,‐./:;<=>?@\[]^\_\`{|}\~

**Attack type:**

* Sniper
  * Username and password and list with 3 words make 6 request.

<table><thead><tr><th width="180.5" align="center">Request Number</th><th align="center">Request Body</th></tr></thead><tbody><tr><td align="center">1</td><td align="center">username=burp&#x26;password=Expl01ted</td></tr><tr><td align="center">2</td><td align="center">username=suite&#x26;password=Expl01ted</td></tr><tr><td align="center">3</td><td align="center">username=intruder&#x26;password=Expl01ted</td></tr><tr><td align="center">4</td><td align="center">username=pentester&#x26;password=burp</td></tr><tr><td align="center">5</td><td align="center">username=pentester&#x26;password=suite</td></tr><tr><td align="center">6</td><td align="center">username=pentester&#x26;password=intruder</td></tr></tbody></table>

* Battering ram
  * Use same word for two possition (username, password).

<table><thead><tr><th width="185.5" align="center">Request Number</th><th align="center">Request Body</th></tr></thead><tbody><tr><td align="center">1</td><td align="center">username=burp&#x26;password=burp</td></tr><tr><td align="center">2</td><td align="center">username=suite&#x26;password=suite</td></tr><tr><td align="center">3</td><td align="center">username=intruder&#x26;password=intruder</td></tr></tbody></table>

* Pitchfork
  * It is usefull when passwords leaked.

<table><thead><tr><th width="182.5" align="center">Request Number</th><th align="center">Request Body</th></tr></thead><tbody><tr><td align="center">1</td><td align="center">username=joel&#x26;password=J03l</td></tr><tr><td align="center">2</td><td align="center">username=harriet&#x26;password=Emma1815</td></tr><tr><td align="center">3</td><td align="center">username=alex&#x26;password=Sk1ll</td></tr></tbody></table>

* Cluster bomb
  * Will iterate through every combination of the provided payload sets to ensure that every possibility has been tested.

<table><thead><tr><th width="180.5" align="center">Request Number</th><th align="center">Request Body</th></tr></thead><tbody><tr><td align="center">1</td><td align="center">username=joel&#x26;password=J03l</td></tr><tr><td align="center">2</td><td align="center">username=harriet&#x26;password=J03l</td></tr><tr><td align="center">3</td><td align="center">username=alex&#x26;password=J03l</td></tr><tr><td align="center">4</td><td align="center">username=joel&#x26;password=Emma1815</td></tr><tr><td align="center">5</td><td align="center">username=harriet&#x26;password=Emma1815</td></tr><tr><td align="center">6</td><td align="center">username=alex&#x26;password=Emma1815</td></tr><tr><td align="center">7</td><td align="center">username=joel&#x26;password=Sk1ll</td></tr><tr><td align="center">8</td><td align="center">username=harriet&#x26;password=Sk1ll</td></tr><tr><td align="center">9</td><td align="center">username=alex&#x26;password=Sk1ll</td></tr></tbody></table>
