# Nikto

### Basic scaning

`nikto -h vulnerable_ip`

### Verbosing our Scan

`-Display`

<table><thead><tr><th width="130" align="center">Argument</th><th width="145" align="center">Description</th><th align="center">Reasons for Use</th></tr></thead><tbody><tr><td align="center">1</td><td align="center">Show any redirects that are given by the web server.</td><td align="center">Web servers may want to relocate us to a specific file or directory, so we will need to adjust our scan accordingly for this.</td></tr><tr><td align="center">2</td><td align="center">Show any cookies received</td><td align="center">Applications often use cookies as a means of storing data. For example, web servers use sessions, where e-commerce sites may store products in your basket as these cookies. Credentials can also be stored in cookies.</td></tr><tr><td align="center">E</td><td align="center">Output any errors</td><td align="center">This will be useful for debugging if your scan is not returning the results that you expect!</td></tr></tbody></table>

### Tuning Your Scan for Vulnerability Searching

`-Tuning`

<table><thead><tr><th align="center">Category Name</th><th width="286" align="center">Description</th><th align="center">Tuning Option</th></tr></thead><tbody><tr><td align="center">File Upload</td><td align="center">Search for anything on the web server that may permit us to upload a file. This could be used to upload a reverse shell for an application to execute.</td><td align="center">0</td></tr><tr><td align="center">Misconfigurations / Default Files</td><td align="center">Search for common files that are sensitive (and shouldn't be accessible such as configuration files) on the web server.</td><td align="center">2</td></tr><tr><td align="center">Information Disclosure</td><td align="center">Gather information about the web server or application (i.e. verison numbers, HTTP headers, or any information that may be useful to leverage in our attack later)</td><td align="center">3</td></tr><tr><td align="center">Injection</td><td align="center">Search for possible locations in which we can perform some kind of injection attack such as XSS or HTML</td><td align="center">4</td></tr><tr><td align="center">Command Execution</td><td align="center">Search for anything that permits us to execute OS commands (such as to spawn a shell)</td><td align="center">8</td></tr><tr><td align="center">SQL Injection</td><td align="center">Look for applications that have URL parameters that are vulnerable to SQL Injection</td><td align="center">9</td></tr></tbody></table>

### Saving Your Findings

`nikto -h http://ip_address -o report.html`
