# Week 5 — Networking Labs
## DNS, DHCP, NAT/PAT and Troubleshooting

**Phase:** Phase 1 — Networking  
**Week:** 5  
**Status:** Completed

---

# Day 1 Lab — DNS Investigation with NSLOOKUP

## Objective

Investigate DNS resolution using `nslookup`.

## What I did

I used `nslookup` to investigate DNS resolution and connect the command-line result with the DNS fundamentals studied during the week.

## Tool

- Windows `nslookup`

## What I looked at

- DNS resolution
- DNS server information
- Domain queries
- Returned DNS results

## Result

I completed the DNS investigation using `nslookup`.

## Security relevance

`nslookup` is useful during basic network and security troubleshooting because it can help establish whether DNS resolution is working and which DNS infrastructure is involved.

---

# Day 2 Lab — DNS Security Observation

## Objective

Observe DNS traffic and consider its security relevance.

## What I did

I used Wireshark to observe DNS-related traffic and connected the packet activity with the DNS security concepts from the notes.

## Tool

- Wireshark

## What I observed

I examined DNS requests and responses and considered the information that can be obtained from DNS traffic during an investigation.

## Security relevance

DNS traffic can provide useful network evidence, including information about hosts making queries, DNS servers being contacted and domains being requested.

## Result

I completed the DNS security observation exercise.

---

# Day 3 Lab — Capture DORA

## Objective

Capture and observe the DHCP DORA process.

## What I did

I captured DHCP traffic and followed:

```text
Discover → Offer → Request → Acknowledge
```

## Tool

- Wireshark

## What I observed

I used the packet capture to follow the DHCP exchange and connect the four stages of DORA with actual network traffic.

## Result

I successfully captured and inspected the DHCP DORA exchange.

## Security relevance

Understanding DHCP traffic helps when investigating how a host obtains its network configuration and when interpreting network evidence related to a device.

---

# Day 4 Lab — Observe Networks in NAT Context

## Objective

Observe network communication in the context of NAT and PAT.

## What I did

I studied network communication from the perspective of address and port translation.

## Concepts examined

- NAT
- PAT
- Private addressing
- Translated addressing
- Port information

## Result

I completed the NAT/PAT observation exercise and connected the translation concepts with network traffic analysis.

## Security relevance

NAT/PAT is important during investigations because the address seen at one point in a communication path may represent translated traffic rather than the original internal addressing context.

---

# Day 5 Lab — Troubleshooting Decision Tree

## Objective

Use a structured troubleshooting decision tree to investigate a networking problem.

## What I did

I worked through a troubleshooting decision tree rather than approaching the problem by changing multiple things at once.

The process involved identifying the problem, gathering evidence, testing possible causes and narrowing the investigation.

## Investigation approach

```text
Identify
   ↓
Gather evidence
   ↓
Check likely causes
   ↓
Test
   ↓
Analyse
   ↓
Narrow the problem
   ↓
Verify
   ↓
Document
```

## Result

I completed the troubleshooting decision-tree exercise.

## Security relevance

Structured troubleshooting is directly relevant to SOC work because analysts need to investigate alerts and network problems systematically instead of relying on assumptions.

---

# Day 6 Lab 1 — DNS Packet Investigation

## Objective

Investigate DNS packets and understand the communication visible in the capture.

## What I did

I investigated DNS traffic in Wireshark and followed the DNS packet activity.

## Tool

- Wireshark

## What I investigated

- DNS queries
- DNS responses
- Network endpoints
- DNS communication flow

## Result

I completed the DNS packet investigation.

## Security relevance

Packet-level DNS investigation is useful when troubleshooting name resolution and when analysing DNS activity as part of a security investigation.

---

# Day 6 Lab 2 — DHCP Packet Investigation

## Objective

Investigate DHCP packets and understand the DHCP communication flow.

## What I did

I investigated DHCP traffic in Wireshark and followed the DHCP exchange.

I connected the captured packets with the DORA process studied earlier in the week.

## Tool

- Wireshark

## What I investigated

- DHCP communication
- DORA sequence
- Client/server interaction
- Packet-level evidence

## Result

I completed the DHCP packet investigation.

## Security relevance

DHCP packet analysis provides useful context when investigating how a host obtained network configuration and when correlating network activity during an investigation.

---

# Week 5 Practical Summary

The labs covered:

- DNS investigation with `nslookup`
- DNS security observation
- DHCP DORA capture
- NAT/PAT network observation
- Troubleshooting decision tree
- DNS packet investigation
- DHCP packet investigation

The practical work moved from individual protocol testing to packet-level investigation and structured troubleshooting.
