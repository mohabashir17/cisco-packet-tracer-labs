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

1. Enable Layer 3 routing on multilayer switch  

2. Convert switch port to Layer 3 routed port  

3. Configure Layer 3 point-to-point link between SW2 and R1  

4. Configure default route on SW2 using R1 as next hop  

5. Create SVIs on SW2 (one per VLAN)  

6. Assign last usable IP of each subnet to each SVI  

7. Test inter-VLAN connectivity using ping  

8. Test Internet connectivity by pinging 1.1.1.1  

---

## Configuration Summary
* Enabled routing using `ip routing`  
* Configured routed port using `no switchport`  
* Configured SVIs using `interface vlan <vlan-number>`  
* Configured default route on SW2  
* Verified inter-VLAN communication  
* Verified Internet connectivity  

---

## What I Understood Overall
* Multilayer switches can route using SVIs  
* `ip routing` enables Layer 3 functionality on switch  
* `no switchport` converts a Layer 2 port into a Layer 3 routed port  
* SVIs act as gateways for VLANs  
* Layer 3 switching is more scalable and faster than router-on-a-stick  
* Default route allows VLAN networks to reach external networks  

---

## Author
Mohamed
