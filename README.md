# Coding Studio - Computer Network Fundamentals
Lessons learned on Computer Network Fundamentals from **Coding Studio**:
1. Types of Network Topology
2. Static IP Address and Ping (ICMP)
3. Static Routing
4. Telnet and SSH

## Technology Used
- Cisco Packet Tracer

## Types of Network Topology
There are 5 types of computer network topologies, such as:
1. Bus topology
2. Ring topology
3. Tree topology
4. Star topology
5. Mesh Topology

![Coding Studio - Types of Network Topology.png](https://github.com/eightball270/CodingStudio-ComputerNetworkFundamentals/blob/main/Coding%20Studio%20-%20Types%20of%20Network%20Topology.png)

[Project File Link](https://github.com/eightball270/CodingStudio-ComputerNetworkFundamentals/blob/main/Coding%20Studio%20-%20Types%20of%20Network%20Topology.pkt)

## Static IP Address and Ping (ICMP)
A network can be established if a static IP address is configured on each device. Then, use the **ping** command to ensure that each device is connected to the others.

![Coding Studio - Static IP and ICMP (Pinging).png](https://github.com/eightball270/CodingStudio-ComputerNetworkFundamentals/blob/main/Coding%20Studio%20-%20Static%20IP%20and%20ICMP%20(Pinging).png)

[Project File Link](https://github.com/eightball270/CodingStudio-ComputerNetworkFundamentals/blob/main/Coding%20Studio%20-%20Static%20IP%20and%20ICMP%20(Pinging).pkt)

## Static Routing
In this simulation involving two routers, Router A is connected to the 192.168.2.0/24 network, Router B is connected to the 192.168.3.0/24 network, and the network between the routers is 192.168.1.0/24. To enable communication between the 192.168.2.0 and 192.168.3.0 networks, a routing configuration is required to forward traffic between networks. The method applied is **static routing**, which involves manually creating a routing table. Static routing on Router A is configured by adding the destination network address (including the network address and subnet mask) along with the IP address of Router B’s interface that is directly connected to Router A.  
`ip route [destination network address] [subnet mask] [gateway/ip of another router that is directly connected]`  
example command:  
`RouterA(config)#ip route 192.168.3.0 255.255.255.0 192.168.1.2`  

![Coding Studio - Static Routing.png](https://github.com/eightball270/CodingStudio-ComputerNetworkFundamentals/blob/main/Coding%20Studio%20-%20Static%20Routing.png)

[Project File Link](https://github.com/eightball270/CodingStudio-ComputerNetworkFundamentals/blob/main/Coding%20Studio%20-%20Static%20Routing.pkt)

## Telnet and SSH
To remotely access a network device such as a router or switch from a PC or laptop, there are two methods: Telnet and SSH. Both are network protocols used to access remote devices, but they differ in security. Telnet doesn't use data encryption, while SSH does. Therefore, Telnet is more suitable for private networks, whereas SSH is recommended for public networks.

In this simulation, SSH version 2 is used, which requires a minimum RSA key size of 768 bits. Here, a 1024-bit RSA key is generated for better security. To enable remote access to the switch, the **Vlan1** interface must be configured by enabling it and assigning it an IP address. Then, configure either Telnet or SSH, just like the configuration on the router.

![Coding Studio - Telnet and SSH.png](https://github.com/eightball270/CodingStudio-ComputerNetworkFundamentals/blob/main/Coding%20Studio%20-%20Telnet%20and%20SSH.png)

[Project File Link](https://github.com/eightball270/CodingStudio-ComputerNetworkFundamentals/blob/main/Coding%20Studio%20-%20Telnet%20and%20SSH.pkt)

## Attachment
[Course Certificates (PDF)](https://github.com/eightball270/CodingStudio-ComputerNetworkFundamentals/blob/main/Coding%20Studio%20-%20Certificates.pdf)
