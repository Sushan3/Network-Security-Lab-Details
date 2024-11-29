# Network-Security-Lab-Details

#**Network Project**

**#Portfolio 01: Building a Virtual Sandboxed Network Using VirtualBox**
I am using Oracle VM Virtual Box to create this project on virtual enviroment.

**#Introduction: Briefly describe the purpose of the lab.**
This lab report details the configuration and implementation of a virtual network environment using Oracle VM VirtualBox. The primary objective was to create a functional network topology consisting of multiple virtual machines, including a desktop VM, a gateway router VM, and an application server VM. The network was designed to facilitate communication between these devices, utilizing IP addressing, subnet masking, and routing protocols.

**#Network Diagram: Include the exported diagram.**



**#IP Address Table: Present the table in a clear and organized format.**

**#Configuration Steps: Detail the steps you took to configure the network.**
Device Configuration

Desktop VM:
IP Address: 192.168.34.2/24
Default Gateway: 192.168.34.1

Gateway Router VM:
Interface enp0s3 (NAT): 10.0.2.15/24
Interface enp0s8 (Subnet 01): 192.168.134.1/24
Interface enp0s9 (Subnet 02): 192.168.34.1/24

Application Server VM:
IP Address: 192.168.134.2/24
Default Gateway: 192.168.134.1

Configuration Steps
Create Virtual Machines:
Create virtual machines for the desktop, gateway router, and application server.
Assign appropriate amounts of RAM and CPU cores to each VM.
Install operating systems on each VM (e.g., Windows, Linux).

Network Configuration:
Configure network interfaces on each VM with the specified IP addresses and subnet masks.
Set the default gateway on each VM to the appropriate IP address of the gateway router interface.
Configure the gateway router VM to act as a router between the two subnets (192.168.34.0/24 and 192.168.134.0/24).
Configure NAT on the gateway router's enp0s3 interface to allow the VMs to access the internet.

**#Challenges and Solutions: Discuss any issues you encountered and how you resolved them.**
IP Addressing and Subnetting: Ensuring correct IP address assignment and subnet configuration was crucial to prevent IP conflicts.
Routing Configuration: Configuring the gateway router to route traffic between the two subnets required careful attention to routing table entries.
NAT Configuration: Proper NAT configuration was necessary to enable internet access for the VMs.

**#Conclusion: Summarize your findings and lessons learned.**
This lab provided valuable hands-on experience in configuring and managing a virtual network environment. By successfully implementing the network topology, we gained a deeper understanding of IP addressing, subnet masking, routing protocols, and NAT. This knowledge will be invaluable in future network design and troubleshooting tasks.
