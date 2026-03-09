# DNS Query Analysis – tcpdump

## Objective

Analyze DNS traffic at the packet level using tcpdump and understand:

- UDP-based DNS communication
- A vs AAAA records
- Transaction ID matching
- Ephemeral source ports
- DNS response structure

---

# Screenshot

![DNS Query and Response](screenshots/10-dns-query-response.png)

---

# Observed Traffic Breakdown

## 1️⃣ DNS Uses UDP

- No TCP handshake occurred.
- DNS queries were sent using UDP port 53.
- UDP is connectionless and lightweight.

---

## 2️⃣ Ephemeral Source Ports

Each query used a random high source port:

Example:
192.168.170.130.54515

This allows the system to match responses to requests.

---

## 3️⃣ Transaction ID

Example:
50935+

The transaction ID:

- Uniquely identifies the DNS query
- Must match in the response
- Prevents mismatched responses

---

## 4️⃣ A vs AAAA Records

Two queries were observed:

A? example.com → IPv4 address  
AAAA? example.com → IPv6 address  

Modern systems are dual-stack and request both record types.

---

## 5️⃣ DNS Response Format (1/0/0)

The numbers represent:

Answer RRs / Authority RRs / Additional RRs

In this capture:

1/0/0

Meaning:

- 1 answer record
- 0 authority records
- 0 additional records

---

# Skills Demonstrated

- Packet capture using tcpdump
- Interpretation of DNS query structure
- Understanding UDP vs TCP behavior
- Analysis of DNS resource record sections
- Dual-stack resolution awareness
