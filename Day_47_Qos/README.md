# Day 47 – QoS (Quality of Service) Basics

## Objective
Learn basic QoS configuration by classifying traffic and marking packets with DSCP values, then allocating minimum bandwidth for different traffic types.

---

## Lab Description
In this lab I configured QoS policies on **R1** and applied them outbound on **interface G0/0/0**.

Traffic types handled in the policy:

- **HTTPS** → marked as **AF31** and placed in a **priority queue (minimum 10% bandwidth)**
- **HTTP** → marked as **AF32** with **minimum 10% bandwidth**
- **ICMP** → marked as **CS2** with **minimum 5% bandwidth**

Simulation mode in Packet Tracer was used to observe packet markings and traffic behavior.

---

## Approach
1. Classified traffic based on protocol types (HTTPS, HTTP, ICMP).
2. Marked packets with appropriate **DSCP values**.
3. Allocated minimum bandwidth for each traffic class.
4. Applied the QoS policy **outbound on R1’s G0/0/0 interface**.
5. Used **Simulation Mode** to inspect packet headers and verify DSCP markings during traffic.

---

## What I Understood
- QoS allows networks to **prioritize important traffic**.
- **DSCP markings** identify the priority level of packets.
- **Priority queues** ensure critical traffic (like HTTPS) is transmitted first.
- Bandwidth guarantees help prevent lower-priority traffic from starving the network.
- Simulation tools help visualize how QoS policies affect packet handling.

---

## Author
Mohamed
