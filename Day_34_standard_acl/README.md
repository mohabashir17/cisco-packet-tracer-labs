# Day 34 – OSPF and Standard ACLs (Numbered & Named)

## Objective
Configure OSPF for full network connectivity and implement **standard ACLs**
(numbered and named) to enforce specific network access policies.

---

## Lab Description
In this lab:

- OSPF configured on R1 and R2 for full connectivity between PCs and servers  
- Standard **numbered ACLs** configured on R1  
- Standard **named ACLs** configured on R2  

Network policies implemented:
* Only PC1 and PC3 can access 192.168.1.0/24  
* 172.16.2.0/24 cannot access 192.168.2.0/24  
* 172.16.1.0/24 cannot access 172.16.2.0/24  
* 172.16.2.0/24 cannot access 172.16.1.0/24  

---

## Approach
Steps followed:

1. Configure OSPF on R1 and R2  
2. Configure standard numbered ACLs on R1  
3. Configure standard named ACLs on R2  
4. Apply ACLs to correct interfaces and directions  
5. Test connectivity to verify ACL policies  

---

## Configuration Summary
* OSPF configured for routing between networks  
* Standard numbered ACLs configured on R1  
* Standard named ACLs configured on R2  
* ACLs applied to interfaces to enforce traffic filtering  
* Verified policies using ping tests  

---

## What I Understood Overall
* Standard ACLs filter traffic based on **source IP address only**  
* Numbered ACLs are simpler but less flexible than named ACLs  
* Named ACLs are easier to manage and modify  
* ACL placement is important for correct traffic control  
* OSPF provides routing while ACLs provide security and traffic control  
* Incorrect ACL order or placement can block valid traffic  

---

## Author
Mohamed
