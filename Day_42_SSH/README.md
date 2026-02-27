# Day 32 – SSH Configuration and Switch Security

## Objective
Configure basic switch settings, secure console access, and enable secure remote management using SSH.

---

## Lab Description
- Newly added SW2 configured from console via Laptop1  
- Basic device configuration applied (hostname, enable secret, local user)  
- VLAN1 SVI configured with management IP address  
- Default gateway set for remote connectivity  
- Console and SSH access secured  
- Remote SSH access restricted to PC1 only  

---

## Approach
1. Performed initial configuration through console connection  
2. Configured management IP on VLAN1 SVI and default gateway  
3. Secured console access using local authentication and exec timeout  
4. Configured SSH:
   - Set domain name  
   - Generated 2048-bit RSA keys  
   - Allowed SSH only (disabled Telnet)  
   - Used local user authentication  
   - Set exec timeout to 5 minutes  
5. Applied access control to allow SSH access from PC1 only  

---

## What I Understood
- SSH provides encrypted remote access to network devices  
- RSA keys are required to enable SSH  
- Local user authentication improves security  
- Exec timeout prevents unattended sessions  
- Management VLAN and default gateway are required for remote access  
- Access should be restricted to trusted hosts only  

---

## Author
Mohamed
