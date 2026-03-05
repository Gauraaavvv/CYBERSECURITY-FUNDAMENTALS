# DNS Basics

DNS stands for **Domain Name System**.

It is responsible for translating human-readable domain names into IP addresses that computers can understand.

Example:

```id="11y60v"

google.com → 142.250.182.14

```

Humans prefer using domain names, but computers communicate using **IP addresses**.

DNS acts as the **internet's phonebook**.

---

# Why DNS Exists

Imagine trying to remember the IP addresses of every website.

Example:

```id="yjv25n"

142.250.182.14
151.101.65.69
172.217.160.78

```

This would be extremely difficult.

DNS allows users to access websites using easy-to-remember domain names.

Example:

```id="w7t82g"

https://google.com

```

DNS translates this domain into the correct IP address.

---

# How DNS Works

When you enter a website into your browser, several steps occur.

Example:

```id="p2rz3f"

https://example.com

```

The DNS resolution process works like this:

```id="y32a0e"

User → DNS Resolver → Root Server
        ↓
     TLD Server
        ↓
     Authoritative Server
        ↓
     IP Address returned

```

Steps explained:

1. Your computer asks a DNS resolver.
2. The resolver queries DNS servers.
3. The correct IP address is returned.
4. Your browser connects to the server.

---

# DNS Record Types

DNS servers store different types of records.

---

## A Record

Maps a domain name to an IPv4 address.

Example:

```id="a30p7x"

example.com → 192.168.1.1

```

---

## AAAA Record

Maps a domain name to an IPv6 address.

Example:

```id="txpbrp"

example.com → IPv6 address

```

---

## CNAME Record

Maps one domain name to another domain.

Example:

```id="ij4me5"

blog.example.com → example.com

```

---

## MX Record

Specifies the mail server responsible for receiving emails.

Example:

```id="mnh5jy"

example.com → mail.example.com

```

---

## TXT Record

Stores arbitrary text information.

Often used for:

* domain verification
* SPF records
* security policies

Example:

```id="wh5xg3"

v=spf1 include:_spf.google.com ~all

```

---

# DNS in Cybersecurity

DNS plays an important role in many cyber attacks.

Examples incl
