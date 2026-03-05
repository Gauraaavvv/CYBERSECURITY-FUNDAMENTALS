# HTTP Basics

HTTP stands for **Hypertext Transfer Protocol**.

It is the protocol used for communication between web browsers and web servers.

Whenever you visit a website, your browser sends an **HTTP request**, and the server responds with an **HTTP response**.

---

# Example HTTP Communication

Example when visiting a website:

```id="l18nvy"

Browser → HTTP Request → Web Server
Browser ← HTTP Response ← Web Server

```

Example URL:

```id="7tshfi"

https://example.com

```

---

# HTTP Request

An HTTP request is sent by the client (browser) to the server.

Example HTTP request:

```id="cvq48c"

GET /index.html HTTP/1.1
Host: example.com
User-Agent: Mozilla/5.0

```

Main components:

* Request Method
* URL / Path
* Headers
* Body (optional)

---

# HTTP Methods

HTTP methods define what action the client wants to perform.

Common HTTP methods include:

| Method | Purpose          |
| ------ | ---------------- |
| GET    | Retrieve data    |
| POST   | Send data        |
| PUT    | Update resources |
| DELETE | Remove resources |

Example GET request:

```id="1u5fbc"

GET /products HTTP/1.1

```

Example POST request:

```id="oj9h6d"

POST /login HTTP/1.1

username=admin
password=1234

```

---

# HTTP Headers

Headers provide additional information about the request or response.

Example request headers:

```id="1egaxn"

Host: example.com
User-Agent: Mozilla/5.0
Cookie: session=abc123

```

Headers are very important in web security because attackers often manipulate them.

Example attack:

* Cookie manipulation
* Authorization bypass
* Header injection

---

# HTTP Response

The server responds with an HTTP response.

Example response:

```id="ps1b6u"

HTTP/1.1 200 OK
Content-Type: text/html

<html>
Welcome to the website
</html>

```

---

# HTTP Status Codes

Status codes indicate the result of a request.

Common status codes include:

| Code | Meaning      |
| ---- | ------------ |
| 200  | Success      |
| 301  | Redirect     |
| 403  | Forbidden    |
| 404  | Not Found    |
| 500  | Server Error |

Example:

```id="f9p6ix"

HTTP/1.1 404 Not Found

```

---

# HTTP vs HTTPS

HTTP sends data **in plain text**.

This means attackers could intercept the communication.

HTTPS is the secure version of HTTP.

HTTPS uses **TLS encryption** to protect data during transmission.

Example:

```id="pyu2xd"

http://example.com
https://example.com

```

---

# HTTP in Web Security

Understanding HTTP is essential for web application testing.

Security professionals analyze HTTP traffic to identify vulnerabilities.

Tools commonly used include:

```id="wcc09a"

Burp Suite
OWASP ZAP
Wireshark

```

Example tasks:

* Intercepting HTTP requests
* Modifying parameters
* Testing for vulnerabilities

---

# Example Attack Scenario

Example login request:

```id="4y1j3t"

POST /login HTTP/1.1

username=admin
password=admin

```

An attacker may modify the request to attempt:

* SQL Injection
* Authentication bypass
* Parameter manipulation

---

# Key Takeaways

HTTP is the protocol used for communication between web browsers and web servers.

Important concepts include:

```id="45bhhh"

HTTP requests
HTTP responses
Headers
Status codes
HTTP methods

```

Understanding HTTP is essential for identifying and exploiting web vulnerabilities.
