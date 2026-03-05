# HTTPS and TLS

HTTPS stands for **Hypertext Transfer Protocol Secure**.

It is the secure version of HTTP and is used to protect communication between a web browser and a web server.

HTTPS uses **TLS (Transport Layer Security)** to encrypt data transmitted across the internet.

---

# Why HTTPS is Important

Normal HTTP traffic is **not encrypted**.

This means attackers on the same network could intercept and read sensitive data.

Example:

```id="4v0xhs"

HTTP login request
username=admin
password=1234

```

Attackers could capture this information using tools like **Wireshark**.

HTTPS prevents this by encrypting the communication.

---

# What TLS Does

TLS provides three major security properties.

```id="l6s2hx"

Encryption
Integrity
Authentication

```

---

# Encryption

Encryption ensures that data transmitted between the client and server cannot be read by attackers.

Example:

```id="x9v2o3"

Plain text → Encrypted data

```

Only the intended server can decrypt the data.

---

# Integrity

Integrity ensures that the transmitted data cannot be modified during transmission.

If attackers try to alter the data, the communication will fail.

---

# Authentication

Authentication verifies that the website you are connecting to is legitimate.

This is done using **digital certificates**.

Example:

Your browser verifies the certificate before establishing a secure connection.

---

# TLS Handshake

Before secure communication begins, the client and server perform a **TLS handshake**.

This process establishes encryption keys.

Example simplified handshake:

```id="5i4l9y"

Client → Hello → Server
Server → Certificate → Client
Client verifies certificate
Encryption keys generated
Secure connection established

```

After the handshake, all communication becomes encrypted.

---

# Digital Certificates

Websites use **SSL/TLS certificates** to prove their identity.

Certificates are issued by **Certificate Authorities (CA)**.

Examples of CAs include:

```id="n6d4m0"

Let's Encrypt
DigiCert
GlobalSign

```

When a browser connects to a website, it verifies the certificate to ensure it is valid.

---

# Example HTTPS URL

Example secure website:

```id="s9y7jt"

https://example.com

```

Indicators of HTTPS include:

* Lock icon in browser
* Secure connection warning removed

---

# HTTPS in Cybersecurity

Understanding HTTPS helps security professionals analyze secure traffic.

Examples include:

* TLS handshake analysis
* certificate validation
* encrypted traffic inspection

Tools used include:

```id="x6d8kp"

Wireshark
Burp Suite
OpenSSL

```

---

# Example Security Risk

If attackers intercept traffic on an insecure WiFi network:

```id="j7m1ph"

HTTP → attacker can read data

HTTPS → attacker sees encrypted traffic

```

This is why most modern websites enforce HTTPS.

---

# Key Takeaways

HTTPS is the secure version of HTTP.

It uses **TLS encryption** to protect communication between clients and servers.

Key concepts include:

```id="q5e9zb"

Encryption
Integrity
Authentication
TLS handshake
Digital certificates

```

Understanding HTTPS is essential for analyzing secure web communication and detecting security issues.
