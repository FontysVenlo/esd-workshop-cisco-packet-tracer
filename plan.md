# Cisco Packet Tracer Workshop Plan

> **Duration:** ~1 hour  
> **Goal:** Introduce students to basic networking concepts and practical network simulation using *Cisco Packet Tracer*.

---

## Workshop Overview

| **Section** | **Topic** | **Duration** |
|--------------|------------|---------------|
| 1 | Introduction | 15 min |
| 2 | Devices & Connections | 15 min |
| 3 | Basic Networking Concepts | 15 min |
| 4 | Network Services | 35 min |
| 5 | Routing & VLANs | 10 min |
| 6 | Security & Performance | 10 min |
| 7 | Final Simulation | 5–10 min |
| 8 | Wrap-Up & Q&A | 5 min |

---

## 1. Introduction

### Objectives
- Introduce the **purpose** of the workshop and its connection to *Computer Architecture and Networking (CAN)*.
- Explain **what Cisco Packet Tracer (PT)** is and why it’s valuable for visualizing real-world networks.
- Outline **the workshop structure** and expected learning outcomes.

### Topics Covered
- Understanding network devices and communication.
  - Questions to ask: 
    - What network devices do you know
    - What type of comunication means do you know
- OSI model and data flow.
  - Questions:
    - Have you ever heard the OSI Model
    - Do you know the different layers of the OSI model
    - Which devices belong to which layer
- Key protocols: **ARP**, **DHCP**, **DNS**, **RIP**.
- VLANs, routing, and firewall setup.
- Simulating and analyzing network performance.

---

## 2. Devices & Connections

### Concepts Introduced
- **Network Hardware:**
  - Hubs  
  - Switches  
  - Routers  
  - Servers  
  - PCs / Laptops  

- **Transmission Media:**
  - Copper cables  
  - Fiber optic cables  
  - Wireless connections  

### Discussion Points
- Physical vs. Logical **Topologies** (Star, Bus, Mesh, etc.)  
- **LAN vs. WAN**  
- **OSI Layers Overview**  
- Role of **ARP (Address Resolution Protocol)**  

### Packet Tracer Demo
- Add and connect basic devices.  
- Configure basic links and verify connectivity using **ping**.  
- Identify interfaces and physical connections.

---

## 3. Basic Networking Concepts

### Concepts
- **Addressing:**
  - IP and MAC addresses  
  - Subnetting basics  

- **Topologies:**  
  - Star  
  - Bus  
  - Mesh  

- **Data Flow:**  
  - Show how packets travel through devices.  
  - Use **Simulation Mode** to visualize ARP and data transmission.

### Packet Tracer Activity
- Create a **small LAN** with 2 PCs and a switch.  
- Assign **static IP addresses** and verify communication.  

---

## 4. Network Services

### DHCP (Dynamic Host Configuration Protocol)
- Explain how DHCP assigns IP addresses automatically.
- Configure a **DHCP Server**:
  - IP range, default gateway, DNS address.
- Connect clients and verify automatic IP allocation.

### DNS (Domain Name System)
- Explain domain names vs. IPs.
- Configure a **DNS Server** and map:
- example.local → 192.168.1.10

- Verify by **pinging the domain name** instead of the IP.

### Servers
- Introduce different server roles:
- Web Server  
- DNS Server  
- DHCP Server  
- Host a **simple static web page** accessible from another PC.

---

## 5. Routing & VLANs

### Routing Information Protocol (RIP)
- Explain dynamic routing and why it’s useful.
- Configure **RIP routing** between two routers:
- Enable RIP on both routers.  
- Add network addresses.  
- Verify route propagation using `show ip route`.

### VLAN (Virtual LAN)
- Explain VLANs for **network segmentation**.
- Create VLANs in a switch:
- VLAN 10 – Administration  
- VLAN 20 – Students  
- Assign ports to VLANs and test isolation.

---

## 6. Security & Performance

### Firewall Configuration
- Explain the role of firewalls in protecting a network.
- Demonstrate **basic firewall setup**:
- Block specific IPs or ports.  
- Restrict traffic between VLANs.

### Performance & Monitoring
- Use Packet Tracer tools to:
- Measure latency and packet loss.  
- Analyze network traffic flow.  
- Control traffic using ACLs (Access Control Lists).  

---

## 7. Final Simulation

### Objective
Integrate all previously learned concepts into one complete setup.

### Scenario
1. A **web server** is hosted in *Network B*.  
2. A **client PC** in *Network A* tries to access it via the domain `example.local`.  
3. The system includes:
 - **DHCP** for dynamic IP allocation  
 - **DNS** for name resolution  
 - **RIP routing** between routers  
 - **Firewall rules** controlling access  

### Expected Output
The client successfully opens the web page using the **domain name**, demonstrating proper network configuration.

---

## 8. Wrap-Up & Q&A

### Summary
- Key takeaways:
- Network structure and topology  
- Communication protocols and services  
- Practical routing and VLAN setup  
- Security basics  

### Discussion
- Open Q&A session.  
- Encourage students to experiment with:
- Custom topologies  
- VLAN configurations  
- Additional protocols (FTP, SMTP, etc.)

---

## Workshop Materials

| **Material** | **Description** |
|---------------|-----------------|
| Presentation Slides | Used for theory and visual explanations. |
| Cisco Packet Tracer File (.pkt) | Pre-configured base file for live demonstration and student practice. |
| Exercises | 1. Build a LAN with DHCP + DNS. <br> 2. Configure RIP between routers. <br> 3. Host and access a webpage via DNS name. |

---

## Suggested Structure for the Cisco Packet Tracer File

| **Component** | **Details** |
|----------------|-------------|
| Routers | 2 (connected via serial or Ethernet) |
| Switches | 2 (one per network) |
| PCs | 4 (2 per LAN) |
| Servers | 1 Web/DNS/DHCP Server |
| Connections | Copper Straight-Through & Fiber |
| VLANs | VLAN 10 (Admin), VLAN 20 (Students) |
| IP Range | 192.168.1.0/24 and 192.168.2.0/24 |
| Protocols | DHCP, DNS, RIP, ARP |
| Security | Basic Firewall Rules & ACLs |

---

> **Tip:**  
> The workshop should balance theory and practice.  
> Start each section with a short explanation (2–3 minutes), followed by a live Packet Tracer demonstration where students can follow along.

---