# Day 12 – Life of a Packet (MAC Address Tracking Across Multiple Routers)

## Objective
The objective of this lab is to understand the **Life of a Packet** by tracking the
**source and destination MAC addresses** as a packet travels:

- From a **PC in one network**
- To a **PC in another network**
- Through **three routers**

The focus is on observing how **MAC addresses change at each hop**, while the IP
addresses remain the same end-to-end.

---

## Lab Topology Overview
- Source PC in Network A
- Destination PC in Network B
- Three routers connecting the two networks

Each router represents a new hop where the Ethernet frame is rebuilt with new MAC
addresses.

---

## Approach Used
To answer the lab question and identify the MAC addresses at each hop, I manually
verified the MAC addresses on:

- The source PC
- Each router interface involved in forwarding the packet
- The destination PC’s default gateway

---

## Steps Performed

### 1️⃣ Identify Source PC MAC Address
On the source PC, I used:

```bash
ipconfig /all

### 1️⃣ Identify Destination router interface MAC Address
On the Destination router, I used:

```bash
show interface _interface_

