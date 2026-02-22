# Day 38 – DNS Configuration and Name Resolution

## Objective
Practice DNS configuration and name resolution in a small network, including analysis of DNS query behavior.

---

## Lab Description
- Default route to the Internet configured on R1  
- PCs configured to use an external DNS server (1.1.1.1)  
- R1 configured with host entries for R1, PC1, PC2, and PC3  
- DNS name resolution tested from R1 and PC1 using simulation mode  

---

## Approach
1. Configured default route on R1 for Internet access  
2. Set PCs to use 1.1.1.1 as DNS server  
3. Configured R1 host entries for all local devices  
4. Verified local name resolution by pinging PC1 from R1 by name  
5. Simulated DNS queries from PC1 to external site (youtube.com) using Packet Tracer simulation mode  

---

## What I Understood
- DNS maps hostnames to IP addresses for communication  
- Host entries allow local name resolution without an external DNS server  
- Simulation mode shows the DNS query and response process  
- DNS is essential for network usability and troubleshooting  
- Packet Tracer may not support `ip dns server`, but you can still practice name resolution concepts  

---

## Author
Mohamed
