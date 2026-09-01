# Networking Basics: MAC and IP Addressing with ARP

## Overview

Truly, when they say practice makes perfect, it isn't a cliché. Today's practical made that obvious.

I finished Module 13, which brought together the concepts of MAC and IP addressing, how they work together, and how ARP helps devices determine the MAC address associated with an IP address.

The practical work in Packet Tracer also gave me the opportunity to observe how Layer 2 and Layer 3 addressing behave when communicating with devices on both local and remote networks.

## Learning Objectives

By completing this module, I was able to:

- Understand the relationship between MAC and IP addresses.
- Differentiate between Layer 2 and Layer 3 addressing.
- Understand how local and remote communication differ.
- Explain how ARP maps IP addresses to MAC addresses.
- Understand broadcast domains.
- Observe MAC and IP addresses during packet transmission.
- Use Packet Tracer Simulation Mode to analyze network traffic.

## MAC and IP Addresses

Every network-connected device uses both a MAC address and an IP address for network communication.

A MAC address is assigned to the device's Network Interface Controller (NIC) and identifies the network interface at Layer 2.

An IP address provides logical addressing at Layer 3 and is assigned based on the network the device is connected to.

The two addresses work together, but they serve different purposes.

## Local Network Communication

When sending data to a device on the same local network, the Ethernet frame is addressed to the destination device's MAC address.

The destination IP address identifies the intended device at Layer 3, while the destination MAC address identifies the network interface that should receive the Ethernet frame.

## Remote Network Communication

When sending data to a device on a remote network, the Ethernet frame is initially addressed to the MAC address of the default gateway.

The default gateway becomes the first hop toward the remote destination.

As the packet travels through routers:

- Layer 3 IP addresses remain unchanged from source to destination.
- Layer 2 MAC addresses change from hop to hop.

Each router removes the incoming Layer 2 frame and creates a new frame for the next network.

This helped me understand how IP addresses provide end-to-end logical addressing while MAC addresses handle communication across each individual network link.

## Address Resolution Protocol (ARP)

Address Resolution Protocol (ARP) is used when a device knows the destination IP address but does not know the corresponding MAC address.

The process works as follows:

1. The device checks its ARP table for the required IP-to-MAC mapping.
2. If the mapping is not available, it sends an ARP request as a broadcast.
3. Devices on the local network receive the request.
4. The device with the requested IP address responds with its MAC address.
5. The requesting device stores the information in its ARP table for future communication.

ARP allows IPv4 devices to determine the Layer 2 address needed to deliver an Ethernet frame.

## Broadcast Domains

Switches and routers handle broadcast traffic differently.

A switch floods a broadcast frame out of all applicable ports except the port where the frame was received.

A router does not forward the broadcast into another network.

This creates a boundary known as a broadcast domain.

Understanding this helped connect ARP broadcasts with the role routers play in separating networks.

## Packet Tracer Practical

For the practical task, I used Packet Tracer's Simulation Mode to observe the concepts from the module.

I tested communication by pinging devices on both local and remote networks.

The simulation allowed me to inspect:

- Source IP address
- Destination IP address
- Source MAC address
- Destination MAC address
- Packet movement between devices
- Changes in Layer 2 addressing across routers

Observing the traffic directly made the relationship between MAC and IP addressing much clearer.

## Troubleshooting Experience

Getting the local network's Layer 2 and Layer 3 addressing required a little more attention.

While working with the ping simulation, I accidentally clicked the ping button twice. Since I was used to terminating commands in a real terminal, I also pressed Ctrl + C.

The command responded, but the PDU changed color midway and became stuck.

After fixing the issue, I repeated the ping and successfully collected the required information, including the source and destination IP and MAC addresses.

It was another reminder that Packet Tracer does not always behave exactly like a real terminal environment.

## Assessment

### Module 13 Quiz

Questions: 12

Score: 75%

I missed 3 questions.

Interestingly, one of the questions included a note directing me to refer to the Packet Tracer Skills Activity. That was also one of the questions I answered incorrectly.

It showed me that practical activities are sometimes directly connected to the assessment, so understanding the lab itself matters just as much as studying the theory.

## Skills Gained

- MAC addressing
- IP addressing
- Layer 2 and Layer 3 communication
- Local network communication
- Remote network communication
- Address Resolution Protocol
- ARP tables
- Broadcast domains
- Packet Tracer Simulation Mode
- Packet analysis
- Basic network troubleshooting

## Personal Takeaways

Today's module brought several networking concepts together.

I had already learned about IP addresses, MAC addresses, default gateways, and broadcast traffic separately. Module 13 helped me understand how they work together during actual communication.

The Packet Tracer practical was especially useful because I was able to watch the packet move through the network and inspect the addresses involved.

The difference between local and remote communication also became clearer. A local frame is addressed directly to the destination MAC address, while communication with a remote network initially uses the default gateway's MAC address.

The ARP process tied everything together by explaining how a device finds the MAC address associated with an IPv4 address.

The 75% quiz score also showed me an area to improve. Since one of the questions specifically pointed toward the Packet Tracer Skills Activity, I'll pay closer attention to the practical details when reviewing future modules.

Truly, today's practical reinforced the value of learning by doing.
