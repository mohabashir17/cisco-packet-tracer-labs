# Day 41 – Syslog and Logging Configuration

## Objective
Practice configuring and analyzing Syslog messages, logging destinations, and remote management access.

---

## Lab Description
- Connected to R1 via console from PC2  
- Generated syslog messages by shutting down and enabling an interface  
- Accessed R1 remotely using Telnet from PC1  
- Configured different logging methods (console, VTY, buffer, and syslog server)

---

## Approach
1. Used console connection to:
   - Shut down and re-enable G0/0  
   - Observe generated syslog messages  
   - Identify severity level  
   - Enable timestamps for log messages  

2. Used Telnet to access R1 via G0/0:
   - Enabled unused G0/1 interface  
   - Observed no syslog message on VTY initially  
   - Enabled logging to VTY session (Packet Tracer limitation: logging monitor enabled by default)

3. Enabled logging to router buffer and configured buffer size (8192 bytes)

4. Configured remote logging to syslog server (SRV1) with severity level set to debugging

---

## What I Understood
- Syslog messages have severity levels (0–7) indicating importance  
- By default, console displays logs but VTY sessions may not  
- Logging destinations include console, VTY, buffer, and external syslog servers  
- Buffer logging allows reviewing logs locally on the router  
- Remote syslog servers centralize logging for monitoring and troubleshooting  
- Timestamps are important for accurate event tracking  

---

## Author
Mohamed
