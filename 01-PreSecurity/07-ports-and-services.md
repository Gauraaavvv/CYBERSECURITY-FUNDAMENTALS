# Ports and Network Services

In computer networking, **ports** are communication endpoints that allow different services to run on the same system.

Each service running on a system listens on a specific port number.

This allows multiple services to operate simultaneously on one machine.

---

# Why Ports Exist

Imagine a server running multiple services:

* Web server
* SSH server
* Email server

All services use the same IP address.

Ports allow the system to determine **which service should handle incoming data**.

Example:

```id="vhhkcd"

IP Address → 192.168.1.10

Port 80 → Web Server
Port 22 → SSH Server
Port 25 → Mail Server

```

---

# What is a Port Number

A port number is a **16-bit number** used to identify specific services on a device.

Port numbers range from:

```id="i1e6dl"
0 – 65535
```

Ports are categorized into three types.

---

# Well-Known Ports (0–1023)

These ports are reserved for commonly used services.

Examples:

| Port | Service |
| ---- | ------- |
| 21   | FTP     |
| 22   | SSH     |
| 23   | Telnet  |
| 25   | SMTP    |
| 53   | DNS     |
| 80   | HTTP    |
| 443  | HTTPS   |

These ports are frequently targeted during penetration testing.

---

# Registered Ports (1024–49151)

These ports are assigned to user applications.

Examples:

```id="3ybwqf"
MySQL
PostgreSQL
Remote desktop services
```

---

# Dynamic / Private Ports (49152–65535)

These ports are temporarily assigned by the operating system for client connections.

Example:

When your browser connects to a web server.

---

# How Ports Work

When a client connects to a server, it specifies both:

* IP address
* Port number

Example:

```id="g66te4"

https://example.com:443

```

Here:

```
443 = HTTPS service
```

---

# Port Communication Example

Example communication when opening a website:

```id="y9rdj0"

Client Computer
      ↓
TCP Connection
      ↓
Server Port 443
      ↓
Web Server

```

This allows the web server to process the request.

---

# Port Scanning

Port scanning is a technique used by attackers and security professionals to discover open services on a system.

Open ports often indicate potential attack surfaces.

Example tool:

```id="9q8o9k"
nmap
```

Example scan:

```id="q8ms21"
nmap target.com
```

This command scans the target system to identify open ports.

---

# Example Nmap Output

```id="7z3n4n"

PORT   STATE SERVICE
22/tcp open  ssh
80/tcp open  http
443/tcp open https

```

This means:

* SSH service running
* Web server running
* Secure web server running

Attackers may try to exploit vulnerabilities in these services.

---

# Ports in Web Security

Understanding ports is important for web application testing.

Examples:

```
80 → HTTP
443 → HTTPS
8080 → Alternative web server
```

Sometimes developers run **admin panels on unusual ports**.

Example:

```id="g9h9eh"
example.com:8080/admin
```

These can become security weaknesses.

---

# Key Takeaways

Ports allow multiple services to run on a single system.

Important facts:

```id="zoxljg"

0–1023 → Well known ports
1024–49151 → Registered ports
49152–65535 → Dynamic ports

```

Security professionals often perform **port scanning** to identify potential attack surfaces.
