# Day 18 – Inter-VLAN Routing Using Multilayer Switch (SVIs)

## Objective
Replace router-on-a-stick with Layer 3 switching using SVIs on a multilayer switch
and configure routing to allow inter-VLAN and Internet connectivity.

---

## Lab Description
In this lab:

- SW2 was replaced with a **multilayer switch**
- Existing setup from Day 17 was used (VLANs + trunk to SW1)
- ROAS between R1 and SW2 was removed
- A **Layer 3 point-to-point link** was configured between R1 and SW2
- SVIs were configured on SW2 (one per VLAN)
- Default route configured on SW2 pointing to R1
- Connectivity tested between VLANs and to the Internet (1.1.1.1)

Rules used:
* Last usable IP → Assigned to each SVI
* Default route → Points to R1 G0/0

---

## Approach
Steps followed:

1. Remove router-on-a-stick configuration  
2. Configure Layer 3 point-to-point link between SW2 and R1  
3. Configure default route on SW2 using R1 as next hop  
4. Create SVIs on SW2 (one per VLAN)  
5. Assign last usable IP of each subnet to each SVI  
6. Test inter-VLAN connectivity using ping  
7. Test Internet connectivity by pinging 1.1.1.1  

---

## Configuration Summary
* Configured Layer 3 routed link between SW2 and R1  
* Configured SVIs for each VLAN on multilayer switch  
* Configured default route on SW2  
* Verified inter-VLAN communication  
* Verified Internet connectivity  

---

## What I Understood Overall
* Multilayer switches can perform routing using SVIs  
* SVIs act as gateways for VLANs (instead of router subinterfaces)  
* Layer 3 links between router and switch improve performance  
* Default route allows internal networks to reach external networks  
* Layer 3 switching is faster and more scalable than ROAS  

---

## Author
Mohamed
