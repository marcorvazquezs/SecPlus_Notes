<!-- omit in toc -->
# Embedded and Specialized Systems

<!-- omit in toc -->
## Topics

- [Embedded systems](#embedded-systems)
- [SoC and RTOS](#soc-and-rtos)
- [Real-time operating system (RTOS)](#real-time-operating-system-rtos)
- [SCADA and ICS](#scada-and-ics)

## Embedded systems

- Found in printers, smart TVs and HVAC control systems, among other devices
- Attacks against embedded systems rely on exploiting security vulnerabilities in the software and hardware components of the implementation and are vulnerable to timing and side channel attacks

## SoC and RTOS

- **System on chip (SoC)** is basically a hardware module in a small form factor
- Examples: nanorobots, video devices for the visually impaired and wireless antennas

## Real-time operating system (RTOS)

- **Real-time operating system (RTOS)** is a small operating system used in embedded systems and IoT applications that are typically run in a SoC environment
- Main goal is to allow the rapid switching of tasks with focus on timing instead of throughput
- Vulnerabilities associated with RTOS
  - Exploitation of shared memory
  - Priority inversion
  - Interprocess communication (IPC) attacks
  - Code injection
  - DoS attacks

## SCADA and ICS

- **Supervisory Control and Data Acquisition (SCADA)** - A subset of systems considered to be critical infrastructure systems
- **Industrial Control Systems (ICS)** - A system that is considered to be critical to the infrastructure, such as manufacturing, logistics and transportation networks, energy and utilities, agriculture and food production networks.
- A key control against attacks on SCADA systems is to implement physical segregation of internal and external network to reduce the attack surface
