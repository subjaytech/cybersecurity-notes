# Networking Basics - Module 5: Communication Protocols

## Overview

This module introduced communication protocols and explained how they enable devices from different manufacturers and networks to communicate reliably.

It also covered protocol layering, the TCP/IP and OSI reference models, and the organizations responsible for developing Internet standards.

---

## Learning Objectives

By completing this module, I was able to:

- Explain the purpose of communication protocols.
- Describe how multiple protocols work together during network communication.
- Differentiate between the OSI and TCP/IP models.
- Identify the functions of the TCP/IP layers.
- Understand the purpose of RFCs and the Internet Engineering Task Force (IETF).

---

## What Are Communication Protocols?

Communication protocols are a set of agreed rules that govern how devices exchange information across a network.

For successful communication, devices must agree on:

- Sender and receiver identification
- Message formatting
- Transmission method
- Timing
- Error detection
- Delivery confirmation

Without common protocols, devices would not be able to communicate effectively.

---

## Protocol Layering

Network communication depends on multiple protocols working together.

For example, when loading a webpage:

| Protocol | Function |
|----------|----------|
| Ethernet | Transfers data within the local network |
| IP | Delivers packets between networks |
| TCP | Ensures reliable and ordered delivery |
| HTTP | Transfers web pages between client and server |

Each protocol performs a specific task while working with the others to complete the communication process.

---

## TCP/IP Model

The TCP/IP model is the protocol suite used by the modern Internet.

### Layers

1. Application
2. Transport
3. Internet
4. Network Access

Each layer provides services to the layer above it while relying on the services of the layer below it.

---

## OSI Reference Model

The OSI model is a conceptual framework used to understand how network communication works.

### Layers

1. Physical
2. Data Link
3. Network
4. Transport
5. Session
6. Presentation
7. Application

Unlike TCP/IP, the OSI model is primarily used for learning, troubleshooting, and understanding networking concepts.

---

## OSI vs TCP/IP

| OSI Model | TCP/IP Model |
|-----------|--------------|
| Application | Application |
| Presentation | Application |
| Session | Application |
| Transport | Transport |
| Network | Internet |
| Data Link | Network Access |
| Physical | Network Access |

Although both models describe the same communication process, the OSI model separates networking functions into more detailed layers.

---

## Request for Comments (RFC)

Request for Comments (RFC) documents define many of the standards used on the Internet.

RFCs are published and maintained by the Internet Engineering Task Force (IETF).

These standards allow devices, applications, and networks from different vendors to communicate using common protocols.

Examples include standards for:

- TCP
- IP
- HTTP
- SMTP
- DNS

---

## Skills Gained

- Communication protocols
- Protocol layering
- TCP/IP architecture
- OSI reference model
- Internet standards
- RFC documentation
- Network communication concepts

---

## Personal Takeaways

One of the biggest lessons from this module was understanding that network communication is not handled by a single protocol.

Every action performed over the Internet depends on multiple protocols working together, with each protocol responsible for a specific part of the communication process.

Learning the relationship between the OSI and TCP/IP models also made it easier to understand where different networking protocols operate and why both models remain important despite serving different purposes.

---

## References

- Cisco Networking Academy, Networking Basics
- RFC Editor
- Internet Engineering Task Force (IETF)
