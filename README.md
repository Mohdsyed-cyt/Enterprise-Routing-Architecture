# Enterprise Network Segmentation & Gateway Routing

## Project Overview
This project focuses on designing and implementing a segmented network architecture to facilitate secure communication between two distinct departments. Using a **Cisco 2911 ISR**, I established a centralized routing gateway to bridge different logical subnets and ensure controlled traffic flow.

## Architectural Design
The infrastructure is divided into two primary segments to optimize management and security:
* **Internal Operations Segment:** A three-node workstation cluster on the `192.168.1.0/24` subnet.
* **Remote/Management Segment:** A second three-node cluster on the `172.16.100.0/24` subnet.
* **Inter-Subnet Routing:** Both segments are aggregated via **Cisco 2960 Access Switches** and uplinked to dedicated GigabitEthernet interfaces on the primary router.

## Technical Skills Demonstrated
* **Network Topology Design:** Creating logical segmentation for organizational departments.
* **L3 Routing:** Configuring gateway interfaces and inter-VLAN traversal.
* **IP Schema Management:** Implementing a structured addressing plan for scalability.
* **Cisco IOS Configuration:** Hands-on command-line experience with ISR and Catalyst switches.

## Addressing Schema
| Device Group | Interface | Subnet | Gateway |
| :--- | :--- | :--- | :--- |
| Operations (PCs 0-2) | Gig 0/0 | 192.168.1.0/24 | 192.168.1.1 |
| Management (PCs 3-5) | Gig 0/1 | 172.16.100.0/24 | 172.16.100.1 |

---
**View the Full Technical Documentation:** [Download PDF Here](./Mohdsyed_Enterprise-Routing-Architecture.pdf)
