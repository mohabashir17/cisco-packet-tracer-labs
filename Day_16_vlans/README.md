# Day 16 – VLANs (VLAN Configuration & Gateway Setup)

## Objective
Configure VLANs on a switch and configure router interfaces to act as gateways
for each VLAN. Verify connectivity and observe broadcast behavior inside VLANs.

---

## Lab Description
In this lab, I configured VLANs on SW1 and connected R1 to provide gateway
addresses for each VLAN.

VLANs used:
* Engineering
* HR
* Sales

Rules used:
* PCs → Correct IP address and subnet mask
* Gateway → Last usable IP address in subnet
* One router interface → One VLAN network

---

## Approach
When configuring VLANs, I followed this order:

1. Configure IP address and subnet mask on each PC  
2. Set default gateway as **last usable IP**  
3. Connect R1 to SW1 using three interfaces (one per VLAN)  
4. Configure router interfaces with gateway IP addresses  
5. Configure switch ports into correct VLANs  
6. Name VLANs (Engineering, HR, Sales)  
7. Test connectivity using ping  
8. Test broadcast using subnet broadcast address (Simulation Mode)

---

## Configuration Summary
* Configured VLANs on switch
* Assigned switch ports to correct VLANs
* Configured router interfaces as VLAN gateways
* Verified PC-to-PC connectivity using ping
* Verified broadcast behavior using Simulation Mode

---

## What I Understood Overall
* VLANs separate networks logically at Layer 2
* Each VLAN is its own broadcast domain
* Devices in different VLANs need Layer 3 gateway to communicate
* Gateway must be in same subnet as PCs
* Broadcast traffic stays inside the VLAN
* VLAN naming improves network management and clarity


---

## Author
Mohamed
