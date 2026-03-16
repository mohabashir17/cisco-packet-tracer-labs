# Day 50 – DHCP Snooping

## Objective
Practice configuring **DHCP Snooping** to protect the network from unauthorized DHCP servers.

---

## Lab Description
In this lab, **R1** was configured as the DHCP server for the LAN.  
DHCP Snooping was then enabled on **SW1 and SW2** to control which interfaces are allowed to send DHCP server messages.

Key settings:
- DHCP pool for **192.168.1.0/24**
- Addresses **192.168.1.1 – 192.168.1.9 excluded**
- Default gateway set to **R1**
- Uplink interfaces configured as **trusted ports**

After configuration, PC1 requested an IP address using **IPCONFIG /RENEW**.

---

## Approach
1. Configured R1 as the DHCP server and created the address pool.
2. Enabled DHCP Snooping on SW1 and SW2.
3. Configured the uplink interfaces toward the router as **trusted**.
4. Tested DHCP by renewing the IP address on PC1.
5. Adjusted the configuration so DHCP messages from the server were allowed through trusted ports.

---

## What I Understood
- **DHCP Snooping** is a Layer 2 security feature that filters DHCP messages from untrusted ports.
- Switch ports are **untrusted by default**, so DHCP server messages are blocked unless the port is trusted.
- **Trusted ports** should be configured on uplinks toward the legitimate DHCP server.
- DHCP Snooping helps prevent **rogue DHCP attacks**.
- Proper trust configuration is required for DHCP to work correctly.

---

## Author
Mohamed
