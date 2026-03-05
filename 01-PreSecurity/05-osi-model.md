# OSI Model

The **OSI Model (Open Systems Interconnection Model)** is a conceptual framework that describes how data travels through a network.

It divides the communication process into **seven layers**, each responsible for a specific function.

Understanding these layers helps network engineers and security professionals analyze network behavior and identify potential vulnerabilities.

---

# The 7 Layers of the OSI Model

The OSI model consists of the following layers:

```id="mdj8el"
7 Application
6 Presentation
5 Session
4 Transport
3 Network
2 Data Link
1 Physical
```

Data travels **from top to bottom when sending** and **bottom to top when receiving**.

---

# OSI Data Flow

When a user sends data across a network, it passes through multiple layers.

Example:

```id="c0a0s7"

Application Layer
      ↓
Transport Layer
      ↓
Network Layer
      ↓
Data Link Layer
      ↓
Physical Layer

```

Each layer adds its own **header information** to the data.

This process is known as **encapsulation**.

---

# Layer 7 — Application Layer

This is the layer closest to the user.

It provides network services directly to applications.

Examples:

* Web browsers
* Email clients
* File transfer tools

Common protocols:

```id="2o3l6o"
HTTP
HTTPS
FTP
SMTP
DNS
```

Cybersecurity relevance:

Most **web application attacks** happen here.

Examples:

* SQL Injection
* Cross Site Scripting (XSS)
* File upload attacks

---

# Layer 6 — Presentation Layer

This layer is responsible for **data formatting and encryption**.

Functions include:

* Data encryption
* Data compression
* Data translation

Example:

```id="ryp0hu"
HTTPS encryption
```

Cybersecurity relevance:

Encryption protects sensitive data from attackers during transmission.

---

# Layer 5 — Session Layer

The session layer manages connections between systems.

Responsibilities include:

* Establishing sessions
* Maintaining sessions
* Terminating sessions

Example:

```id="3q8t17"
Login session between browser and server
```

Cybersecurity relevance:

Session hijacking attacks target this layer.

---

# Layer 4 — Transport Layer

The transport layer ensures reliable communication between systems.

Main protocols include:

```id="5y69jq"
TCP
UDP
```

TCP provides reliable communication.

UDP provides faster but less reliable communication.

Cybersecurity relevance:

Many attacks involve manipulating TCP connections.

Example attacks:

* Port scanning
* SYN flood attacks

---

# Layer 3 — Network Layer

This layer is responsible
