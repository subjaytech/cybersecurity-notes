# IPv4 Addressing and Packet Tracer

## Overview

This module introduced IPv4 addressing and how devices use IP addresses to communicate across networks.

The practical Packet Tracer activity helped connect the theory to actual network communication by testing connectivity with ping and accessing a web server directly through its IP address.

## Learning Objectives

By completing this module, I was able to:

- Explain the purpose of an IPv4 address.
- Understand the structure of an IPv4 address.
- Identify network and host portions of an address.
- Understand how source and destination IP addresses are used.
- Convert between binary and decimal representations of IPv4 addresses.
- Test network connectivity using Packet Tracer.

## IPv4 Address Structure

An IPv4 address is a 32-bit logical address divided into four 8-bit sections called octets.

Each octet is represented as a decimal value from 0 to 255.

Example:

```text
192.168.1.1
```

The four octets are:

```text
192 . 168 . 1 . 1
```

Each device uses an IP address to identify itself on a network and communicate with other devices.

## Network and Host Portions

An IPv4 address contains information identifying:

- The network
- The host on that network

The subnet mask determines which portion represents the network and which portion represents the host.

For devices to communicate directly on the same local network, their addresses must belong to the same network.

## Source and Destination Addresses

Network packets contain source and destination IP addresses.

The source address identifies where the packet came from.

The destination address identifies where the packet is going.

This allows devices to determine where network traffic should be delivered and where responses should return.

## Packet Tracer Activity

The practical activity involved communicating with a web server using its IPv4 address.

I:

1. Configured the required network devices.
2. Used Packet Tracer to test connectivity.
3. Sent ICMP traffic to the web server using `ping`.
4. Observed successful responses.
5. Accessed the web server through a browser using its IP address.

Example command:

```bash
ping <server-ip-address>
```

Successful replies confirmed that the addressing and network connectivity were functioning correctly.

## Key Concepts

### IPv4

A 32-bit logical addressing system used to identify devices on an IP network.

### Octet

An 8-bit section of an IPv4 address.

### Subnet Mask

Determines the network and host portions of an IPv4 address.

### Source IP

Identifies the device sending a packet.

### Destination IP

Identifies the intended recipient of a packet.

### Ping

A connectivity testing utility that uses ICMP to determine whether a destination is reachable.

## Practical Takeaway

The Packet Tracer activity made IPv4 addressing much easier to understand.

Seeing ping requests reach a server and receive replies provided a practical connection between IP addressing theory and actual network communication.

Accessing the same server through a browser using its IP address also demonstrated how correct addressing allows applications to communicate across a network.

## Skills Gained

- IPv4 addressing
- IP address structure
- Network and host identification
- Basic subnetting concepts
- ICMP connectivity testing
- Packet Tracer
- Basic network troubleshooting
