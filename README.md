# Albion-University-Network-Topology
Cisco Packet Tracer simulation of a multi-campus university network with VLANs, routing, and DHCP

## Project Overview
This project simulates a multi-campus network for Albion University, which has two campuses located 20 miles apart. The university consists of four faculties: Health & Sciences, Business, Engineering/Computing, and Art/Design. Each staff member has a PC, and students have access to PCs in labs.

The purpose of this project is to **design, configure, and test a network topology** that supports the connectivity requirements of both campuses, including access to internal servers and an external email server hosted in the cloud.

---

## Objectives
- Design a scalable network for two campuses.
- Configure VLANs for network segmentation and security.
- Implement **RIPv2** for internal routing.
- Implement static routing for access to the external email server.
- Configure **DHCP** for dynamic IP addressing in administrative areas.
- Test end-to-end connectivity between departments, labs, and servers.

---

## Campus Layout

### Main Campus
- **Building A:** Administrative staff (Management, HR, Finance) and Faculty of Business  
- **Building B:** Faculty of Engineering/Computing and Faculty of Art/Design  
- **Building C:** Student labs and IT department hosting university servers  

### Smaller Campus
- **Faculty of Health & Sciences:** Staff and student labs on separate floors  

---

## Tools and Technologies
- **Cisco Packet Tracer** – network simulation and configuration   
- **RIPv2** – dynamic routing for internal network  
- **Static Routing** – external email server access  
- **DHCP** – dynamic IP allocation for administrative PCs  
- **VLANs** – network segmentation and security  

---

## Network Design

### VLANs
Each department/faculty is assigned its own VLAN:
- VLAN 10 – Administration  
- VLAN 20 – HR  
- VLAN 30 – Finance  
- VLAN 40 – Faculty of Business  
- VLAN 50 – Faculty of Engineering/Computing  
- VLAN 60 – Faculty of Art/Design  
- VLAN 70 – Student
- VLAN 80 – IT Department
- VLAN 90 – Staff
- VLAN 100 –Student Labs  
 

### IP Addressing
Each VLAN is on a separate subnet. Example:
| Department/Faculty        | IP Range          |
|---------------------------|----------------|
|Administration             | 192.168.1.0/24 |
| HR                        | 192.168.2.0/24 |
| Finance                   | 192.168.3.0/24 |
| Faculty of Business       | 192.168.4.0/24 |
| Engineering/Computing     | 192.168.5.0/24 |
| Art/Design                | 192.168.6.0/24 |
| Student                   | 192.168.7.0/24 |
| IT Department             | 192.168.8.0/24 |
| Staff                     | 192.168.9.0/24 |
| Student Labs              | 192.168.10.0/24 |


---

## Implementation Steps
1. Built network topology in **Cisco Packet Tracer** with routers, switches, and end devices.  
2. Configured **VLANs** on switches for each department/faculty.  
3. Assigned IP addresses (static for servers, dynamic via DHCP for staff PCs).  
4. Configured **RIPv2** for internal routing and static routes for the external server.  

---

## Results
- VLANs successfully segmented traffic for each department/faculty.  
- End-to-end connectivity verified for all required devices.  
- Internal servers and external email server accessible.  
- DHCP successfully assigned dynamic IP addresses to staff PCs in Building A.

---

## Screenshots
Include relevant screenshots from Packet Tracer:

- Topology diagram (`/Screenshots/topology.png`)  
- VLAN configuration (`/Screenshots/vlan.png`)  
- Routing table verification (`/Screenshots/routing.png`)  
- Ping test results (`/Screenshots/ping.png`)  

---

## Project Files
- **Cisco Packet Tracer file:** `/PacketTracer-Files/Albion_University.pkt`  
- **Configuration files (optional):** `/Configs/`  
- **Report (PDF/Word):** `/Reports/Albion_University_Report.pdf`  

---

## Author
**Collins Agbenyegah**  
Aspiring Network Engineer | IT Student  
Email: your-email@example.com
