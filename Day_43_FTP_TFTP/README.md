# Day 43 – FTP/TFTP File Transfer and IOS Upgrade

## Objective
Practice using **TFTP and FTP** to transfer files between devices and upgrade router operating systems.

---

## Lab Description
- R1 and R2 routers connected to SRV1 (file server)  
- IP addresses and routing configured for full connectivity  
- TFTP used on R1 to retrieve IOS image from SRV1  
- FTP used on R2 to retrieve IOS image with authentication  
- Upgraded IOS on both routers and deleted old images from flash  

---

## Approach
1. Verified current flash, file system, and IOS version on routers  
2. Configured TFTP on R1 and FTP on R2 to retrieve IOS files from SRV1  
3. Upgraded routers’ IOS images and set the new image as boot system  
4. Deleted old IOS images from flash after upgrade  
5. Verified successful file transfer and system upgrade  

---

## What I Understood
- TFTP allows simple, unauthenticated file transfer; FTP allows authenticated transfer  
- IOS upgrades require careful file transfer and boot system configuration  
- Verifying flash and file system ensures sufficient space for upgrades  
- Router IOS can be managed and upgraded remotely using TFTP/FTP  
- Always delete old IOS images after upgrade to free flash space  

---

## Author
Mohamed
