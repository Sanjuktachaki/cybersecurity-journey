# Week 4 — IPv4, Subnetting, Ethernet and ARP

**Week:** Week 4  
**Phase:** Phase 1 — Networking  
**Status:** Completed

## What I worked on

This week I continued building my networking foundation by focusing on IPv4 addressing, subnetting, local network communication, Ethernet and ARP.

The main topics I covered were:

- IPv4 structure
- Subnet masks
- CIDR
- Subnetting calculations
- MAC addresses
- Ethernet
- ARP
- Security applications of these networking concepts

Along with the notes, I completed practical labs using packet inspection and Wireshark.

## Notes and Concepts

### IPv4 Structure

I studied the structure of an IPv4 address and how IPv4 addressing is used to identify devices on a network.

### Subnet Masks and CIDR

I studied subnet masks and CIDR notation.

I also worked through subnetting calculations and practiced the calculations rather than only learning the definitions.

The focus was understanding how subnetting divides networks and how the CIDR prefix relates to the network and host portions of an IPv4 address.

### MAC and Ethernet

I studied MAC addresses and Ethernet as part of understanding communication at the local network level.

This connected IPv4 addressing with Ethernet traffic.

### ARP

I studied ARP and how it connects IP addressing with MAC addressing on a local network.

I also captured and inspected ARP traffic using Wireshark.

### Security Applications

I studied the security applications of IPv4, subnetting, MAC addresses, Ethernet and ARP.

These concepts provide a foundation for analysing network traffic and investigating network behaviour.

---

# Practical Labs

## Day 1 — Inspect IPv4 Packet

### Objective

Inspect an IPv4 packet and identify the IPv4 information available in the packet.

### What I did

I inspected IPv4 traffic and examined the information contained in the IPv4 packet using Wireshark.

### Result

I connected the IPv4 structure studied in the notes with real network traffic.

### Security relevance

IPv4 packet inspection is useful when analysing network traffic and understanding communication between hosts.

---

## Day 2 — Subnetting Practice

### Objective

Practice IPv4 subnetting calculations.

### What I did

I worked through subnetting calculations and practiced determining relevant network information from IPv4 addresses, subnet masks and CIDR notation.

### Result

I completed the subnetting practice and worked through the calculations independently.

### Security relevance

Subnetting knowledge is important for understanding network boundaries, addressing and the structure of internal networks during security and network investigations.

---

## Day 3 — Subnetting Practice

### Objective

Continue practicing IPv4 subnetting and CIDR calculations.

### What I did

I completed additional subnetting calculations to reinforce the concepts from the previous lab.

The focus was on applying the subnetting process rather than only remembering definitions.

### Result

I completed the subnetting practice and reinforced my understanding of subnet masks and CIDR.

### Security relevance

A security analyst needs to understand IP addressing and network ranges when interpreting network traffic and investigating hosts within a network.

---

## Day 4 — Inspect Ethernet Traffic

### Objective

Inspect Ethernet traffic and connect Ethernet information with network communication.

### What I did

I used Wireshark to inspect Ethernet traffic and examine the information visible at the Ethernet level.

### Result

I connected the MAC and Ethernet concepts from the notes with real captured traffic.

### Security relevance

Ethernet and MAC-level information can be useful when analysing local network traffic and understanding communication between devices on the same network.

---

## Day 5 — Capture ARP Requests and Replies

### Objective

Capture and inspect ARP requests and replies.

### What I did

I used Wireshark to capture ARP traffic and observed ARP requests and replies.

This allowed me to connect IPv4 addressing with MAC addressing in actual network traffic.

### What I observed

I observed the ARP request and reply traffic and used the capture to understand how ARP operates on a local network.

### Result

I successfully captured and inspected ARP requests and replies using Wireshark.

### Security relevance

ARP traffic can be relevant during network investigations because an analyst may need to understand how IP addresses are resolved to MAC addresses on a local network.

---

# What I learned this week

This week helped me connect IPv4 addressing and local network communication with actual network traffic.

The subnetting exercises gave me practical experience with subnet masks and CIDR calculations instead of only learning the concepts theoretically.

The Wireshark labs helped me see IPv4, Ethernet and ARP information in real traffic.

## Security relevance

The topics from this week provide useful foundations for later cybersecurity work involving:

- Network traffic analysis
- PCAP investigation
- SOC investigations
- Network monitoring
- Incident response
- Vulnerability assessment
- Understanding internal network structure

## Weekly takeaway

The main takeaway from Week 4 was understanding how addressing works at different parts of a network.

I worked with IPv4 addressing and subnetting, then connected those concepts with MAC addresses, Ethernet and ARP at the local network level.

The practical Wireshark exercises made the concepts more concrete because I could inspect the traffic rather than only studying diagrams and definitions.

## What I can explain now

I should be able to explain:

1. The basic structure of an IPv4 address.
2. What a subnet mask is.
3. What CIDR notation represents.
4. How to perform basic subnetting calculations.
5. What a MAC address is.
6. The role of Ethernet in local network communication.
7. What ARP does.
8. How IPv4 and MAC addressing are connected through ARP.
9. How to inspect IPv4, Ethernet and ARP traffic in Wireshark.
10. Why these concepts matter during network and security investigations.

## Repository contents

The Week 4 folder contains:

- `README.md` — this weekly summary
- `notes/Week-04-Networking-Notes.md` — detailed notes
- `labs/Week-04-Networking-Labs.md` — Day 1 to Day 5 practical labs
