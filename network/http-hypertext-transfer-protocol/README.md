# HTTP (Hypertext Transfer Protocol)

* Your web browser connects to the webserver and uses HTTP to request HTML pages and images among other files and submit forms and upload various files.
* HTTP sends and receives data as cleartext (not encrypted); therefore, you can use a simple tool, such as Telnet (or Netcat), to communicate with a web server and act as a “web browser”.

1. First, we connect to port 80 using `telnet 10.10.245.19 80`.
2. Next, we need to type `GET /index.html HTTP/1.1` to retrieve the page `index.htm`l or `GET / HTTP/1.1` to retrieve the default page.
3. Finally, you need to provide some value for the host like `host: telnet` and hit the Enter/Return key twice.

**Three popular choices for HTTP servers are:**

* Apache
* Internet Information Services (IIS) (requires paying for a license)
* nginx
