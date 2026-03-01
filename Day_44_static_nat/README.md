# Day 44 – Static NAT Configuration

## Objective
Practice configuring **Static NAT** to allow internal hosts to communicate with external networks.

---

## Lab Description
- Tested connectivity from internal network to external IP (8.8.8.8)  
- Configured static NAT on R1  
- Mapped internal PCs to public 100.0.0.x/24 addresses  
- Verified NAT translations after generating traffic  
- Cleared NAT table and observed remaining entries  

---

## Approach
1. Attempted initial ping to 8.8.8.8 (before NAT configuration)  
2. Configured inside and outside NAT interfaces on R1  
3. Created static NAT mappings for PC1, PC2, and PC3  
4. Retested connectivity to external IP and domain name  
5. Verified NAT translations table  
6. Cleared NAT entries and observed static mappings remaining  

---

## What I Understood
- Static NAT creates a permanent one-to-one mapping between private and public IP addresses  
- Inside and outside interfaces must be defined correctly  
- Without NAT, private IP addresses cannot reach the public Internet  
- Static NAT entries remain even after clearing dynamic translations

---

## Author
Mohamed
