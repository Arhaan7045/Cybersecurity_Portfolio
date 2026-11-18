
# EP-011 - Linux Networking Commands

## Mission

Investigated Ubuntu network configuration, connectivity, DNS resolution, listening services and HTTP communication.

## Commands Learned

- hostname -I
- ip addr
- ip route
- ping
- getent hosts
- nslookup
- dig
- ss
- curl

## Key Concepts

- IP address and network interface
- Default gateway and routing table
- ICMP and connectivity testing
- DNS resolution
- Listening sockets and network ports
- HTTP response headers and status codes

## Biggest Takeaway

Networking commands help analysts understand how a system communicates, identify connectivity issues and investigate potentially suspicious network activity.

## SOC Perspective

Analysts use network information to investigate destination IPs, listening services, DNS queries and connections initiated by processes.

A failed ping alone does not prove that a destination is offline.

## Practical Evidence

- Network interface:
- IPv4 address:
- Default gateway:
- Connectivity test:
- DNS result:
- Listening services:
- HTTP response status:

## Interview Questions

- What is an IP address?
- What is a default gateway?
- What is DNS?
- What does ss -tuln show?
- What does curl -I do?
- Does a failed ping prove a system is offline?

## Communication Practice

Explain the difference between an IP address and a domain name in simple English.

## Next Episode

Linux Package Management and Software Updates
