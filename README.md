# Network Operations Virtualization for Faculty of Computing Block N28B

> Virtualizing the network infrastructure of a brand‑new two‑storey Faculty of Computing building (Block N28B) using Cisco Packet Tracer.

---

## 📖 Table of Contents

1. [Introduction](#introduction)  
2. [Project Goals & Scope](#project-goals--scope)  
3. [Task Breakdown](#task-breakdown)  
4. [Network Architecture](#network-architecture)
5. [Topology](#topology)
6. [Key Benefits](#key-benefits)  
7. [Challenges & Lessons Learned](#challenges--lessons-learned)  

---

## Introduction

This project continues our “Network Communication” case study by virtualizing the infrastructure for a new two‑storey building at the Faculty of Computing. The building houses:

- **4 specialized labs**  
  - General Purpose (31 workstations)  
  - Computer Security (25 workstations)  
  - Network (32 workstations)  
  - IoT (25 workstations)  
- **2 video‑conferencing rooms** (2 workstations each)  

Our aim is to design, simulate, and document a scalable, secure network that supports advanced research, training, and seamless virtual collaboration 

---

## Project Goals & Scope

- **Scalability**: Accommodate future expansion and additional devices.  
- **Security**: Isolate sensitive traffic and protect data.  
- **Reliability & Performance**: Ensure low‑latency, redundant paths for uninterrupted connectivity.  
- **Practical Training**: Provide students hands‑on experience with real‑world networking concepts.

---

## Task Breakdown

1. **Task 1 – Project Setup**  
   - Form group (“NetworkNinjaz”), choose/modify an existing floor plan, record meeting minutes.  
2. **Task 2 – Topology Design**  
   - Build a simplified Packet Tracer topology (4 hosts per lab), add core and access layers, document design.  
3. **Task 3 – IP Addressing (VLSM)**  
   - Subnet the 172.16.34.0/23 network for labs, video rooms, server room, and router links; show detailed calculations.  
4. **Task 4 – Routing Protocols**  
   - Implement static & EIGRP dynamic routes, verify end‑to‑end connectivity, highlight routing in topology.  
5. **Task 5 – VLAN Segmentation**  
   - Add staff rooms on each floor, assign new subnets, demonstrate VLAN tables and connectivity.  
6. **Task 6 – DHCP Deployment**  
   - Configure lab hosts for dynamic IP assignment via a central DHCP server and relay agents.  
7. **Task 7A – Group Report**  
   - Compile results and reflections for Tasks 1–6 into a cohesive PDF with reflections, conclusions, references, and appendices.  
8. **Task 7B – Individual Report**  
   - Personal two‑page account of contributions, teamwork experiences, lessons learned, and suggestions.

---

## Network Architecture

We adopted a **two‑tier hierarchical** design with a **partial‑mesh** between routers:

- **Core Layer**  
  - Single Core Router for high‑speed forwarding and redundancy.  
- **Access Layer**  
  - Four lab routers & two video‑room subnets, each connected via Layer‑2 switches and APs.  
- **Partial‑Mesh Links**  
  - Direct router interconnections for fault tolerance, load balancing, and minimal hops.

---

## Topology
![Final topology](https://github.com/user-attachments/assets/ecc7949b-c39f-45a7-87e3-c7d4a82f3016)

---

## Key Benefits

- **Redundancy & Resilience**  
  - Mesh links ensure alternate paths on link/router failures.  
- **Efficient IP Utilization**  
  - VLSM minimizes wasted addresses across diverse subnet sizes.  
- **Segmentation & Security**  
  - VLANs isolate traffic, reducing broadcast domains and enhancing access control.  
- **Automated Host Configuration**  
  - DHCP simplifies address management and reduces misconfiguration.

---

## Challenges & Lessons Learned

- **Complex Subnet Planning**  
  - Designing VLSM for multiple small/big subnets required meticulous calculation.  
- **Routing Convergence**  
  - Balancing static vs. EIGRP routes to ensure predictable failover behavior.

---


