# WPScan

### Enumerating for Installed Themes

`wpscan --url http://cmnatics.playground/ --enumerate t`

### Enumerating for Installed Plugins

`wpscan --url http://cmnatics.playground/ --enumerate p`

### Enumerating for Users

`wpscan --url http://cmnatics.playground/ --enumerate u`

### The "Vulnerable" Flag

`wpscan --url http://cmnatics.playground/ --enumerate vp`

### Performing a Password Attack

`wpscan –-url http://cmnatics.playground –-passwords rockyou.txt –-usernames cmnatic`

### Adjusting WPScan's Aggressiveness (WAF)

aggressiveness profile (passive/aggressive) `--plugins-detection aggressive`
