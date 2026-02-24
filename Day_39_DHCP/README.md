# Day 39 – DHCP Configuration and Relay

## Objective
Practice configuring DHCP pools, DHCP client, and DHCP relay to automate IP address assignment.

---

## Lab Description
- R2 configured with three DHCP pools for different subnets  
- R1 configured as a DHCP client for one network  
- R1 configured as a **DHCP relay** for another subnet  
- PCs configured to request IP addresses from their DHCP servers  

---

## Approach
1. Created DHCP pools on R2 with reserved addresses, DNS, domain, and default gateways  
2. Configured R1 G0/0 as DHCP client and verified assigned IP  
3. Configured R1 as DHCP relay for 192.168.1.0/24 subnet  
4. PCs requested IP addresses via DHCP and verified proper assignment  

---

## What I Understood
- DHCP automates IP address assignment for hosts  
- DHCP relay allows clients on other subnets to obtain IP from a centralized DHCP server  
- Reserved addresses prevent conflicts with static IPs 

---

## Author
Mohamed
