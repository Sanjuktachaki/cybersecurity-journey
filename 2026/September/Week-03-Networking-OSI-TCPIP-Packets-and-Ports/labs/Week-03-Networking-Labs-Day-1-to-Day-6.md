# Week 3 Labs — Networking

**Week:** 14 September 2026 → 19 September 2026  
**Phase:** Phase 1 — Networking  
**Status:** Completed

---

# Day 1 Lab — Network Troubleshooting by Layer

## Objective

Use basic Windows networking commands and relate the results to OSI layers.

## What I did

I used Windows networking commands to inspect different parts of the network configuration and connectivity.

The purpose was to understand how command output can provide evidence about different parts of a network connection.

## Commands / tools used

- Windows Command Prompt
- Basic Windows networking commands

## What I observed

The commands provided information about different parts of the network configuration and connectivity.

I compared the results with the OSI model instead of treating networking as one single layer.

## Security relevance

The same type of information can become useful during security troubleshooting.

For example, an analyst may need to determine whether an issue is related to:

- local network configuration;
- IP connectivity;
- DNS;
- transport connectivity;
- or an application/service.

## Result

I completed the troubleshooting exercise and connected the command results with the relevant networking concepts.

## What I learned

The main takeaway was that the OSI model is useful as a troubleshooting framework rather than just a theory topic.

It gives me a structured way to think about where a networking problem may be occurring.

---

# Day 2 Lab — Protocol Mapping

## Objective

Identify where common network protocols fit in the TCP/IP model.

## What I did

I mapped common protocols to the TCP/IP model and compared the mapping with the OSI model.

## Protocols studied

- DNS
- HTTP
- TCP
- UDP
- IP
- Ethernet

## Basic mapping

| Protocol | TCP/IP Layer | General OSI Relationship |
|---|---|---|
| DNS | Application | Application |
| HTTP | Application | Application |
| TCP | Transport | Transport |
| UDP | Transport | Transport |
| IP | Internet | Network |
| Ethernet | Link | Data Link / Physical relationship |

## Security relevance

Protocol identification is important during traffic analysis.

When looking at network traffic, knowing the protocol helps determine what type of communication I am looking at and what evidence may be relevant.

## Result

I completed the protocol mapping exercise and can now explain the basic relationship between the TCP/IP and OSI models.

## Takeaway

The models are useful for organising networking concepts. I should understand the purpose of the layers rather than relying only on memorised mappings.

---

# Day 3 Lab — Capture and Inspect a Packet

## Objective

Observe encapsulation inside real network traffic.

## Tool

Wireshark

## What I did

I generated network traffic and captured packets using Wireshark.

I then inspected the captured traffic and looked at the information available at different protocol layers.

## What I looked for

- Ethernet/frame information
- IP information
- Transport-layer information
- Source and destination information
- Protocol information
- Port information

## What I observed

The captured traffic showed how information from different networking layers appears together inside real traffic.

This made the concept of encapsulation easier to understand because I could see the protocol information rather than only reading about it.

## Security relevance

Packet captures can provide useful evidence during security investigations.

An analyst can use packet information to understand:

- communicating hosts;
- protocols;
- ports;
- connection behaviour;
- and other traffic characteristics.

## Result

I successfully captured and inspected network traffic and used the capture to connect networking theory with real packets.

## Evidence

Relevant screenshots and safe packet-capture evidence are stored separately where appropriate.

Private or sensitive traffic should not be uploaded.

---

# Day 4 Lab — Find Listening Services

## Objective

Identify listening network services and connect ports to processes.

## What I did

I checked which network services were listening for connections and connected the listening ports with the relevant processes or services.

## What I looked for

- Listening ports
- Protocol
- Local address
- Port number
- Associated process/service

## Why this matters

A listening service represents a potential network entry point into a system.

During security investigation, knowing what is listening can help establish:

- which services are exposed;
- which ports are in use;
- which process owns a connection;
- whether a service is expected in the environment.

A listening port is not automatically malicious. It needs to be interpreted in context.

## Result

I completed the exercise and connected network ports with the processes/services using them.

## Security relevance

This provides a basic foundation for later work involving:

- network enumeration;
- endpoint investigation;
- vulnerability assessment;
- incident response;
- and SOC investigations.

---

# Day 5 Lab — Observe TCP Handshake in Wireshark

## Objective

Identify the TCP three-way handshake and TCP flags in real traffic.

## Tool

Wireshark

## What I did

I generated TCP traffic and captured it in Wireshark.

I then located the TCP connection establishment and identified:

1. SYN
2. SYN-ACK
3. ACK

## TCP flags

The packets contained TCP flag information that helped identify the stage of the connection.

The main flags I focused on for this lab were:

- SYN
- ACK

## What I observed

The three packets showed the basic process used to establish a TCP connection.

Seeing the handshake in actual traffic made the sequence easier to understand than studying it only as a diagram.

## Security relevance

TCP handshake information can be useful when analysing network traffic.

An analyst may want to understand:

- whether a connection attempt occurred;
- whether a response was received;
- whether a TCP connection was established;
- and what other traffic followed the connection.

## Result

I successfully identified the TCP three-way handshake in Wireshark and connected the TCP flags with the connection process.

---

# Day 6 Lab — Full Packet Flow Capstone

## Objective

Trace a complete DNS, TCP, TLS and HTTP communication flow.

## Tools

- Wireshark
- Browser/network traffic
- Packet capture
- Packet-flow diagram

## What I did

For the final networking lab, I generated network traffic and captured it in Wireshark.

I then worked through the capture step by step instead of looking at individual packets separately.

The goal was to reconstruct the communication flow.

## Investigation process

### 1. DNS

I first identified the DNS activity associated with the communication.

This showed the domain-resolution stage before following the subsequent network traffic.

### 2. TCP connection

I then located the TCP connection.

I identified the:

- SYN
- SYN-ACK
- ACK

sequence.

This confirmed the TCP three-way handshake.

### 3. TLS

After establishing the TCP connection, I identified the TLS-related traffic.

Because TLS encrypts application data, the visible packet information was different from what would be available in unencrypted application traffic.

### 4. HTTP / application communication

I then followed the application-level communication represented in the traffic.

I used the available packet information to connect the traffic back to the overall communication flow.

## Full flow

My simplified investigation flow was:

```text
Browser / Application
        |
        v
      DNS
        |
        v
  Destination IP
        |
        v
   TCP connection
        |
        v
       SYN
        |
        v
     SYN-ACK
        |
        v
       ACK
        |
        v
      TLS
        |
        v
HTTP / Application communication
```

## Packet analysis

I used Wireshark to locate the relevant packets and follow the communication.

I did not treat each packet as an isolated event. Instead, I used addresses, ports, protocols and packet relationships to reconstruct the sequence.

## Security observations

The exercise showed that network evidence can provide useful information even when application traffic is encrypted.

Depending on the environment and available evidence, an analyst may still be able to observe things such as:

- source and destination IP addresses;
- ports;
- protocols;
- timing;
- packet sizes;
- DNS activity;
- connection attempts;
- TCP flags;
- TLS-related traffic.

The actual encrypted content is not automatically visible.

## Result

I successfully reconstructed the complete communication flow from DNS through TCP connection establishment and TLS to the application communication.

I also created a full flow diagram and recorded the relevant security observations.

## What this lab demonstrated

This lab brought together the main topics from Week 3:

- OSI model
- TCP/IP model
- packets
- ports
- TCP
- DNS
- TLS
- HTTP
- Wireshark
- packet analysis
- network investigation

## Security relevance

This is directly connected to later cybersecurity work involving:

- PCAP investigation;
- SOC alert investigation;
- network monitoring;
- threat detection;
- incident response;
- and network-based security analysis.

## Interview explanation

If asked to explain a basic browser-to-server flow, I can describe it as a sequence rather than only naming protocols.

I would start with DNS resolution, then explain the TCP connection and three-way handshake, followed by TLS and the application communication.

The exact sequence can vary depending on the protocol and environment, so I would describe this as the flow I investigated rather than claiming that every web connection always looks exactly the same.
