# Offensive Security

Offensive security focuses on **actively attacking systems in a controlled and ethical manner** to identify security weaknesses before malicious attackers exploit them.

Instead of simply defending systems, offensive security professionals **simulate real-world cyber attacks**.

This process helps organizations discover vulnerabilities and fix them before they can be exploited.

---

# Goal of Offensive Security

The main goal of offensive security is:

• Identify vulnerabilities
• Exploit weaknesses
• Demonstrate the impact of attacks
• Help organizations improve security

Offensive security is commonly performed through **penetration testing**.

---

# What is Penetration Testing

Penetration testing (Pentesting) is the process of **simulating cyber attacks against a system to evaluate its security**.

A penetration tester behaves like a real attacker and attempts to compromise systems.

Example targets include:

* Web applications
* Company networks
* Mobile applications
* Cloud infrastructure

---

# Typical Penetration Testing Workflow

A penetration test usually follows several phases.

```
Reconnaissance
        ↓
Scanning & Enumeration
        ↓
Vulnerability Discovery
        ↓
Exploitation
        ↓
Privilege Escalation
        ↓
Post Exploitation
        ↓
Reporting
```

---

# Phase 1 — Reconnaissance

Reconnaissance is the process of gathering information about the target.

Attackers try to identify:

* Domain names
* Subdomains
* IP addresses
* Technologies used by the target

Common tools used:

```
Google
whois
theHarvester
Amass
Subfinder
```

Example:

```
whois example.com
```

---

# Phase 2 — Scanning & Enumeration

After gathering basic information, attackers scan the target to identify open services.

This step helps identify:

* Open ports
* Running services
* Potential entry points

Example tool:

```
nmap
```

Example scan:

```
nmap -sV target.com
```

This command detects services running on the target.

---

# Phase 3 — Vulnerability Discovery

In this stage, attackers search for weaknesses in the system.

Examples include:

* SQL Injection
* Cross-Site Scripting (XSS)
* Authentication bypass
* Misconfigured servers

Tools often used:

```
Burp Suite
Nikto
Nuclei
OWASP ZAP
```

---

# Phase 4 — Exploitation

Once vulnerabilities are found, attackers attempt to exploit them.

Example:

SQL Injection attack:

```
' OR 1=1 --
```

This payload may allow attackers to bypass login authentication.

Example of exploitation tools:

```
Metasploit
Burp Suite
SQLMap
```

---

# Phase 5 — Privilege Escalation

After gaining access to a system, attackers attempt to increase their privileges.

Example:

```
Normal user → Administrator
```

Privilege escalation is commonly performed in:

* Linux systems
* Windows environments

---

# Phase 6 — Post Exploitation

After gaining higher privileges, attackers explore the system to identify valuable data.

Examples:

* Database credentials
* Sensitive documents
* Internal network access

---

# Phase 7 — Reporting

After the penetration test is completed, the findings are documented.

A professional penetration testing report includes:

* Vulnerability description
* Impact analysis
* Exploitation evidence
* Remediation recommendations

---

# Offensive Security in Real Life

Examples of offensive security activities include:

• Bug bounty hunting
• Web application penetration testing
• Red team operations
• Security research

Platforms used for learning offensive security include:

```
TryHackMe
Hack The Box
PortSwigger Labs
```

---

# Key Takeaways

Offensive security focuses on **attacking systems ethically** to identify vulnerabilities.

The main phases include:

```
Reconnaissance
Scanning
Vulnerability discovery
Exploitation
Privilege escalation
Post exploitation
Reporting
```

Understanding these phases helps security professionals simulate real attacker behavior.
