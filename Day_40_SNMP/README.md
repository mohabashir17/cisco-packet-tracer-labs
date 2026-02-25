# Day 40 – SNMP Configuration and Monitoring

## Objective
Practice basic SNMP configuration and monitoring using SNMP Get and Set operations.

---

## Lab Description
- Configured SNMP communities on R1:
  - Read-only community
  - Read/write community
- Used the MIB Browser on PC1 to retrieve device information via SNMP
- Modified router configuration using an SNMP Set message

*Note: SNMP functionality is very limited in Packet Tracer.*

---

## Approach
1. Configured SNMP read-only and read/write communities on R1  
2. Used SNMP Get requests from PC1 to retrieve:
   - System uptime  
   - Configured hostname  
   - Number of interfaces  
   - Interface details  
3. Explored additional available MIB information  
4. Used SNMP Set request to change R1’s hostname  

---

## What I Understood
- SNMP allows remote monitoring and management of network devices  
- Read-only communities allow monitoring; read/write allows configuration changes  
- SNMP Get retrieves information from a device’s MIB  
- SNMP Set can modify device parameters remotely  
- SNMP is powerful but should be secured properly  
- Packet Tracer supports only basic SNMP features for practice  

---

## Author
Mohamed
