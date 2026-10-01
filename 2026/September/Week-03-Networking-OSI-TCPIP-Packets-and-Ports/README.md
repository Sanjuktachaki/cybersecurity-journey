\# Week 3 — Networking: OSI, TCP/IP, Packets and Ports



\*\*Week:\*\* 14 September 2026 → 19 September 2026  

\*\*Phase:\*\* Phase 1 — Networking  

\*\*Status:\*\* Completed



\## What I worked on



This week I worked on the basic networking concepts that are important for understanding how devices communicate and how a security analyst can investigate network activity.



The main topics I covered were:



\- OSI model

\- TCP/IP model

\- Packets, segments and frames

\- Encapsulation and decapsulation

\- Ports and sockets

\- Listening services

\- TCP and UDP

\- TCP three-way handshake

\- DNS, TCP, TLS and HTTP

\- Packet-flow analysis



The main goal was not only to memorize the models and protocol names, but to connect the concepts with actual network traffic and troubleshooting.



\## Practical work



I completed six networking labs during the week.



\### Day 1 — Network troubleshooting by layer



I used basic Windows networking commands and related the results to the appropriate OSI layers.



The purpose was to understand how an analyst can use different types of network information to narrow down where a problem may be occurring.



\### Day 2 — Protocol mapping



I mapped common networking protocols to the TCP/IP model and connected them with their approximate OSI-layer equivalents.



This helped me understand where protocols such as DNS, HTTP, TCP, IP and Ethernet fit into the overall communication process.



\### Day 3 — Capture and inspect a packet



I captured real network traffic and inspected the packet structure.



The main objective was to observe encapsulation in actual traffic rather than only studying it theoretically.



\### Day 4 — Find listening services



I checked listening network services and connected network ports with the processes/services using them.



This helped me understand why listening ports are relevant from a security perspective.



\### Day 5 — Observe TCP handshake in Wireshark



I captured TCP traffic in Wireshark and identified the TCP three-way handshake.



I looked at the SYN, SYN-ACK and ACK packets and connected the flags with the process of establishing a TCP connection.



\### Day 6 — Full packet-flow capstone



For the final lab, I traced a complete communication flow.



I generated network traffic, captured it and identified:



\- DNS activity

\- TCP connection establishment

\- SYN

\- SYN-ACK

\- ACK

\- TLS traffic

\- HTTP-related communication



I then organised the observations into a complete packet-flow diagram and recorded the security-related observations.



\## What I learned



The biggest change this week was moving from learning networking terms to actually looking at network traffic.



I now have a clearer understanding of how the OSI and TCP/IP models can be used to break down a networking problem.



I also understand the difference between packets, segments and frames at a basic level, and how data is encapsulated as it moves through the networking stack.



The TCP handshake became much easier to understand after seeing SYN, SYN-ACK and ACK in Wireshark.



I also learned why ports and listening services matter when investigating a system. A port by itself does not explain everything, so it is useful to connect the port with the protocol, service and process using it.



\## Security relevance



Networking is one of the foundations I need for cybersecurity and SOC work.



A security analyst may need to understand:



\- where network traffic came from;

\- where it was going;

\- which protocol was involved;

\- which port was used;

\- whether a connection was established;

\- what DNS activity occurred;

\- what traffic was encrypted;

\- and what information can be extracted from available network evidence.



The packet-flow exercise was particularly useful because it connected several of these concepts together.



\## Evidence



Practical evidence from this week includes:



\- Windows networking command results

\- protocol mapping

\- packet capture and inspection

\- listening-service results

\- TCP handshake analysis in Wireshark

\- full DNS/TCP/TLS/HTTP packet-flow analysis

\- packet-flow diagram



Sensitive or unnecessary personal network information is not included in the repository.



\## What I can explain now



I should be able to explain:



1\. What the OSI model is and why analysts use layers.

2\. How the TCP/IP model relates to the OSI model.

3\. The difference between packets, segments and frames.

4\. What ports and sockets are.

5\. The difference between TCP and UDP.

6\. How the TCP three-way handshake works.

7\. Where DNS, TCP, IP, TLS and HTTP fit into a typical communication flow.

8\. How Wireshark can be used to inspect network traffic.

9\. Why listening services and open ports matter during security investigation.

10\. How to trace a basic browser-to-server communication flow.



\## Next step



Next I will continue building my networking foundation and start connecting these concepts with security monitoring and investigation.



The longer-term goal is to use this knowledge when working with logs, PCAPs, SIEM tools and SOC investigations.

