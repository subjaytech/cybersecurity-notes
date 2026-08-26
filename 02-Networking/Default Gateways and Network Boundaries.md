# Networking Basics: Default Gateways and Network Boundaries

## Overview

Today's session started with a checkpoint exam covering Modules 1 through 11 before moving into Module 12, which focuses on gateways and network boundaries.

The checkpoint revisited several concepts from the previous modules, including DHCP. Module 12 then introduced the role of the default gateway and how devices determine whether traffic needs to remain within the local network or leave it.

## Checkpoint Exam

The checkpoint exam covered material from Modules 1 through 11 and contained three questions.

One of the questions focused on the DHCP process, which I now remember as DORA:

- Discover
- Offer
- Request
- Acknowledge

### Assessment

First attempt: 50%

Second attempt: 80% ✅

I fell below the pass mark on my first attempt, reviewed the material, and returned with a stronger score on the second attempt.

## Module 12: Gateways and Network Boundaries

Module 12 focused on the role of gateways and how devices communicate beyond their local network.

The concept that stood out most was the default gateway.

## Default Gateway

A default gateway is the device a host uses when it needs to send traffic to a destination outside its own local network.

Usually, the default gateway is the router interface connected to the local network.

Before sending traffic, a host determines whether the destination belongs to its own network.

If the destination is local, the device communicates directly within the local network.

If the destination is outside the local network, the device forwards the traffic to its default gateway.

The basic process is:

1. The host checks the destination IP address.
2. It determines whether the destination belongs to the local network.
3. If the destination is local, traffic stays within the local network.
4. If the destination is remote, traffic is sent to the default gateway.
5. The router then forwards the traffic toward its destination.

## Why the Default Gateway Matters

One thing that stood out to me is how important a single configuration value is.

If a device has the wrong default gateway address, it might still communicate with other devices on its local network, but it will not be able to reach destinations outside that network.

Even a small configuration error, such as entering the wrong final digit of the gateway address, can prevent external communication while the rest of the IP configuration appears correct.

This made the role of the default gateway much easier to understand.

## Network Boundaries

The router also represents an important boundary between networks.

A local network might use private IP addresses internally, while the router provides the connection toward external networks and the internet.

DHCP often provides hosts with the correct default gateway automatically, reducing the need for manual configuration.

## Practical Work

I started the Module 12 reading and reached the point where the next task is the Packet Tracer practical.

Rather than rush through it, I decided to pause and give the practical task my full attention.

The practical work will provide an opportunity to apply the concept of default gateways in an actual network configuration.

## Skills Gained

- Understanding default gateways
- Identifying local and remote destinations
- Understanding network boundaries
- Understanding router interfaces
- DHCP gateway configuration
- Basic routing concepts
- Network troubleshooting fundamentals

## Assessment

### Checkpoint Exam

First attempt: 50%

Second attempt: 80% ✅

The checkpoint covered Modules 1 through 11 and included three questions.

### Module 12 Practical

Pending.

I paused before starting the Packet Tracer practical so I could continue with it properly in the next session.

## Personal Takeaways

Today's session connected several networking concepts I had already studied.

The DHCP process came back during the checkpoint, and remembering it as DORA made it easier to recall.

Module 12 then shifted my attention toward what happens when a device needs to communicate beyond its local network.

The default gateway stood out because it acts as the route out of the local network. Understanding how a host decides whether traffic is local or remote made the purpose of the gateway much clearer.

I also learned that a small configuration mistake in the default gateway can affect external connectivity even when the rest of the network configuration looks correct.

I stopped before the practical task so I could approach it properly instead of rushing through it.

Tomorrow, I'll finish the Module 12 Packet Tracer practical and then move straight into Module 13.
