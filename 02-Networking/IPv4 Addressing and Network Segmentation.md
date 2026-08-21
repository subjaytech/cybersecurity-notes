# Networking Basics: IPv4 Addressing and Network Segmentation

## Overview

Today's session focused on public and private IPv4 addresses, Network Address Translation (NAT), special-use IPv4 addresses, IP address allocation, and network segmentation.

The difference between public and private IPv4 addresses finally became clear to me. The session also connected several networking concepts I had previously studied, especially how routers and switches control traffic within a network.

## Learning Objectives

By completing this session, I was able to:

- Differentiate between public and private IPv4 addresses.
- Understand how NAT allows private devices to communicate over the internet.
- Identify special-use IPv4 addresses.
- Understand the limitations of classful addressing.
- Explain how IANA and Regional Internet Registries (RIRs) distribute IP addresses.
- Understand broadcast domains and network segmentation.
- Explain how subnetting helps reduce unnecessary broadcast traffic.

## Public and Private IPv4 Addresses

Private IPv4 addresses are used within internal networks such as homes, schools, and offices.

The three private IPv4 ranges are:

- 10.0.0.0/8
- 172.16.0.0/12
- 192.168.0.0/16

These addresses are not globally routable on the public internet.

Public IPv4 addresses are globally routable and are used for communication across the internet.

## Network Address Translation (NAT)

Network Address Translation (NAT) allows devices using private IP addresses to communicate with the public internet.

When traffic leaves a private network, NAT translates the private source address into a public address at the network's connection to the ISP.

This allows devices inside a private network to access external networks without each device requiring its own public IPv4 address.

## Special-Use IPv4 Addresses

I also learned about IPv4 addresses reserved for specific purposes.

### Loopback Addresses

The 127.0.0.0/8 range is reserved for loopback communication.

The most familiar example is:

127.0.0.1

A device uses a loopback address to communicate with itself. This is useful for testing and troubleshooting local network services and configurations.

### Link-Local Addresses

The 169.254.0.0/16 range is used for link-local addressing.

When a Windows device fails to obtain an IPv4 address through DHCP, it can automatically assign itself a 169.254.x.x address.

This provides local communication even when normal IP configuration fails.

## Classful Addressing

The session also revisited the older classful IPv4 addressing system.

The original system divided IPv4 addresses into:

- Class A
- Class B
- Class C
- Class D
- Class E

Classful addressing used fixed network boundaries, which resulted in significant address wastage.

For example, Class A networks provided a huge number of addresses to relatively few organizations.

This inefficiency led to the adoption of classless addressing, which provides more flexibility when allocating IP address space.

## IP Address Allocation

Public IPv4 addresses are not assigned randomly.

The Internet Assigned Numbers Authority (IANA) manages global IP address allocation and distributes address blocks to five Regional Internet Registries (RIRs).

The RIRs then distribute address space to Internet Service Providers (ISPs), organizations, and other networks within their regions.

## Network Segmentation

The second part of the session focused on network segmentation and broadcast domains.

Ethernet broadcasts are used for processes such as:

- Address Resolution Protocol (ARP)
- DHCP discovery
- Device discovery

Switches forward broadcast frames within the local network, while routers stop broadcasts from crossing into other networks.

This boundary defines a broadcast domain.

## Why Subnetting Matters

A large network with hundreds of devices creates a large broadcast domain.

As the number of devices increases, broadcast traffic also increases.

Subnetting addresses this problem by dividing a larger network into smaller networks.

This keeps broadcasts within smaller sections of the network and reduces unnecessary traffic.

It also makes networks easier to manage and organize.

## Skills Gained

- Public and private IPv4 addressing
- Network Address Translation
- Special-use IPv4 addresses
- Classful and classless addressing
- IP address allocation
- Broadcast domains
- Network segmentation
- Subnetting fundamentals

## Assessment

### Module Quiz

First attempt: 64%

Second attempt: 82%

I improved by 18 percentage points after reviewing the questions I missed on my first attempt. I still missed two questions on the second attempt, giving me specific areas to revisit.

## Personal Takeaways

The biggest takeaway from today's session was finally understanding the practical difference between public and private IPv4 addresses.

NAT also made more sense once I connected it to how private devices access the public internet.

The discussion around broadcast domains and subnetting helped connect several networking concepts together. I now have a clearer understanding of why large networks need segmentation and how subnetting helps control broadcast traffic.

I also learned the importance of reviewing mistakes after an assessment. My score improved from 64% to 82% after going back through the questions I missed.

Now diving fully into Internet Protocol version 6 (IPv6).
