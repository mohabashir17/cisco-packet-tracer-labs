# Day 52 – HSRP and STP Synchronization

## Objective
Practice configuring **HSRP** for gateway redundancy and aligning it with **STP** to optimize traffic flow.

---

## Lab Description
- Two distribution switches: **DSW1** and **DSW2**  
- HSRP configured for gateway redundancy in multiple VLANs  
- STP tuned to match HSRP roles for efficient Layer 2 forwarding  

Configuration goals:
- **VLAN 10**
  - DSW1 → HSRP Active & STP Root  
  - DSW2 → HSRP Standby & STP Secondary  

- **VLAN 20**
  - DSW2 → HSRP Active & STP Root  
  - DSW1 → HSRP Standby & STP Secondary  

---

## Approach
1. Configured HSRP on both switches for each VLAN  
2. Assigned active and standby roles based on VLAN requirements  
3. Tuned STP root bridge priorities to match HSRP roles  
4. Verified redundancy and proper traffic flow  

---

## What I Understood
- **HSRP** provides default gateway redundancy for hosts  
- **STP** controls Layer 2 path selection  
- Aligning HSRP active with STP root avoids inefficient traffic paths  
- Load balancing can be achieved by splitting roles across VLANs  
- Proper design improves performance and redundancy  

---

## Author
Mohamed
