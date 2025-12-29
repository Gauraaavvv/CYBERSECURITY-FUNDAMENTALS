
# DNS and HTTP Basics for Security

## What DNS is (in simple words)
DNS (Domain Name System) translates human-readable domain names into IP addresses.
Without DNS, users would need to remember IP addresses to access websites.

## Why attackers care about DNS
Attackers abuse DNS to redirect users to malicious servers, monitor DNS requests for data exfiltration, or hide malicious traffic.
DNS is often trusted, which makes it a valuable target for attackers.

## Why defenders care about DNS
Defenders analyze DNS logs to detect suspicious domains, unusual request patterns, and communication with known malicious servers.
Blocking malicious domains at the DNS level can prevent attacks early.

---

## What HTTP is (in simple words)
HTTP is the protocol used for communication between a client (browser) and a web server.
It defines how requests and responses are sent over the network.

## Why attackers care about HTTP
Attackers exploit HTTP-based applications using techniques like SQL injection, XSS, and authentication bypass.
Insecure HTTP traffic can expose sensitive data.

## Why defenders care about HTTP
Defenders monitor HTTP traffic, logs, and application behavior to detect attacks.
Using HTTPS, secure headers, and input validation helps protect web applications.

---

## Common security risks related to DNS and HTTP
- DNS spoofing or poisoning
- Communication with malicious domains
- Plain HTTP traffic exposing sensitive data
- Poorly secured web applications

## Key takeaways
- DNS and HTTP are frequent attack targets
- DNS monitoring can stop attacks early
- Web security relies heavily on HTTP understanding
