# Day 15 – VLSM (Variable Length Subnet Masking)

## Objective
Apply VLSM to subnet the network 192.168.5.0/24 based on different LAN host requirements
and configure static routing so all PCs can communicate.

---

## Lab Description
In this lab, I subnetted 192.168.5.0/24 using VLSM to support:

* LAN1 → 45 hosts
* LAN2 → 64 hosts
* LAN3 → 14 hosts
* LAN4 → 9 hosts
* R1–R2 point-to-point link → 2 hosts

Rules used:
* First usable IP → PC
* Last usable IP → Router interface
* /30 subnet → Router-to-router link

---

## Approach
When performing VLSM, I followed this order:

1. Assign subnet to the **largest LAN first**
2. Then assign subnet to the **second largest LAN**
3. Continue until smallest networks are assigned
4. Point-to-point links are usually assigned last (/30)

This ensures efficient IP address usage and avoids wasting address space.

---

## Configuration Summary
* Configured router interfaces with assigned IP addresses
* Configured static routes on each router
* Verified connectivity using ping

---

## What I Understood Overall
* VLSM allows efficient use of IP address space
* Subnet planning must be done before configuration
* Always subnet from largest to smallest network
* Static routing requires correct next-hop addressing
* Incorrect subnet mask or route breaks connectivity
* Good subnet design improves scalability and management

---

## Commands Used
* `ip route`
* `ip address`
* `no shutdown`
* `interface _interface_`
* `show ip route`
* `ping`

---

## Author
Mohamed

