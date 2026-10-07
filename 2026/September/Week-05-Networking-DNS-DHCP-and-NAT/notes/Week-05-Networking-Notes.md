# Week 5 — Networking Notes
## DNS, DHCP, NAT/PAT and Troubleshooting

**Phase:** Phase 1 — Networking  
**Week:** 5  
**Status:** Completed

---

## 1. DNS Fundamentals

DNS (Domain Name System) is a core networking service used for name resolution.

A simplified resolution process is:

```text
Client → DNS query → DNS server → DNS response → IP address / DNS result
```

DNS is important during troubleshooting because a host can have general network connectivity while name resolution is failing.

### Security relevance

DNS traffic can provide useful evidence during investigations, including:

- domains being queried
- source hosts making queries
- DNS servers being used
- query and response behaviour
- unusual or unexpected DNS activity

---

## 2. DNS Security

I studied the security relevance of DNS and used Wireshark to observe DNS-related traffic.

Useful information during DNS analysis can include:

- source IP
- destination DNS server
- queried domain
- query type
- response
- timing
- frequency of queries

DNS can therefore become useful evidence when investigating suspicious network activity.

---

## 3. DHCP

DHCP (Dynamic Host Configuration Protocol) is used to provide network configuration to clients.

A DHCP exchange can be understood through the DORA sequence:

```text
Discover
   ↓
Offer
   ↓
Request
   ↓
Acknowledge
```

### DORA

**Discover** — the client begins the process of obtaining network configuration.

**Offer** — a DHCP server responds with an offer.

**Request** — the client requests the offered configuration.

**Acknowledge** — the server acknowledges the configuration.

### Security relevance

DHCP is useful during network investigation because it helps explain how a device receives network configuration and provides evidence about DHCP client/server activity.

---

## 4. NAT

NAT stands for Network Address Translation.

NAT allows address translation between network addressing contexts.

It is commonly encountered when private internal addresses communicate through a translated address toward another network.

### Security relevance

NAT matters during investigations because the address visible at one point in a communication path may not be the same address used by the original internal host.

---

## 5. PAT

PAT stands for Port Address Translation.

PAT uses port information as part of address translation so that multiple connections can share a translated address.

```text
Internal host
Private IP + Port
       ↓
     NAT/PAT
       ↓
Translated IP + Port
       ↓
External network
```

### Security relevance

Ports become important when analysing translated connections because multiple internal connections may be represented through a translated address.

---

## 6. Troubleshooting Principles

Networking troubleshooting should be systematic rather than based on random changes.

A useful approach is:

```text
Identify the problem
        ↓
Gather information
        ↓
Check likely causes
        ↓
Test
        ↓
Analyse the result
        ↓
Narrow the problem
        ↓
Verify
        ↓
Document
```

The important principle is to use evidence to decide what to check next.

### DNS troubleshooting

Useful checks include:

- whether the client has network connectivity
- whether the configured DNS server is reachable
- whether DNS queries are being sent
- whether DNS responses are being received
- whether the expected domain resolves
- whether observed traffic matches expected behaviour

### Wireshark in troubleshooting

Wireshark provides packet-level evidence when normal troubleshooting commands are not enough.

It can help answer:

- Was a query actually sent?
- Where was it sent?
- Did a response return?
- What protocol was used?
- What happened before or after the problem?

---

## 7. Investigation Lab Concepts

The final investigation work brought the topics together through:

- a troubleshooting decision tree
- DHCP investigation
- DNS packet investigation
- DHCP packet investigation

The purpose was to move from learning individual protocols to analysing network evidence and making a structured troubleshooting decision.

---

## Weekly Takeaway

This week connected DNS, DHCP, NAT/PAT and troubleshooting.

I studied how DNS handles name resolution, how DHCP provides network configuration, and how NAT/PAT affects address and port translation.

The practical work then moved into packet investigation with Wireshark.

The main lesson was that troubleshooting should be evidence-driven: identify the problem, inspect relevant traffic or configuration, narrow the possible causes, and verify the result.
