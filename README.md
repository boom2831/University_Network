
# University Networking – CN Mini Project
---

## 📌 Project Overview

This project simulates a scalable and secure university campus network using **Cisco Packet Tracer**. It addresses key challenges such as network congestion, inefficient communication, and lack of secure access to central resources through a well-planned topology featuring VLANs, DMZ, DHCP, DNS, and dynamic routing.

---

## 🧩 Features

- Logical segmentation using **VLANs** for departments (HR, Admin, Finance, etc.)
- **Inter-VLAN routing** via a central router
- **Dynamic Host Configuration Protocol (DHCP)** for automatic IP assignment
- **Domain Name System (DNS)** for hostname resolution
- **Routing Information Protocol (RIP v2)** for dynamic path sharing
- **DMZ (Demilitarized Zone)** for hosting public services like web and email
- **VPN connectivity** for remote branch access
- **Ping tests** for verifying communication between departments and branches

---

## 🗺️ Network Topology Highlights

- **Core Router:** Handles inter-VLAN routing and connects all departments
- **Switches:** Each department is connected to switches configured with relevant VLAN IDs
- **PCs:** Configured with static IPs for testing or DHCP where applicable
- **Servers:** Deployed in the DMZ (VLAN 99) to host Web, DNS, and Email services
- **Routers:** Simulate campus branches and cloud connectivity with RIP protocol

---

## 💻 IP Configuration (Examples)

| Device | IP Address     | Subnet Mask       | Default Gateway   |
|--------|----------------|-------------------|-------------------|
| PC0    | 192.168.1.2    | 255.255.255.0     | 192.168.1.1       |
| PC1    | 192.168.2.2    | 255.255.255.0     | 192.168.2.1       |
| ...    | ...            | ...               | ...               |
| PC9    | 192.168.9.2    | 255.255.255.0     | 192.168.9.1       |

> Note: VLANs are assigned according to department subnets (e.g., VLAN 10 for HR: `192.168.10.0/24`)

---

## 🛡️ Security Features

- **VLAN Isolation** to limit unnecessary broadcast traffic
- **Controlled Inter-VLAN Routing** for regulated cross-department access
- **DMZ** ensures public-facing servers are segmented from internal network
- **Private IP Addressing** to avoid direct internet exposure

---

## 🌐 VPN & Remote Access

- Remote branch networks are connected via simulated **VPN/WAN**
- RIP v2 allows dynamic exchange of route info between main and branch routers
- Branch employees securely access main campus services through VPN

---

## ✅ Testing & Results

- **Ping tests** confirm:
  - Inter-department connectivity
  - Branch to campus server communication
  - Branch-to-branch communication

---

## 📚 Conclusion

The University Networking project successfully models a real-world, secure campus network. With robust configurations and simulation tests, this project demonstrates practical implementation of:

- Network segmentation
- Remote access via VPN
- Public-private server isolation
- Automated IP management
- Dynamic routing protocols

---

## 🚀 Future Enhancements

- Implementation of **Access Control Lists (ACLs)**
- Integration of **Wireless Access Points**
- Deployment of **Network Monitoring Tools**
- Use of **IPv6 addressing** for future scalability
