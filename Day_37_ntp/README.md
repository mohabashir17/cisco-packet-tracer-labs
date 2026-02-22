# Day 37 – NTP Configuration and Time Synchronization

## Objective
Practice configuring NTP and time synchronization across multiple routers.

---

## Lab Description
- Routing preconfigured (default route on R1, OSPF on all routers)  
- R1, R2, and R3 synchronize time using NTP  
- R1 synchronizes to an external NTP server (1.1.1.1)  
- R1 configured as **stratum 8 NTP master** for R2 and R3 with authentication  
- Hardware clock updates simulated in Packet Tracer  

---

## Approach
1. Set software clock on all routers to a specific UTC time  
2. Configured local time zones on all routers  
3. Synchronized R1 to external NTP server and verified stratum  
4. Configured R1 as NTP master and synchronized R2 and R3 using authentication  
5. Simulated updating hardware calendars (Packet Tracer limitation)  

---

## What I Understood
- NTP ensures consistent time across devices, crucial for logs and network events  
- Routers have stratum levels indicating accuracy relative to a primary source  
- Authentication improves security of NTP synchronization  
- Packet Tracer allows practicing NTP configuration even if some commands are unavailable  
- Time zone and clock configuration are essential for accurate network monitoring  

---

## Author
Mohamed
