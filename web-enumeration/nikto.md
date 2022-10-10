# Nikto

### Basic scaning

`nikto -h vulnerable_ip`

### Verbosing our Scan

`-Display`

| Argument |                      Description                     |                                                                                                     Reasons for Use                                                                                                     |
| :------: | :--------------------------------------------------: | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |
|     1    | Show any redirects that are given by the web server. |                                              Web servers may want to relocate us to a specific file or directory, so we will need to adjust our scan accordingly for this.                                              |
|     2    |               Show any cookies received              | Applications often use cookies as a means of storing data. For example, web servers use sessions, where e-commerce sites may store products in your basket as these cookies. Credentials can also be stored in cookies. |
|     E    |                   Output any errors                  |                                                               This will be useful for debugging if your scan is not returning the results that you expect!                                                              |

### Tuning Your Scan for Vulnerability Searching

`-Tuning`

|           Category Name           |                                                                             Description                                                                            | Tuning Option |
| :-------------------------------: | :----------------------------------------------------------------------------------------------------------------------------------------------------------------: | :-----------: |
|            File Upload            |       Search for anything on the web server that may permit us to upload a file. This could be used to upload a reverse shell for an application to execute.       |       0       |
| Misconfigurations / Default Files |                       Search for common files that are sensitive (and shouldn't be accessible such as configuration files) on the web server.                      |       2       |
|       Information Disclosure      | Gather information about the web server or application (i.e. verison numbers, HTTP headers, or any information that may be useful to leverage in our attack later) |       3       |
|             Injection             |                               Search for possible locations in which we can perform some kind of injection attack such as XSS or HTML                              |       4       |
|         Command Execution         |                                        Search for anything that permits us to execute OS commands (such as to spawn a shell)                                       |       8       |
|           SQL Injection           |                                         Look for applications that have URL parameters that are vulnerable to SQL Injection                                        |       9       |

### Saving Your Findings

`nikto -h http://ip_address -o report.html`
