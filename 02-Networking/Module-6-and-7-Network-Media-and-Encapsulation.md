# Networking Basics - Modules 6 & 7: Network Media and Encapsulation

## Overview

These modules focused on two essential networking concepts: how data physically travels across a network and how data is prepared for transmission using Ethernet frames.

The material reinforced concepts I had previously studied during my undergraduate Data Communication and Networking course while introducing additional detail on Ethernet frame structure and switch operation.

---

## Learning Objectives

By completing these modules, I was able to:

- Differentiate between common network transmission media.
- Understand when to use copper, fibre optic, or wireless communication.
- Explain the process of data encapsulation.
- Identify the components of an Ethernet frame.
- Describe how switches forward traffic using MAC address tables.

---

## Network Media

Network media provides the communication path through which data travels between devices.

### Copper Cabling

Copper cables transmit data using electrical signals.

Common types include:

- Twisted Pair (UTP/STP)
- Coaxial Cable

Typical uses:

- Ethernet LAN connections
- Cable television networks
- Broadband Internet services

Advantages:

- Low cost
- Easy installation
- Widely available

Limitations:

- Susceptible to electromagnetic interference
- Limited transmission distance

---

### Fibre Optic Cable

Fibre optic cables transmit data as pulses of light.

Advantages:

- Very high bandwidth
- Long-distance communication
- Immune to electromagnetic interference
- Greater security against signal interception

Common uses:

- Internet backbone infrastructure
- Data centres
- Enterprise networks

---

### Wireless Media

Wireless communication transmits data using radio waves.

Examples include:

- Wi-Fi
- Cellular Networks
- Bluetooth

Advantages:

- Mobility
- Flexible deployment
- Reduced cabling requirements

Limitations:

- Signal interference
- Reduced range
- Security considerations

---

## Choosing the Right Medium

The choice of transmission media depends on several factors:

- Distance
- Required bandwidth
- Installation cost
- Environmental conditions
- Reliability requirements

---

## Encapsulation

Encapsulation is the process of preparing data for transmission across a network.

Each networking layer adds its own information to the original data before passing it to the next layer.

This process is similar to placing a letter inside an addressed envelope before mailing it.

---

## Ethernet Frames

On Ethernet networks, encapsulated data is carried inside an Ethernet frame.

A typical Ethernet frame contains:

- Destination MAC Address
- Source MAC Address
- Type/Length Field
- Payload (Data)
- Frame Check Sequence (FCS)

The Frame Check Sequence helps detect transmission errors.

---

## MAC Addresses

A MAC (Media Access Control) address is a unique hardware identifier assigned to a network interface.

Switches use MAC addresses to determine where Ethernet frames should be forwarded.

---

## How Network Switches Work

Switches build a MAC Address Table by learning which devices are connected to each port.

When a frame arrives:

1. The switch reads the destination MAC address.
2. It checks its MAC Address Table.
3. The frame is forwarded only to the correct destination port.

This approach significantly reduces unnecessary network traffic compared to Ethernet hubs, which broadcast data to every connected device.

---

## Skills Gained

- Network media selection
- Ethernet fundamentals
- Data encapsulation
- Ethernet frame structure
- MAC addressing
- Layer 2 switching concepts

---

## Assessment

### Module 6 Quiz

Score: **100%**

### Module 7 Quiz

Score: **82%**

### Checkpoint Assessment

- Attempt 1: 45%
- Attempt 2: 57%
- Attempt 3: 71% ✅

---

## Personal Takeaways

Module 6 felt familiar because it closely aligned with concepts covered during my undergraduate networking coursework. Revisiting these topics helped reinforce my understanding of transmission media and their practical applications.

Module 7 introduced a deeper understanding of how Ethernet networks operate behind the scenes. Learning how switches build MAC address tables and forward traffic efficiently provided valuable insight into how modern local area networks reduce unnecessary traffic and improve performance.

The checkpoint assessment required several attempts before passing, reinforcing the importance of reviewing weak areas rather than moving on too quickly. Revisiting the material resulted in a much stronger understanding of Ethernet switching and frame encapsulation.
