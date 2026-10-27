# CMPG 325 — Network Topologies & IPv6 Routing

A Cisco Packet Tracer project exploring network design, switching, VLAN segmentation, IPv4/IPv6 addressing, and EIGRP routing. The repository contains topology files, configuration notes, and screenshots.

## Explore the simulations

| Simulation | Cisco Packet Tracer file |
| --- | --- |
| Bus | [Open Bus Topology](<Bus Topology/bus topology.pkt/Bus Topology.pkt>) |
| Mesh | [Open Mesh Topology](<Mesh Topology/mesh.topology/Mesh Topology.pkt>) |
| Star | [Open Star Topology](<Star Topology/star topology.pkt/Star Topology.pkt>) |
| Ring | [Open Ring Topology](<Ring Topology/ring topology.pkt/Ring Topology.pkt>) |
| Extended star | [Open Extended Star](<Extended Star/Extended star.pkt/Extended Star Topology.pkt>) |
| Hybrid (VLANs and services) | [Open Hybrid Topology](<Hybrid Topology/hybrid topology.pkt/latest_hybrid2.pkt>) |
| IPv6 EIGRP | [Open IPv6 EIGRP topology](<Part ll/eigrp-ipv6-topology.pkt/part2.pkt>) |

### How to review

1. Download the relevant `.pkt` file from its link above.
2. Open it in a compatible version of Cisco Packet Tracer.
3. Inspect the addressing, interfaces, VLANs, routing configurations, and connectivity tests.
4. Read the topology-specific folders for configuration notes and screenshots.

**Note:** The configuration stored in each Packet Tracer file is the reference for exact interface addresses and device settings. The report below records the project's design and reported tests.

---

## Detailed project documentation

## **Project Overview**
This project demonstrates the design, implementation, and configuration of various network topologies using Cisco Packet Tracer. The project is divided into three main parts:

Part I (60%): Design and simulation of 5 basic topologies (Bus, Mesh, Star, Ring, Extended Star) and 1 hybrid topology  
Part II (20%): Implementation of EIGRP for IPv6 on network devices  
Part III (20%): Video demonstration showcasing configurations and testing  

### Technologies Used

Cisco Packet Tracer  
IPv4 and IPv6 addressing  
VLAN segmentation  
EIGRP routing protocol  
Network services: HTTP, DNS  


**Part I: Network Topologies Design & Simulation**
1. **Bus Topology**  
File: [Bus Topology.pkt](<Bus Topology/bus topology.pkt/Bus Topology.pkt>)

Description: Linear topology where all devices connect to a single backbone cable    
Devices: 4 PCs, 4 switches  
**Key Features:**

Simple design with minimal cabling
Single point of failure demonstration

## **Screenshot:**
<img width="800" height="545" alt="image" src="https://github.com/user-attachments/assets/699d55b5-2fdf-4a99-bcb9-b271c12b0791" />

 **2. Mesh Topology**
Location: /topologies/mesh-topology.pkt

Description: Full/partial mesh where devices have multiple redundant connections  
Devices: 4 routers/switches with redundant links  
**Key Features:**

High redundancy and fault tolerance  
Multiple communication paths  
## **Screenshot:**  
<img width="650" height="580" alt="image" src="https://github.com/user-attachments/assets/304c3543-a4b8-4150-b5c7-30a97c188b2d" />

**3. Star Topology**
Location: /topologies/star-topology.pkt

Description: Central hub/switch with devices radiating outward
Devices: 1 central switch, 5 PCs
**Key Features:**

Easy to manage and troubleshoot
Central point of failure

## **Screenshot:**
<img width="580" height="490" alt="image" src="https://github.com/user-attachments/assets/bc318c47-e4e6-4962-af0d-f60c7880e863" />

**4. Ring Topology**
Location: /topologies/ring-topology.pkt

Description: Devices connected in a circular fashion  
Devices:4 devices in ring configuration    
**Key Features:**

Data flows in one direction  
Equal access for all devices

## **Screenshot:**  
<img width="650" height="400" alt="image" src="https://github.com/user-attachments/assets/18d79c4b-3202-4562-a881-48ee553fdc9f" />  

**5. Extended Star Topology**
Location: /topologies/extended-star-topology.pkt

Description: Hierarchical star with multiple star networks connected together
Devices: Multiple switches in hierarchical design, 4 PCs
**Key Features:**  

Scalable design  
Distributed network segments  
## **Screenshot:** 
<img width="700" height="450" alt="image" src="https://github.com/user-attachments/assets/81dc0ec9-8085-4562-9f0c-6a3db32d40ac" />

### **6. Hybrid Topology**   
Location: /topologies/hybrid-topology.pkt

Description: Integration of all 5 basic topologies into one comprehensive network  
**Network Segments:**

VLAN 10: Ring,Extended star - Students section  
VLAN 20: Bus - Admin section  
VLAN 30: Mesh,star - Guest section  
VLAN 40: Server segment (HTTP/DNS)    



**Key Features:**

IPv4 and IPv6 dual-stack configuration  
VLAN segmentation for security and traffic management  
Multiple servers: HTTP (Server-PT HTTP), DNS (Server-PT DNS)    
DHCP for automatic IP assignment    
Inter-VLAN routing configured    
Basic security measures implemented   

**Devices:**

Routers: 1 (Router0 - 1941)  
Switches: 12 (2960-24TT models)  
End devices: 20 PCs total   
Servers: 2 (HTTP, DNS)      
## **Screenshot:**  
<img width="800" height="500" alt="image" src="https://github.com/user-attachments/assets/bb24ea62-5a19-4c6e-9adb-9dbbace8c70c" />  
 <img width="484" height="300" alt="image" src="https://github.com/user-attachments/assets/03881011-6928-40a4-99bc-de437ef5f846" />  <img width="484" height="300" alt="image" src="https://github.com/user-attachments/assets/059f83a8-0ea5-4d78-b4b4-61cf8ed461c4" />  

 **Security Features**

Port security enabled on access ports  
VLAN segmentation isolates traffic  
Access control lists (ACLs) for inter-VLAN traffic control 
Password is enabled on router  
     



## **Part II: EIGRP for IPv6 Individual Configuration Proj_90**

File: [IPv6 EIGRP Packet Tracer topology](<Part ll/eigrp-ipv6-topology.pkt/part2.pkt>)
Note: This is a separate topology designed specifically to demonstrate EIGRP for IPv6 routing protocol configuration and functionality.  
Implementation Details  
EIGRP (Enhanced Interior Gateway Routing Protocol) for IPv6 has been configured on the following devices:  
**Configured Devices:**

Router2 (1941)
Router3 (1941)

Network Topology:

Router2 connects to Switch2 → PC0  
Router2 ↔ Router3 (backbone connection)  
Router3 connects to Switch3 → PC1  

IPv6 Networks:

2000:bad:cafe:1::/64 - Router2 to Switch2  
2000:bad:cafe:2::/64 - Router2 to Router3 link  
Router3 to Switch3: consult the Packet Tracer file for the exact IPv6 subnet (the earlier placeholder in these notes was not valid IPv6 notation)

## **Screenshot:** 
<img width="400" height="350" alt="image" src="https://github.com/user-attachments/assets/8fb0add2-0fcd-4639-ba2c-e6d20d7253be" />
<img width="400" height="350" alt="image" src="https://github.com/user-attachments/assets/4f1f352b-d960-4c4e-950c-919d9fd656b6" />  



## Testing & Verification
### **Connectivity Tests Performed**

**Intra-VLAN Communication**

PC0 to PC1 (VLAN 10) - Successful  
PC4 to PC5 (VLAN 20) - Successful  
PC10 to PC11 (VLAN 30) - Successful  


**Inter-VLAN Communication**

VLAN 10 to VLAN 20  - Successful   
VLAN 20 to VLAN 40 (Server access) - Successful  


**Service Verification**

HTTP Server accessible from all VLANs  
DNS resolution working  
 


**EIGRP Verification**

Neighbor relationships established  
Routes learned and advertised  
IPv6 connectivity via EIGRP 

 


## Challenges Faced & Solutions
Part I: Network Topologies Design
Challenge 1: VLAN Configuration Complexity

Configuring trunk ports between switches and ensuring all VLANs were properly allowed on trunk links  
Solution: Used systematic approach - configured VLANs first, then set trunk ports with specific VLAN allowances  

Challenge 2: Inter-VLAN Routing

Getting devices in different VLANs to communicate with each other  
Solution: Configured router-on-a-stick or SVI (Switch Virtual Interfaces) for inter-VLAN routing with proper IP addressing on each VLAN interface  

Challenge 3: IP Addressing Scheme

Planning and implementing a logical IP addressing scheme across multiple VLANs and network segments  
Solution: Created detailed IP addressing table before implementation to avoid conflicts and ensure proper subnet allocation  

Challenge 4: Integrating Multiple Topologies

Combining Bus, Mesh, Star, Ring, and Extended Star into one cohesive hybrid topology    
Solution: Planned the network architecture on paper first, identifying which topology type best suited each network segment (Admin, Students, Guest, Servers)    

## Part II: EIGRP for IPv6 Configuration  
Challenge 6: IPv6 Address Format

Understanding and correctly implementing IPv6 addressing format (much different from IPv4)  
Solution: Followed structured IPv6 addressing scheme (2000:bad:cafe::/48) and used consistent patterns for each network segment  

Challenge 7: EIGRP Not Forming Neighbor Relationships

Initially, Router2 and Router3 were not becoming EIGRP neighbors
Solution: Ensured no shutdown command was executed under ipv6 router eigrp 1 and verified interfaces were in the same IPv6 subnet
 

