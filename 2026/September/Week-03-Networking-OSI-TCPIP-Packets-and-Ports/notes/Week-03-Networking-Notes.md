# Week 3 Notes — Networking

**Period:** 14 September 2026 → 19 September 2026

## 1. OSI Model

The OSI model divides network communication into seven layers.

1. Physical
2. Data Link
3. Network
4. Transport
5. Session
6. Presentation
7. Application

The main reason for using layers is to break a complicated networking problem into smaller parts.

For security analysis, the layers can help identify what type of information or failure I am looking at.

## 2. TCP/IP Model

The TCP/IP model is commonly described using four layers:

1. Application
2. Transport
3. Internet
4. Link

Some examples:

- DNS → Application
- HTTP → Application
- TCP → Transport
- UDP → Transport
- IP → Internet
- Ethernet → Link

The exact mapping is not always one-to-one with the OSI model, so I should understand the relationship rather than simply memorising a table.

## 3. Packets, Segments and Frames

Data is encapsulated as it moves through the networking stack.

At a basic level:

- Application data is passed down the stack.
- The transport layer adds transport information.
- The network layer adds IP information.
- The link layer adds frame information.

The terminology depends on the layer being discussed.

A simplified view is:

Application data
→ Segment
→ Packet
→ Frame

On the receiving side, the process is reversed through decapsulation.

## 4. Encapsulation

Encapsulation means adding protocol information as data moves down the networking stack.

Headers can contain information such as:

- source address
- destination address
- protocol information
- port information
- sequencing information

This is important when examining packets because different layers provide different pieces of information.

## 5. Ports and Sockets

A port helps identify a network service or communication endpoint on a host.

Examples studied this week:

- 22 — SSH
- 53 — DNS
- 80 — HTTP
- 443 — HTTPS

A socket can be thought of as an endpoint used for network communication.

From a security perspective, listening ports are useful during investigation because they can show which services are accepting network connections.

A port number alone is not enough to determine whether something is malicious. It needs to be considered together with the protocol, process, service, host and traffic.

## 6. TCP

TCP is connection-oriented.

The basic TCP connection establishment process uses:

1. SYN
2. SYN-ACK
3. ACK

TCP also uses sequence and acknowledgement information.

The three-way handshake was inspected directly in Wireshark during this week's lab.

## 7. UDP

UDP is connectionless and does not establish a TCP-style three-way handshake.

It is useful for applications where lower overhead or different communication characteristics are preferred.

From a security perspective, UDP traffic still needs to be understood because security monitoring is not limited to TCP.

## 8. DNS

DNS is used to translate domain names into IP addresses and for other DNS-related records.

In the packet-flow lab, DNS was the first major stage I identified before following the subsequent communication.

## 9. TLS

TLS provides encryption and security for network communication.

When examining encrypted traffic, I may still be able to observe metadata such as:

- source and destination IP addresses
- ports
- packet timing
- packet sizes
- protocol information

The actual encrypted application content may not be visible without the appropriate decryption context.

## 10. HTTP

HTTP is an application-layer protocol used for web communication.

HTTPS generally involves HTTP being carried over a TLS-protected connection.

During the capstone I traced the communication flow rather than looking at HTTP in isolation.

## 11. Packet Flow

A simplified browser-to-server flow studied this week was:

DNS
↓
TCP connection
↓
SYN
↓
SYN-ACK
↓
ACK
↓
TLS communication
↓
HTTP/application communication

The exact packets and sequence can vary depending on the environment and protocol version, so this is a simplified model of the flow I investigated.

## 12. Security Perspective

Networking knowledge is important for SOC work because many investigations involve network evidence.

Useful questions include:

- Who communicated with whom?
- Which IP addresses were involved?
- Which ports were used?
- Which protocol was used?
- Was the connection established?
- Was DNS involved?
- Was the traffic encrypted?
- Which process or service was listening?
- Does the traffic pattern require further investigation?

## Weekly takeaway

This week helped me connect networking theory with actual traffic.

Instead of only remembering protocol names and model layers, I used Windows commands and Wireshark to observe network behaviour directly.

The most useful practical exercise was tracing the complete packet flow because it brought together DNS, TCP, TLS, HTTP, ports and packet analysis in one investigation.
