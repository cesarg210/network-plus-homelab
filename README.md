# Network+ Homelab – Networking Foundation

## Objective

Develop strong networking fundamentals through hands-on configuration and packet-level analysis within a virtualized lab environment.

This lab takes a hands-on approach at core networking concepts aligned with my CompTIA Network+ study objectives, including TCP/IP behavior, subnetting, DNS resolution, and traffic analysis.

---

## Lab Environment

Virtualization:
- VMware Fusion (Apple Silicon)

Virtual Machines:
- Linux OS
- Windows 11
- Ubuntu Server

Networking Configuration:
- NAT networking
- Internal virtual subnet
- Static IP configuration via Netplan
- Manual DNS configuration

---

## Networking Skills Practiced

- Subnet mask interpretation
- CIDR notation analysis
- DNS resolution troubleshooting
- TCP three-way handshake analysis
- UDP vs TCP traffic comparison
- Kerberos authentication packet analysis
- Packet capture using tcpdump and Wireshark

---

## Packet Analysis Exercises

### 1. TCP, ARP, ICMP Breakdown
- TCP three-way handshake (Layer 4)
- Identified source and destination ports
- Analyzed sequence numbers
- ARP resolution (Layer 2)
- ICMP communication (Layer 3)
- Sequence and acknowledgment behavior
- SYN flood mechanics

### 2. DNS Query Analysis
- Captured DNS SRV lookups
- Identified UDP port 53 usage
- Traced name resolution flow

### 3. Kerberos Authentication Flow
- Observed traffic on port 88
- Identified client-to-KDC communication (same host)
- Validated authentication through packet capture
- Observed UDP to TCP fallback behavior

### 4. Wireshark Packet dissection
 Expand and observed:
- Ethernet headers
- IP headers
- TCP headers
- TTL
- window size
- MSS option
- TCP options
- raw hex data

---

## Tools Used

- tcpdump
- Wireshark
- iproute2 (ip a, ip route)
- netplan
- host / dig
- kinit / klist

---

## What I Learned

- How packet flow reflects authentication processes
- How DNS misconfiguration impacts Kerberos
- How to validate routing and gateway configuration
- How subnetting applies to real virtual networks
- How to analyze traffic without relying on automation
