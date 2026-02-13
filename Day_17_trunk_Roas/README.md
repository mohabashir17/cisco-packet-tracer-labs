# Day 17 – VLANs, Trunks, and Router-on-a-Stick

## Objective
Configure VLANs with trunking between switches and a router-on-a-stick setup
so all PCs in different VLANs can communicate.

---

## Lab Description
In this lab:

- SW1 and SW2 connect multiple VLANs (Engineering, HR, Sales)  
- PC interfaces configured as **access ports** in their VLAN  
- Connection between SW1 and SW2 configured as a **trunk**, carrying only necessary VLANs  
- Unused VLAN assigned as the **native VLAN**  
- SW2 connected to R1 using **router-on-a-stick**, with R1 subinterfaces assigned the **last usable IP** of each subnet  
- Connectivity tested by pinging all PCs

---

## Approach
Steps followed:

1. Configure PC ports on SW1 and SW2 as access ports in correct VLANs  
2. Configure trunk between SW1 and SW2, allow necessary VLANs, set unused VLAN as native  
3. Create VLANs on both switches as needed  
4. Configure router-on-a-stick subinterfaces on R1 with last usable IPs  
5. Test connectivity between all PCs to verify inter-VLAN routing

---

## Configuration Summary
* VLANs created and assigned to PC ports  
* SW1–SW2 trunk configured with allowed VLANs and native VLAN  
* Router-on-a-stick subinterfaces configured on R1  
* Verified PC-to-PC connectivity across VLANs using ping

---

## What I Understood Overall
* Trunks allow multiple VLANs to pass between switches  
* Unused VLAN as native VLAN prevents VLAN mismatches  
* Router-on-a-stick enables inter-VLAN communication through a single router interface  
* PCs in different VLANs rely on R1’s subinterfaces to communicate  
* Proper VLAN creation on all switches is crucial for connectivity

---

## Author
Mohamed
