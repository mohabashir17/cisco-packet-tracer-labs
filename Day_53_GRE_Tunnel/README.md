# Day 53 – GRE Tunnel and OSPF

## Objective
Practice configuring a **GRE tunnel** between routers and running **OSPF** over the tunnel for end-to-end connectivity.

---

## Lab Description
- Two routers: **R1** and **R2** connected via a GRE tunnel  
- PCs on either side of the tunnel require connectivity  
- OSPF configured on tunnel interfaces to exchange routes  

---

## Approach
1. Configured a GRE tunnel between R1 and R2 with appropriate tunnel source and destination  
2. Assigned IP addresses to tunnel interfaces  
3. Configured OSPF on tunnel interfaces to advertise networks  
4. Verified that PC1 and PC2 could ping each other across the tunnel  

---

## What I Understood
- **GRE tunnels** encapsulate packets to create a logical point-to-point link over an IP network  
- OSPF can run over the tunnel to dynamically share routes  
- Tunnel interfaces must have IP addresses and matching source/destination  
- Proper routing ensures connectivity between remote networks  
- GRE is useful when direct Layer 2 connections are not available  

---

## Author
Mohamed
