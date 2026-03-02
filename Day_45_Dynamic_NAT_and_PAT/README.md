# Day 45 – Dynamic NAT and PAT

## Objective
Practice configuring **Dynamic NAT** and **PAT (Port Address Translation)** and understand the difference between them.

---

## Lab Description
- Configured Dynamic NAT on R1  
- Created NAT pool (100.0.0.1–100.0.0.2)  
- Translated traffic from 172.16.0.0/24  
- Tested connectivity from internal PCs to the Internet  
- Switched configuration from Dynamic NAT to PAT using R1’s public IP  

---

## Approach
1. Configured inside and outside NAT interfaces  
2. Created NAT pool with two public IP addresses  
3. Mapped 172.16.0.0/24 network using Dynamic NAT  
4. Tested connectivity from PCs and observed NAT table  
   - Noticed limited pool size affected translations  
5. Cleared NAT configuration  
6. Reconfigured NAT as PAT using single public IP  
7. Retested connectivity and verified NAT translations  

---

## What I Understood
- Dynamic NAT uses a pool of public IP addresses for translation  
- If the pool is exhausted, additional hosts cannot access the Internet  
- PAT allows multiple devices to share a single public IP using port numbers  
- PAT is more scalable and commonly used in real networks  
- NAT translation tables help monitor active sessions  
- Proper inside/outside interface configuration is critical  

---

## Author
Mohamed
