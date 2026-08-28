# Networking Basics: NAT and ARP

## Overview

Today's session was an interesting one, and I actually finished Module 12 before moving into Module 13.

Module 12 focused on Network Address Translation (NAT), including how private devices communicate with the public internet. I also moved into Module 13, which introduced the relationship between IP addresses and MAC addresses and how ARP helps devices find the correct MAC address.

## Learning Objectives

By completing these modules, I was able to:

- Understand how Network Address Translation works.
- Explain how private IP addresses communicate with the internet.
- Observe NAT translations using Packet Tracer simulation mode.
- Understand the relationship between IP and MAC addresses.
- Explain the purpose of ARP.
- Understand how devices communicate with local and remote networks.

## Network Address Translation (NAT)

NAT explains how a device using a private IP address such as:

192.168.1.15

can communicate with the public internet even though private addresses are not globally routable.

The router performs the translation between the private and public addresses.

When traffic leaves the local network, the router replaces the private source IP address with a public IP address and records the translation in a NAT table.

When the response returns, the router checks its translation table and sends the traffic back to the correct device on the private network.

This process happens without the user having to manage the translation manually.

## Packet Tracer NAT Practical

For the practical task, I configured PCs on a wireless router using DHCP and used Packet Tracer's Simulation Mode to observe NAT in action.

I:

1. Connected the PCs to the wireless router.
2. Configured DHCP for the devices.
3. Generated an HTTP request.
4. Followed the packet through the network using Simulation Mode.
5. Examined the packet headers as they crossed the network.
6. Observed the source IP address change from a private address to a public address.
7. Tracked the response back to the original device.

Seeing the private IP address change to a public address during the transmission made the concept much easier to understand than reading about it alone.

## Troubleshooting Experience

I made a small configuration mistake during the simulation.

I accidentally entered the source port number, 1000, into the source IP address field.

The error appeared immediately, and I realized I had placed the value in the wrong field. After correcting it, the simulation continued normally.

It was a small mistake, but it reinforced the importance of paying attention to configuration fields instead of rushing through a task.

## A Small Packet Tracer Observation

I also noticed something I had not paid attention to before.

The green link indicator beside a connected PC points in different directions depending on the configuration:

- Downward for static IP configuration
- Upward for DHCP

It is a small visual detail, but practical work makes it easier to notice things like this.

## Module 12 Assessment

### Module 12 Quiz

Score: 82% ✅

I completed the quiz on my first attempt, answering 9 out of 11 questions correctly.

## Module 13: IP and MAC Addresses

After completing Module 12, I moved into Module 13, which introduced how IP addresses and MAC addresses work together.

An IP address identifies the logical destination of traffic.

A MAC address identifies the network interface responsible for receiving the frame on the local network.

Both addresses work together to deliver data to the correct destination.

## Local and Remote Communication

When the destination device is on the same local network, the source device needs the destination device's MAC address to deliver the Ethernet frame.

When the destination is on a different network, the source device sends the frame to the MAC address of the default gateway instead.

The router then forwards the packet toward the remote network.

This helped me understand the different roles of IP and MAC addresses during network communication.

## Address Resolution Protocol (ARP)

ARP is responsible for finding the MAC address associated with an IPv4 address on the local network.

When a device knows the destination IP address but does not know its corresponding MAC address, it uses ARP to discover it.

The basic process is:

1. The device checks whether it already knows the MAC address.
2. If it does not, it sends an ARP request.
3. The device with the matching IP address responds with its MAC address.
4. The source device uses the MAC address to construct the Ethernet frame.

## Skills Gained

- Network Address Translation
- NAT table fundamentals
- Packet Tracer Simulation Mode
- DHCP configuration
- Packet header analysis
- IP and MAC addressing
- ARP fundamentals
- Local and remote network communication
- Basic network troubleshooting

## Assessment

### Module 12 Quiz

Score: 82% ✅

First attempt: 82%

Questions: 11

Incorrect: 2

### Module 13

Theory completed.

Packet Tracer practical: Pending.

## Personal Takeaways

Today's practical work reinforced why I enjoy learning networking through hands-on exercises.

Seeing NAT translate a private IP address into a public address inside Packet Tracer made something I had previously understood in theory much clearer.

The configuration mistake with the source port also reminded me that small errors often come from rushing. Reading the field labels carefully matters, especially when working with packet details.

Module 13 then connected IP addressing with MAC addressing. Understanding why a device communicates directly with a destination MAC address on the local network but uses the router's MAC address for remote destinations helped bring the relationship between Layer 2 and Layer 3 into clearer focus.

I completed the theory for Module 13 but stopped before the practical task so I could give the Packet Tracer exercise proper attention.

I'll pick up the practical tomorrow with fresh focus.
