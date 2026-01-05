# 🌐 Youngminds Enterprise Network Design Project



**📋Overview**

This project demonstrates a enterprise network topology that I developed in my network engineering 1 class during my college days. 
The design focuses on network segmentation, redundancy, and scalability to support a small business environment with multiple departments.


**📖 Project Description**

Your class has been tasked with designing a small business network 
for a hypothetical company called “Young Minds” company.
The company has 62 employees in the manufacturing/production 
department, 28 in the finance and marketing department, 20 in the IT/NOC 
department and 8 for the human resource department. All these operate in 
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

⚡ Key Features

- 🔄 Inter-VLAN Routing: Configured Layer 3 switching to enable communication between different VLANs while maintaining security boundaries
- 🛡️ HSRP Configuration: Implemented Hot Standby Router Protocol on core switches for gateway redundancy and automatic failover
- 🗺️ OSPF Routing: Deployed OSPF as the dynamic routing protocol for efficient route propagation across the WAN
- 📡 Wireless Integration: Separate wireless access points configured for each department with corresponding SSIDs
- 🌍 WAN Connectivity: Point-to-point links connecting branch offices to headquarters and external cloud services
