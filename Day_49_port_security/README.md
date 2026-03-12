# Day 49 – Port Security

## Objective
Practice configuring **Port Security** on switch interfaces and observe how different violation modes behave.

---

## Lab Description
Port Security was configured on specific interfaces of **SW1** and **SW2** to control how many MAC addresses can connect to a port and what action occurs if the limit is exceeded.

Configuration highlights:
- **SW1 (F0/1, F0/2, F0/3)**
  - Maximum MAC addresses: 1
  - Violation mode: Shutdown
  - Sticky learning: Disabled
  - MAC aging: 1 hour

- **SW2 (G0/1)**
  - Maximum MAC addresses: 4
  - Violation mode: Restrict
  - Sticky learning: Enabled

After configuration, additional devices were connected to trigger **port security violations**.

---

## Approach
1. Configured port security on the required switch interfaces.
2. Set the maximum allowed MAC addresses for each port.
3. Applied different violation modes (Shutdown and Restrict).
4. Enabled sticky MAC learning on SW2.
5. Triggered violations by connecting extra devices and observed switch behavior.

---

## What I Understood
- **Port Security** limits which devices can connect to a switch port using MAC addresses.
- **Shutdown mode** disables the interface when a violation occurs.
- **Restrict mode** drops unauthorized traffic but keeps the port active.
- **Sticky learning** automatically saves learned MAC addresses to the configuration.
- **MAC aging** allows learned addresses to expire after a set time.

---

## Author
Mohamed
