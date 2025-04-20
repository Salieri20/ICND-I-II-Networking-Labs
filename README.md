# ICND I & II - Networking Labs
**Institution:** ITI  
**Tools:** Cisco Packet Tracer

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
- QoS (Classification, Marking, Queuing)
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
| [Lab 1](/Labs/Lab1-Basic-Device-Config) | Device Initialization | CLI proficiency, Password encryption | `enable secret`, `line console 0`, `service password-encryption` |
| [Lab 2](/Labs/Lab2-VLAN-Trunking) | Advanced VLANs | VLAN trunking, VTP configuration | `switchport trunk allowed vlan`, `vtp domain`, `show vtp status` |
| [Lab 3](/Labs/Lab3-InterVLAN-Routing) | Layer 3 Switching | SVI configuration, Router-on-a-stick | `interface vlan 10`, `encapsulation dot1q`, `show interface trunk` |
| [Lab 4](/Labs/Lab4-OSPF) | OSPF Implementation | Multi-area OSPF, Route summarization | `area range`, `network 10.0.0.0 0.255.255.255 area 0`, `passive-interface` |
| [Lab 5](/Labs/Lab5-EIGRP) | EIGRP Configuration | Metric calculation, Feasible successors | `variance`, `metric weights`, `show ip eigrp topology` |
| [Lab 6](/Labs/Lab6-ACLs) | Network Security | Named ACLs, Reflexive ACLs | `ip access-list extended`, `evaluate`, `established` |
| [Lab 7](/Labs/Lab7-NAT) | NAT/PAT | Overload configuration, Port forwarding | `ip nat inside source list`, `overload`, `clear ip nat translation *` |
| [Lab 8](/Labs/Lab8-DHCP) | Network Services | DHCP relay, IPv6 addressing | `ip helper-address`, `ipv6 dhcp pool`, `debug dhcp` |

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

📂 [Project Files](/Final-Project) 

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

