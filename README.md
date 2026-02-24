# Network+ Homelab – Networking Foundation

## Objective

Develop strong networking fundamentals through hands-on configuration and packet-level analysis within a virtualized lab environment.

This lab reinforces core networking concepts aligned with CompTIA Network+ objectives, including TCP/IP behavior, subnetting, DNS resolution, and traffic analysis.

---

## Lab Environment

Virtualization:
- VMware Fusion (Apple Silicon)

Virtual Machines:
- Windows 11
- Ubuntu Server

Networking Configuration:
- NAT networking
- Internal virtual subnet
- Static IP configuration via Netplan
- Manual DNS configuration

---

## Networking Skills Practiced

- Static IP configuration
- Default gateway configuration
- Subnet mask interpretation
- CIDR notation analysis
- DNS resolution troubleshooting
- TCP three-way handshake analysis
- UDP vs TCP traffic comparison
- Kerberos authentication packet analysis
- Packet capture using tcpdump and Wireshark

---

## Packet Analysis Exercises

### 1. TCP Handshake Breakdown
- Observed SYN, SYN-ACK, ACK sequence
- Identified source and destination ports
- Analyzed sequence numbers

### 2. DNS Query Analysis
- Captured DNS SRV lookups
- Identified UDP port 53 usage
- Traced name resolution flow

### 3. Kerberos Authentication Flow
- Observed traffic on port 88
- Identified client-to-KDC communication
- Validated authentication through packet capture

---

## Subnetting Practice

Example network used in lab:

192.168.170.0/24

Documented:
- Network address
- Broadcast address
- Usable host range
- Host count
- CIDR interpretation

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
