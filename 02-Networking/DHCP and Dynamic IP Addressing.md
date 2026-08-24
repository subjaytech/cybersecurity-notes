# Networking Basics: DHCP and Dynamic IP Addressing

## Overview

Today's lesson focused on static and dynamic IP addressing, DHCP, and the practical process of automatically assigning network configuration to devices.

The practical side of the module stood out to me again. Using Packet Tracer gave me the opportunity to configure DHCP on a wireless router and verify how devices receive their network settings automatically.

## Learning Objectives

By completing this module, I was able to:

- Differentiate between static and dynamic IP addressing.
- Understand the purpose of DHCP.
- Configure DHCP on a wireless router.
- Configure PCs to obtain IP addresses automatically.
- Understand the four-step DHCP process.
- Test connectivity between devices after DHCP configuration.

## Static and Dynamic IP Addressing

Static IP addressing requires network settings to be configured manually on a device.

Dynamic IP addressing uses DHCP to automatically provide the device with the required network configuration.

This typically includes:

- IP address
- Subnet mask
- Default gateway

DHCP makes network configuration easier, especially when dealing with multiple devices.

## DHCP

Dynamic Host Configuration Protocol (DHCP) automatically assigns IP configuration to devices on a network.

Instead of manually entering network information on every device, a DHCP server provides the required settings automatically.

This reduces configuration errors and makes managing larger networks more efficient.

## Packet Tracer Practical

I used Cisco Packet Tracer to configure DHCP on a wireless router.

The practical task involved:

1. Connecting three PCs to the wireless router.
2. Changing the router's default IP address.
3. Configuring the DHCP address range.
4. Switching each PC from static configuration to DHCP.
5. Confirming that each PC received the correct IP configuration automatically.
6. Testing connectivity between the devices.

The entire practical task was completed successfully.

## The DHCP Four-Step Process

The quiz focused heavily on the four-step DHCP process, known as DORA:

### Discover

The client broadcasts a DHCP Discover message to find an available DHCP server.

### Offer

The DHCP server responds with a DHCP Offer containing an available IP configuration.

### Request

The client sends a DHCP Request to indicate which offered configuration it wants to use.

### Acknowledge

The DHCP server sends a DHCP Acknowledgment, confirming the IP configuration assigned to the client.

The sequence is:

Discover → Offer → Request → Acknowledge

Understanding this process helped connect the theory behind DHCP with the practical configuration I performed in Packet Tracer.

## Skills Gained

- Static and dynamic IP addressing
- DHCP configuration
- Wireless router configuration
- Automatic IP address assignment
- DHCP DORA process
- Packet Tracer configuration
- Network connectivity testing
- Basic network troubleshooting

## Assessment

### Practical Task

Result: 100% ✅

I successfully configured DHCP on the wireless router, configured all three PCs to obtain their addresses automatically, and confirmed connectivity between the devices.

### Module Quiz

First attempt: 36%

Second attempt: 64%

Third attempt: 73%

Final attempt: 100% ✅

The first attempt was my lowest quiz score so far. I reviewed the module videos again and kept working through the questions until I fully understood the DHCP process.

## Personal Takeaways

Today's lesson reinforced why I enjoy the practical side of networking.

Configuring DHCP in Packet Tracer and seeing the PCs automatically receive their network settings made the concept much easier to understand.

The quiz was a different experience. Despite watching both videos twice, I scored 36% on my first attempt. Instead of moving on, I went back through the material and kept attempting the quiz until I reached 100%.

The biggest takeaway for me was the connection between configuration and theory. I could configure DHCP successfully in Packet Tracer, but understanding the DORA process required additional review.

Overall, this was another interesting hands-on networking session, and I look forward to more practical work.
