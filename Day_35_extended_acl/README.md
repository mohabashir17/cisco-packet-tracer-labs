# Day 35 – Extended ACLs

## Objective
Practice configuring **Extended ACLs** (named and numbered) to control traffic based on source, destination, and service.

---

## Lab Requirements
- Hosts in **172.16.2.0/24** cannot communicate with **PC1**  
- Hosts in **172.16.1.0/24** cannot access **DNS service on SRV1**  
- Hosts in **172.16.2.0/24** cannot access **HTTP/HTTPS services on SRV2**

---

## Approach
- Configured **named extended ACL** to block 172.16.2.0/24 to PC1  
- Configured **numbered extended ACL** to block other restricted traffic (DNS, HTTP/HTTPS)  
- Applied ACLs to the correct interfaces in the proper direction  
- Verified ACL functionality using `show access-lists` to check matches  
- Tested connectivity to confirm allowed traffic was unaffected

---

## What I Understood
- Extended ACLs filter traffic by **source, destination, and protocol/service**  
- **Named ACLs** are easier to manage; **numbered ACLs** are faster to type  
- ACL placement is critical — usually applied close to the source for extended ACLs  
- `show access-lists` helps verify which traffic is matched or permitted  
- Proper ACL design ensures network security without blocking legitimate traffic

---

## Author
Mohamed
