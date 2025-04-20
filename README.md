# ICND I & II - Networking Labs
**Institution:** ITI  
**Tools:** Cisco Packet Tracer, Wireshark, GNS3

## 📌 Overview
### Core Networking Competencies Demonstrated:
#### 🌐 **Network Fundamentals**
- IPv4/IPv6 addressing & subnetting (VLSM, CIDR)
- OSI/TCP-IP model implementation
- Ethernet standards (UTP, fiber, PoE)

#### 🔄 **Switching Technologies**
- VLANs (Voice/Data segregation)
- STP/RSTP/PVST+ configuration
- EtherChannel (LACP/PAGP)
- Switchport security (MAC limiting, sticky MAC)

#### 🛣️ **Routing Technologies**
- Static routing (floating static routes)
- Dynamic routing (OSPFv2/v3, EIGRP metrics)
- Route summarization & redistribution
- IPv6 routing (OSPFv3, EIGRP for IPv6)

#### 🔒 **Network Security**
- Standard/Extended/Named ACLs
- NAT/PAT (Static, Dynamic, Overload)
- Port security & DHCP snooping
- Basic VPN concepts (IPSec, GRE)

#### ⚙️ **Infrastructure Services**
- DHCPv4/v6 (Server/Relay agent)
- DNS & NTP configurations
- Device management (SSH, Syslog, SNMPv3)

#### 🛠️ **Troubleshooting**
- Layer 2 issues (VLAN mismatches, STP loops)
- Layer 3 issues (Routing protocol adjacencies)
- Network analysis tools (ping, traceroute, debugs)
- Wireshark packet captures

---

## 🛠 Labs
| Lab | Topic | Key Skills | Key Commands |
|-----|-------|------------|--------------|
| [Lab 1](01-Initial-Device-Setup) | Device Initialization | CLI proficiency, Password encryption | `enable secret`, `line console 0`, `service password-encryption` |
| [Lab 2](02-VLAN-Implementation) | Advanced VLANs | VLAN trunking, VTP configuration | `switchport trunk allowed vlan`, `vtp domain`, `show vtp status` |
| [Lab 3](03-InterVLAN-Routing) | Layer 3 Switching | SVI configuration, Router-on-a-stick | `interface vlan 10`, `encapsulation dot1q`, `show interface trunk` |
| [Lab 4](04-Subnetting) | Subnetting & Summarization | VLSM, Network summarization, Route tracing | `ip address`, `show ip route`, `ping`, `traceroute` |
| [Lab 5](05-OSPF-Configuration) | OSPF Configuration | Multi-area OSPF, Passive interfaces | `router ospf`, `network`, `passive-interface` |
| [Lab 6](06-EIGRP-Implementation) | EIGRP Implementation | Metric calculation, Feasible successors | `router eigrp`, `variance`, `show ip eigrp topology` |
| [Lab 7](07-ACL-Firewalling) | ACLs & Security | Named ACLs, Reflexive ACLs | `ip access-list extended`, `evaluate`, `established` |
| [Lab 8](08-NAT-Translation) | NAT/PAT | Overload configuration, Port forwarding | `ip nat inside source list`, `overload`, `clear ip nat translation *` |


---

## 🏆 Final Project
**Enterprise Network Design**  
**Topology Features:**  
✅ Multi-site OSPF with Area 0 backbone  
✅ IPv4/IPv6 dual-stack implementation  

**Security Implementation:**  
- Role-Based ACLs (HR/Engineering/Guest)  
- 802.1X port authentication  
- Zone-Based Firewall  

📂 [Project Files](Final-Project) 

---

## 🔧 How to Use This Repository

1. **Open Labs**:
   - Open `.pkt` files with **Cisco Packet Tracer** to simulate each lab.
   - Use the corresponding `README.md` (if available) in each lab folder for lab instructions.

2. **Practice Configurations**:
   - Open CLI on each device in Packet Tracer.
   - Type in or paste the relevant configuration commands listed in the table above or from the lab’s notes.

3. **Analyze Network Traffic (if available)**:
   - Open `.pcap` or `.dmp` files using **Wireshark**.
   - Use filters like `ip.addr == 192.168.1.1` or `tcp.port == 80` to inspect packets.

4. **Explore the Final Project**:
   - Open the full network topology in Packet Tracer.
   - Explore routing tables, QoS policies, HSRP states, ACL rules, and test connectivity.

5. **Recommended Order**:
   - Start from **Lab 1** and progress sequentially.
   - Leave the Final Project for the end to consolidate all learned topics.

```bash
# Example: Open OSPF Lab
packetracer Labs/Lab4-OSPF/OSPF_MultiArea.pkt
```

Happy labbing! 🎓💻

