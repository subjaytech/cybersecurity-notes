# IPv4 Address Types and Communication Methods

## Overview

This module explored how IPv4 addresses are used for different types of network communication. It covered unicast, broadcast, and multicast communication, along with public, private, and special-use IPv4 addresses.

The module also introduced the historical classful addressing system and how classless addressing replaced it.

## Learning Objectives

By completing this module, I was able to:

- Differentiate between unicast, broadcast, and multicast communication.
- Identify public and private IPv4 addresses.
- Understand the purpose of NAT.
- Recognize special-use IPv4 addresses.
- Understand the limitations of classful addressing.
- Explain why classless addressing was introduced.

## IPv4 Communication Types

### Unicast

Unicast communication sends data from one device to one specific destination.

```text
One sender → One receiver
```

It is the standard communication method for most network traffic.

---

### Broadcast

Broadcast communication sends data from one device to all devices within the local network.

```text
One sender → All devices
```

A limited broadcast uses:

```text
255.255.255.255
```

Routers do not forward broadcast traffic by default. This prevents broadcast traffic from spreading unnecessarily across multiple networks.

---

### Multicast

Multicast communication sends data from one sender to a specific group of devices that have subscribed to the multicast group.

```text
One sender → Specific group
```

An example is:

```text
224.0.0.5
```

OSPF routers use this multicast address to communicate with other OSPF routers on the local network.

## Comparing Communication Types

| Type | Communication | Example |
|------|----------------|---------|
| Unicast | One-to-one | PC → Web Server |
| Broadcast | One-to-all | Device → Local Network |
| Multicast | One-to-group | OSPF → OSPF Routers |

The key difference between broadcast and multicast is control.

Broadcast reaches all devices on the local network, while multicast reaches only devices that have joined the specific multicast group.

## Public and Private IPv4 Addresses

### Private IPv4 Addresses

Private addresses are used within local networks and are not globally routable on the Internet.

Common private ranges include:

```text
10.0.0.0/8
172.16.0.0/12
192.168.0.0/16
```

Examples:

```text
10.0.0.15
172.16.5.20
192.168.1.10
```

### Public IPv4 Addresses

Public addresses are globally routable addresses used for communication across the Internet.

## Network Address Translation (NAT)

NAT allows devices using private IPv4 addresses to communicate with the Internet by translating private addresses into a public address.

Example:

```text
Private Network
192.168.1.10
      ↓
     NAT
      ↓
Public IPv4 Address
      ↓
   Internet
```

This also reduces the need for every device on a private network to have its own public IPv4 address.

## Classful Addressing

Earlier IPv4 networks used a classful addressing system:

- Class A
- Class B
- Class C
- Class D
- Class E

The rigid network sizes of Class A, B, and C resulted in inefficient allocation of IPv4 address space.

Classless addressing was introduced to allow networks to be allocated more efficiently based on their actual requirements.

## Key Takeaways

- Unicast communicates with one destination.
- Broadcast communicates with all devices on the local network.
- Multicast communicates with a specific group.
- Private IPv4 addresses are used inside local networks.
- Public IPv4 addresses are globally routable.
- NAT translates private addresses for communication with external networks.
- Classless addressing improved IPv4 address allocation efficiency.

## Skills Gained

- IPv4 communication types
- Unicast addressing
- Broadcast addressing
- Multicast addressing
- Public and private IPv4 addressing
- NAT fundamentals
- Classful addressing
- Classless addressing
