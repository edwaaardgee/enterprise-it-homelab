# DHCP Configuration

## Overview

This lab demonstrates the configuration of Dynamic Host Configuration Protocol (DHCP) on a Windows Server 2022 Domain Controller. DHCP was configured to automatically assign IP addresses and network settings to domain-joined clients.

## Configuration Details

| Setting          | Value           |
| ---------------- | --------------- |
| DHCP Server      | DC01            |
| Scope Name       | Corporate LAN   |
| Network          | 192.168.10.0/24 |
| Start IP Address | 192.168.10.100  |
| End IP Address   | 192.168.10.200  |
| Subnet Mask      | 255.255.255.0   |
| Default Gateway  | 192.168.10.1    |
| DNS Server       | 192.168.10.10   |
| Domain Name      | gallegos.local  |
| Lease Duration   | 8 Days          |

## Validation

The DHCP configuration was verified by obtaining a DHCP-assigned IP address on CLIENT01.

Commands used:

```cmd
ipconfig /release
ipconfig /renew
ipconfig /all
```

Verification confirmed:

* Automatic IP address assignment
* Correct subnet mask
* Correct default gateway
* Correct DNS server assignment
* Proper communication with the domain controller

## Skills Demonstrated

* DHCP Administration
* Windows Server Administration
* TCP/IP Configuration
* DNS Integration
* Enterprise Network Services
* Client Connectivity Troubleshooting

## Enterprise Concept

DHCP is a core network service used in enterprise environments to automate IP address management. By centrally assigning network configuration settings, organizations reduce administrative overhead, minimize configuration errors, and improve scalability across large numbers of devices.
