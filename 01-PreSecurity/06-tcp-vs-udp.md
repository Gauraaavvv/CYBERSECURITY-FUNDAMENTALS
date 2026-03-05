# TCP vs UDP

TCP and UDP are two important communication protocols used at the **Transport Layer (Layer 4)** of the OSI Model.

They define how data is transmitted between devices across networks.

---

# What is TCP

TCP stands for **Transmission Control Protocol**.

It is a **connection-oriented protocol**, meaning it establishes a reliable connection before transmitting data.

TCP ensures that:

* Data arrives correctly
* Data arrives in order
* Lost packets are retransmitted

Because of this reliability, TCP is widely used in applications where accuracy is critical.

Examples of protocols using TCP:

```id="1xvl2n"
HTTP
HTTPS
FTP
SSH
SMTP
```

Example:

When you open a website:

```
Browser → TCP connection → Web Server
```

---

# TCP Three-Way Handshake

Before communication begins, TCP establishes a connection using a **three-step process** called the **three-way handshake**.

```id="3e9ci0"

Client → SYN → Server
Client ← SYN-ACK ← Server
Client → ACK → Server

```

Steps explained:

1. **SYN**
   The client sends a request to establish a connection.

2. **SYN-ACK**
   The server acknowledges the request.

3. **ACK**
   The client confirms the connection.

After this handshake, data transfer begins.

---

# What is UDP

UDP stands for **User Datagram Protocol**.

It is a **connectionless protocol**, meaning data is sent without establishing a connection first.

UDP does not guarantee:

* Packet delivery
* Packet order
* Packet duplication

However, UDP is **much faster than TCP** because it does not perform connection checks.

Examples of protocols using UDP:

```id="53e5ri"
DNS
DHCP
VoIP
Streaming services
Online gaming
```

Example:

When your computer queries DNS:

```
Computer → DNS Request → DNS Server
```

No handshake occurs.

---

# TCP vs UDP Comparison

| Feature      | TCP                 | UDP            |
| ------------ | ------------------- | -------------- |
| Connection   | Connection-oriented | Connectionless |
| Reliability  | Reliable            | Unreliable     |
| Speed        | Slower              | Faster         |
| Packet Order | Guaranteed          | Not guaranteed |

---

# Cybersecurity Relevance

Understanding TCP and UDP is important for cybersecurity professionals because many attacks target network protocols.

Examples include:

**TCP-based attacks**

* SYN Flood Attack
* TCP session hijacking
* Port scanning

Example:

```id="l7t0j6"
nmap -sS target.com
```

This command performs a **TCP SYN scan**.

---

**UDP-based attacks**

* UDP Flood
* DNS amplification attacks

Example:

Attackers send large numbers of UDP packets to overwhelm a system.

---

# Real Example

When visiting a website:

```id="j1odrl"

1. DNS query (UDP)
2. TCP connection established
3. HTTP request sent
4. Server response received

```

Understanding this flow helps penetration testers analyze network traffic.

---

# Key Takeaways

TCP and UDP are transport layer protocols used for communication between systems.

Key differences:

```id="5gn7xa"

TCP → Reliable but slower
UDP → Faster but unreliable

```

Both protocols play important roles in networking and cybersecurity.
