# CMPG-325-NETWORK-PROJECT
## **Project Overview**
This project demonstrates the design, implementation, and configuration of various network topologies using Cisco Packet Tracer. The project is divided into three main parts:

Part I (60%): Design and simulation of 5 basic topologies (Bus, Mesh, Star, Ring, Extended Star) and 1 hybrid topology  
Part II (20%): Implementation of EIGRP for IPv6 on network devices  
Part III (20%): Video demonstration showcasing configurations and testing  

### Technologies Used

Cisco Packet Tracer (version 15.4)  
IPv4 and IPv6 addressing  
VLAN segmentation  
EIGRP routing protocol  
Network services: HTTP, DNS  


**Part I: Network Topologies Design & Simulation**
1. **Bus Topology**  
Location: /topologies/bus-topology.pkt

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
 <img width="560" height="400" alt="image" src="https://github.com/user-attachments/assets/03881011-6928-40a4-99bc-de437ef5f846" />



## **Part II: EIGRP for IPv6 Configuration**

Location: /topologies/eigrp-ipv6-topology.pkt
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
2000:mb:boss:3::/64 - Router3 to Switch3 

 

