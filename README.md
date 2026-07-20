# 🌐 Enterprise Network & Security Infrastructure Design (Practical Lab)

Designed and implemented a complete multi-site enterprise topology using PNETLab, integrating Cisco routing/switching, FortiGate firewalls, and Windows Server services.

## 📌 Topology Overview
<img width="1772" height="806" alt="Screenshot 2026-07-20 134429" src="https://github.com/user-attachments/assets/7d34b515-8b6f-4542-8091-92ffc95f5220" />

Security Note: The attached FortiGate backup files are from an isolated, local virtual lab environment. For demonstration and portfolio evaluation purposes, the lab credentials and encrypted hashes have been left intact. In a real-world production environment, all backup files would be properly sanitized or fully encrypted before storage.

## 🚀 Key Implementations

### 1. Network Core & Switching
* Configured **VLANs** and **Inter-VLAN routing**.
* Established **EtherChannel (LACP) / Aggregate ports** between the Core Switch and FortiGate firewalls for redundancy and bandwidth optimization.
* Managed **DHCP pools** directly on the Core Switch.

### 2. Firewall & Advanced Security
* Deployed FortiGate firewalls in a **High Availability (HA) cluster (Active-Passive)** for the main site.
* Implemented **SD-WAN** for optimized traffic routing.
* Configured multiple **IPsec VPN tunnels** to secure connectivity across branches.

### 3. Identity & Access Management
* Integrated FortiGate with Windows Server Active Directory (AD) utilizing **LDAP** and **FSSO** to enforce user-based and group-based security policies.

### 4. Server Publishing & Services
* Configured and managed Windows Servers, including an **IIS server** for a public-facing website.
* Securely published the website to the outside network using **FortiGate Virtual IPs (VIPs)**.

### 5. Troubleshooting & Diagnostics
* Conducted deep, end-to-end network troubleshooting across Layer 2 and Layer 3.
* Resolved routing issues, Spanning Tree Protocol (STP) anomalies, and complex firewall policy/NAT conflicts.
