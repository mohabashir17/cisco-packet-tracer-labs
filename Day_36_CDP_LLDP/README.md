# Day 36 – CDP and LLDP

## Objective
Use CDP to discover missing network information, then disable CDP and configure LLDP for neighbor discovery.

---

## Lab Description
The topology initially had **no documentation** (no interface IDs, no IP addresses labeled).  
Using discovery commands, I identified and documented:

- Interface IDs  
- Neighbor relationships  
- IP addresses  
- Connected devices  

---

## Approach

1. Used discovery commands to identify missing information:
   - `show ip interface brief`
   - `show cdp neighbors`
   - `show cdp interface`
   - Other verification commands

2. Disabled CDP on switch interfaces connected to PCs  

3. Disabled CDP globally on all network devices  

4. Enabled LLDP globally on all devices  

5. Enabled LLDP Tx/Rx on interfaces connected to other network devices  

---

## Configuration Summary
- Discovered undocumented topology information using CDP  
- Disabled CDP per-interface and globally  
- Enabled LLDP globally  
- Enabled LLDP transmit and receive on required interfaces  
- Verified neighbor relationships using LLDP  

---

## What I Understood
- CDP is Cisco proprietary and useful for topology discovery  
- `show cdp neighbors` helps identify connected devices and interfaces  
- `show ip interface brief` helps verify IP addressing quickly  
- CDP can be disabled for security reasons  
- LLDP is vendor-neutral and works across different network vendors  
- Proper documentation is critical in network management  

---

## Author
Mohamed
