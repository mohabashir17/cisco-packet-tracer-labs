# Day 33 – IPv6 Static Routing and SLAAC

## Objective
Enable IPv6 routing on routers, configure PCs with SLAAC, and implement static
routes so PCs in different networks can communicate, with a backup path via R2.

---

## Lab Description
In this lab:

- Routers already have pre-configured IPv6 addresses  
- Serial connections use **link-local addresses** only  
- PC1 and PC2 will receive IPv6 addresses using **SLAAC**  
- Static routes configured on routers allow communication between PCs  
  - Primary path  
  - Backup path via R2  

---

## Approach
Steps followed:

1. Enable IPv6 routing on all routers  

2. Configure PCs using **SLAAC** and check the IPv6 address automatically assigned  

3. Configure static routes on routers:  
- **Recursive static route** → uses next-hop IP address  
- **Fully specified static route** → specifies exit interface and next-hop  
Primary path points directly, backup path via R2

4. Verify connectivity by pinging between PC1 and PC2  

---

## Configuration Summary
* IPv6 routing enabled with `ipv6 unicast-routing`  
* PCs configured with IPv6 via SLAAC  
* Static routes implemented for primary and backup paths  
* Tested connectivity between PCs successfully  

---

## What I Understood Overall
* SLAAC allows PCs to automatically configure IPv6 addresses using router advertisements  
* IPv6 routing must be enabled on routers (`ipv6 unicast-routing`)  
* Recursive and fully specified static routes control traffic flow and backups  
* Link-local addresses are essential for routing over point-to-point links  
* Proper static route planning ensures reliable network communication  

---

## Author
Mohamed
