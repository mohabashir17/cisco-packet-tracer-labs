# Day 51 – Dynamic ARP Inspection (DAI)

## Objective
Practice configuring **Dynamic ARP Inspection (DAI)** to protect the network from ARP spoofing attacks.

---

## Lab Description
- R1 configured as the DHCP server for the network  
- DHCP Snooping enabled on **SW1 and SW2**  
- DAI configured on both switches to validate ARP packets  
- Trusted ports set for connections to routers and switches  

---

## Approach
1. Configured R1 as DHCP server with excluded addresses and default gateway  
2. Enabled DHCP Snooping on SW1 and SW2  
3. Enabled DAI on both switches  
4. Activated additional ARP validation checks  
5. Configured uplink interfaces (to routers/switches) as **trusted ports**  
6. Verified normal communication and protection against invalid ARP messages  

---

## What I Understood
- **DAI** prevents ARP spoofing by validating ARP packets  
- It relies on the **DHCP Snooping binding table** for verification  
- Untrusted ports are checked; trusted ports bypass inspection  
- Additional validation increases security (IP/MAC/ARP checks)  
- DAI helps protect against **man-in-the-middle attacks**  

---

## Author
Mohamed
