# Week 5 — DNS, DHCP, NAT/PAT and Network Troubleshooting

**Phase:** Phase 1 — Networking  
**Week:** 5  
**Status:** Completed

---

## Week Overview

Week 5 focused on network services and troubleshooting concepts that are important for understanding how hosts communicate and how analysts investigate network behaviour.

I covered:

- DNS fundamentals
- DNS security
- DHCP
- NAT
- PAT
- Troubleshooting principles
- DNS investigation
- DHCP investigation
- Packet analysis with Wireshark
- Troubleshooting decision trees

The week combined protocol concepts with practical investigation labs.

---

# Topics Covered

## DNS Fundamentals

I studied DNS and the role it plays in name resolution.

I investigated DNS resolution with `nslookup` and examined DNS traffic in Wireshark.

## DNS Security

I studied the security relevance of DNS and observed DNS traffic using Wireshark.

## DHCP

I studied DHCP and the DORA process:

```text
Discover → Offer → Request → Acknowledge
```

I then captured the DORA exchange using Wireshark.

## NAT and PAT

I studied NAT and PAT and how address and port translation affects network communication.

## Troubleshooting Principles

I studied systematic troubleshooting and used a troubleshooting decision tree in the practical work.

---

# Labs Completed

| Day | Lab | Main Tool / Focus |
|---|---|---|
| Day 1 | DNS Investigation with NSLOOKUP | `nslookup` |
| Day 2 | DNS Security Observation | Wireshark |
| Day 3 | Capture DORA | Wireshark / DHCP |
| Day 4 | Observe Networks in NAT Context | NAT / PAT |
| Day 5 | Troubleshooting Decision Tree | Structured troubleshooting |
| Day 6 | DNS Packet Investigation | Wireshark |
| Day 6 | DHCP Packet Investigation | Wireshark |

---

# Practical Work

### Day 1 — DNS Investigation with NSLOOKUP

I used `nslookup` to investigate DNS resolution and examine DNS server and query results.

### Day 2 — DNS Security Observation

I observed DNS traffic in Wireshark and considered its security relevance.

### Day 3 — Capture DORA

I captured DHCP traffic and followed the Discover, Offer, Request and Acknowledge sequence.

### Day 4 — NAT Context

I observed networking in a NAT/PAT context and connected address and port translation with network communication.

### Day 5 — Troubleshooting Decision Tree

I used a structured decision tree to approach network troubleshooting systematically.

### Day 6 — DNS Packet Investigation

I investigated DNS packets in Wireshark and examined the communication flow.

### Day 6 — DHCP Packet Investigation

I investigated DHCP packets and connected the observed traffic with the DORA process.

---

# What I Learned

This week helped me move from understanding individual networking concepts toward investigating network behaviour.

The practical progression was:

```text
Learn the protocol
      ↓
Test the protocol
      ↓
Observe the traffic
      ↓
Investigate the packets
      ↓
Use evidence to troubleshoot
```

---

# Security Relevance

The topics from Week 5 provide useful foundations for:

- DNS investigation
- Network troubleshooting
- PCAP analysis
- SOC alert investigation
- Network monitoring
- Incident response
- Understanding host/network configuration
- Investigating suspicious network activity

DNS and DHCP can provide useful context when trying to understand what a host was doing on a network.

NAT/PAT knowledge is also important because address and port translation can affect how network activity appears during an investigation.

---

# What I Can Explain Now

After completing Week 5, I should be able to explain:

1. What DNS does and why it is important.
2. How to perform a basic DNS investigation with `nslookup`.
3. Why DNS traffic can have security relevance.
4. What DHCP does.
5. The DHCP DORA process.
6. How to observe DHCP traffic in Wireshark.
7. What NAT does.
8. What PAT does.
9. Why addresses and ports matter when analysing translated traffic.
10. How to approach troubleshooting systematically.
11. How a troubleshooting decision tree helps narrow a problem.
12. How to investigate DNS packets in Wireshark.
13. How to investigate DHCP packets in Wireshark.

---

# Weekly Takeaway

The main takeaway from Week 5 was learning to treat networking as something that can be investigated using evidence.

I did not only study DNS, DHCP and NAT/PAT as definitions. I also used `nslookup`, Wireshark, packet captures and a troubleshooting decision tree to examine how these concepts appear in practice.

This gives me another layer of foundation for later PCAP investigation, SOC and security-monitoring work.

---

# Repository Contents

The Week 5 folder contains:

- `README.md` — weekly summary
- `notes/Week-05-Networking-Notes.md` — detailed networking notes
- `labs/Week-05-Networking-Labs.md` — Day 1 to Day 6 practical labs
