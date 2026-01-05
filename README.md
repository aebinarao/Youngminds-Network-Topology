# 🌐 Youngminds Enterprise Network Design Project



**📋Overview**

This project demonstrates a enterprise network topology that I developed in my network engineering 1 class during my college days. 
The design focuses on network segmentation, redundancy, and scalability to support a small business environment with multiple departments.


**📖 Project Description**

Your class has been tasked with designing a small business network 
for a hypothetical company called “Young Minds” company.
The company has 70 employees in the manufacturing/production 
department, 35 in the finance and marketing department, 25 in the IT/NOC 
department and 12 for the human resource department. All these operate in 
a single office building with three floors.
The company needs a reliable and secure network that allows 
employees to access files, printers, and the internet. The company also 
needs a wireless network that allows employees to connect to the network 
from their personal devices

The network simulates a small enterprise with four departments (HR/Admin, IT/NOC, Manufacturing, and Finance), each with its own VLAN for traffic isolation and security. The design includes redundant core switching, wireless access points, and WAN connectivity to simulate real-world business requirements.

***
🏗️ Network Architecture

🔀 VLANs Implemented

- 🏢 VLAN 40 - HR/Admin: Human Resources and Administrative workstations
- 💻 VLAN 30 - IT/NOC: IT department and Network Operations Center
- 🏭 VLAN 10 - Manufacturing: Production floor devices and systems
- 💰 VLAN 20 - Finance: Finance department workstations

⚡ Key Features Implemented

🔄 Routing & Switching

- 🗺️ OSPF: Internal dynamic routing across all sites
- 🌍 BGP: External routing for ISP connectivity
- 🔄 Inter-VLAN Routing: Layer 3 switching between departments
- 🛡️ HSRP: Gateway redundancy on core switches for high availability
- 🌉 EtherChannels: Link aggregation for increased bandwidth and redundancy

🔐 Security & Access Control

- 🚫 ACLs: Access Control Lists for traffic filtering and security policies
- 🔒 SSH: Secure remote management access
- 🌐 NAT: Network Address Translation for internet access
- 🛡️ Port Security: Protection against unauthorized devices

🌳 Layer 2 Redundancy & Optimization

- ⚡ Rapid PVST+: Fast spanning tree convergence
- 🚀 PortFast: Immediate access for edge devices
- 🛡️ BPDU Guard: Protection against spanning tree attacks on access ports

🖧 Network Services

- 📡 DHCP: Automatic IP address assignment for end devices
- 🌐 DNS: Name resolution services
- 📁 FTP: File transfer services
- 📡 Wireless: Department-specific SSIDs with proper segmentation



🔢 IP Addressing Scheme
The network uses private IPv4 addressing with VLSM:

<table>
  <th>Subnet</th>
  <th>Network Address</th>
  <th>No. of usable IPs</th>
  <th>Broadcast Address</th>
  <th>Subnet Mask</th>
  <tr>
    <td>Manufacturing</td>
    <td>192.168.1.0</td>
    <td>192.168.1.1 - 192.168.1.126</td>
    <td>192.168.1.127</td>
    <td>255.255.255.128</td>
  </tr>
  <tr>
    <td>Finance</td>
    <td>192.168.1.128</td>
    <td>192.168.1.129 - 192.168.1.190</td>
    <td>192.168.1.191</td>
    <td>255.255.255.192</td>
  </tr>
  <tr>
    <td>IT/NOC</td>
    <td>192.168.1.192</td>
    <td>192.168.1.193 - 192.168.1.222</td>
    <td>192.168.1.223</td>
    <td>255.255.255.224</td>
  </tr>
  <tr>
    <td>HR/ADMIN</td>
    <td>192.168.1.224</td>
    <td>192.168.1.225 - 192.168.1.238</td>
    <td>192.168.1.239</td>
    <td>255.255.255.240</td>
  </tr>
</table>


***
<table>
<tr>
<td>
Routing Protocols

🗺️ OSPF
🌍 BGP

</td>
<td>
Redundancy

🛡️ HSRP
⚡ Rapid STP
🌉 EtherChannel

</td>
</tr>
<tr>
<td>
Security

🚫 ACLs
🔒 SSH
🌐 NAT
🛡️ BPDU Guard

</td>
<td>
Services

📡 DHCP
🌐 DNS
📁 FTP
📡 Wireless

</td>
</tr>
<tr>
<td colspan="2">
Optimization

🚀 PortFast
🔀 VLAN Segmentation
🌐 IPv4/VLSM

</td>
</tr>
</table>

***
🚀 Project Evolution
This project started as a classroom assignment and evolved into a comprehensive demonstration of CCNA concepts. I systematically added features including:

- Phase 1: Basic VLAN segmentation and routing
- Phase 2: Redundancy (HSRP, Rapid STP, EtherChannel)
- Phase 3: Security hardening (ACLs, SSH, port security)
- Phase 4: Network services (DHCP, DNS, FTP)
- Phase 5: WAN connectivity (BGP, NAT)
