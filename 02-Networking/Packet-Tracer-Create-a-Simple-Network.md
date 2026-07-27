# Packet Tracer Lab - Create a Simple Network

## Overview

This lab introduced me to Cisco Packet Tracer and how to simulate a basic home network using both the Logical and Physical workspaces.

The objective was to build a simple network, configure end devices, obtain IP addresses using DHCP, and verify network connectivity.

---

## Learning Objectives

By completing this lab, I was able to:

- Navigate the Logical and Physical workspaces.
- Deploy network devices in Packet Tracer.
- Connect devices using the correct cable types.
- Configure hosts using DHCP.
- Verify network connectivity with command-line tools.
- Understand the role of the default gateway and subnet mask.

---

## Network Topology

Devices used:

- PC
- Laptop
- Wireless Router
- Cable Modem
- Internet (ISP)

### Network Diagram

```text
                Internet (ISP)
                      |
                 Coaxial Cable
                      |
               Cable Modem
                      |
        Copper Straight-through
                      |
             Wireless Router
              /             \
             /               \
Copper Straight-         Wireless
Through Cable           Connection
          |                  |
         PC               Laptop
```

---

## Cabling

| Connection | Cable Type |
|------------|------------|
| PC → Wireless Router | Copper Straight-through |
| Wireless Router → Cable Modem | Copper Straight-through |
| Cable Modem → ISP | Coaxial Cable |
| Laptop → Wireless Router | Wireless Connection |

---

## Laptop Wireless Configuration

To connect the laptop wirelessly:

1. Powered off the laptop.
2. Removed the wired Ethernet NIC.
3. Installed a wireless network interface card.
4. Powered the laptop back on.
5. Connected to the wireless network.

---

## IP Configuration

Both end devices obtained their network configuration automatically through DHCP.

Example configuration:

- IP Address: 192.168.0.x
- Subnet Mask: 255.255.255.0
- Default Gateway: 192.168.0.1

The configuration was verified using:

```bash
ipconfig
```

---

## Connectivity Testing

Connectivity was verified using:

```bash
ping
```

Successful ping responses confirmed that devices could communicate across the network.

---

## Key Networking Concepts

### DHCP

Automatically assigns IP addresses and other network settings to devices joining the network.

### IP Address

A unique address assigned to a device on a network.

### Subnet Mask

Determines which part of an IP address identifies the network and which part identifies the individual device.

### Default Gateway

The router responsible for forwarding traffic outside the local network.

---

## Challenge Encountered

The Packet Tracer desktop application became stuck at 50% completion and would not accept the requested IP configuration despite the network functioning correctly.

To verify the configuration, I completed the same activity using the Packet Tracer web version, where the assessment successfully recorded a score of 100%.

---

## Assessment

Packet Tracer Activity

- Score: 100%

Final Quiz

- Score: 5/5

---

## Skills Gained

- Basic network design
- Device deployment
- Cable selection
- DHCP configuration
- IP addressing
- Network verification
- Packet Tracer navigation
- Basic troubleshooting

---

## Personal Takeaways

This lab helped bridge the gap between networking theory and practical implementation.

Building the network from scratch, configuring devices, and verifying connectivity made concepts like DHCP, subnet masks, and default gateways much easier to understand than reading about them alone.

This is my first practical networking lab, and it provides a strong foundation for the networking concepts I'll continue learning throughout the Cisco Networking Academy.
