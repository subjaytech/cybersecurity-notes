# Networking Basics: IPv6 Fundamentals and Transition Mechanisms

## Overview

Today's module focused on why IPv6 was developed, the limitations of IPv4, IPv6 addressing, and the techniques used to support the transition from IPv4 to IPv6.

The session made it clear that IPv6 became necessary because the number of internet-connected devices continued to grow while IPv4 address space remained limited. I also learned how IPv6 improves addressing and introduces features designed to simplify network configuration and communication.

## Learning Objectives

By completing this module, I was able to:

- Explain why IPv6 was developed.
- Understand the limitations of the 32-bit IPv4 address space.
- Compare IPv4 and IPv6 address sizes.
- Explain the role of ICMPv6 in IPv6 networks.
- Identify the three main IPv4-to-IPv6 transition techniques.
- Understand the structure of an IPv6 address.
- Apply IPv6 address compression rules.
- Read and write IPv6 addresses using hexadecimal notation.

## Why IPv6 Was Developed

IPv4 uses 32-bit addresses, providing approximately 4.3 billion possible addresses.

With the rapid growth of internet-connected devices, including smartphones, computers, IoT devices, smart appliances, and biomedical equipment, IPv4 address space became insufficient.

Private addressing and Network Address Translation (NAT) helped extend the usefulness of IPv4, but they did not solve the underlying address shortage.

NAT also affects end-to-end communication and introduces additional processing between devices.

IPv6 was developed to provide a much larger address space and support the continued growth of internet-connected devices.

## IPv6 Address Space

IPv6 uses 128-bit addresses instead of the 32-bit addresses used by IPv4.

This provides approximately 340 undecillion possible addresses.

The difference in address space is significant:

- IPv4: 32-bit address
- IPv6: 128-bit address

The much larger address space provides enough addresses for the continued expansion of the internet and connected devices.

## ICMPv6

IPv6 uses Internet Control Message Protocol version 6 (ICMPv6) for network control and diagnostic functions.

ICMPv6 also supports important IPv6 functions such as Neighbor Discovery and address autoconfiguration.

This allows IPv6 devices to discover neighboring devices and obtain network configuration information without relying on the same mechanisms used by IPv4.

## IPv4 and IPv6 Coexistence

The transition from IPv4 to IPv6 does not happen instantly.

Both protocols are expected to coexist for an extended period, which requires transition mechanisms.

The three main approaches are:

### Dual Stack

Dual stack allows a device to run IPv4 and IPv6 at the same time.

The device communicates using whichever protocol is supported by the destination network or service.

### Tunneling

Tunneling allows IPv6 packets to travel across an IPv4 network.

The IPv6 packet is encapsulated inside an IPv4 packet so it can pass through infrastructure that does not support native IPv6.

### Translation

Translation converts communication between IPv4 and IPv6.

One example is NAT64, which allows IPv6-only devices to communicate with IPv4 resources by translating between the two protocols.

## IPv6 Address Structure

IPv6 addresses use hexadecimal notation instead of the decimal notation used by IPv4.

A complete IPv6 address contains 128 bits divided into eight groups.

Each group contains four hexadecimal digits and is known as a hextet.

A full IPv6 address therefore contains:

- 8 hextets
- 4 hexadecimal digits per hextet
- 128 bits in total

For example:

2001:0db8:0000:0000:0000:ff00:0042:8329

## IPv6 Address Compression

IPv6 addresses are long, so IPv6 provides rules for shortening their representation.

### Removing Leading Zeros

Leading zeros within a hextet can be removed.

For example:

00ab becomes ab

Therefore:

2001:0db8:0000:0000:0000:ff00:0042:8329

can first be shortened to:

2001:db8:0:0:0:ff00:42:8329

### Using Double Colon

A single consecutive sequence of zero hextets can be replaced with a double colon (::).

For example:

2001:db8:0:0:0:ff00:42:8329

becomes:

2001:db8::ff00:42:8329

The double colon shortcut is only used once in an IPv6 address. Using it more than once would make it impossible to determine how many zero hextets each occurrence represents.

## Skills Gained

- IPv4 and IPv6 comparison
- Understanding IPv4 address exhaustion
- IPv6 addressing
- ICMPv6 fundamentals
- IPv4-to-IPv6 transition techniques
- Dual-stack networking
- IPv6 tunneling
- IPv6 translation
- IPv6 hexadecimal notation
- IPv6 address compression

## Assessment

### Module Quiz

First attempt: 64%

Second attempt: 100% ✅

I improved my score from 64% to 100% after revisiting the module and reviewing the concepts I had initially missed.

## Personal Takeaways

The biggest takeaway from this module was understanding why IPv6 became necessary. IPv4 address exhaustion is the main reason, but the continued growth of mobile devices, IoT systems, and other connected technologies made a larger address space essential.

The 128-bit IPv6 address space also helped me understand how differently IPv6 approaches addressing compared to IPv4.

The address compression rules took some time to get used to, especially the use of the double colon. Once I understood how leading zeros and consecutive zero hextets are handled, reading IPv6 addresses became much easier.

My quiz result also showed the value of revisiting the material. I started with 64% and returned to score 100% after reviewing the module.

Next, I’ll continue building my understanding of IPv6 and how it operates in modern networks.
