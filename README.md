# Coding Studio - Computer Network Fundamentals
Lessons on Computer Network Fundamentals from **Coding Studio** that have been learned:
1. Types of Network Topology
2. Static IP Address and Ping (ICMP)
3. Static Routing
4. Telnet and SSH

## Technology Used
- Cisco Packet Tracer

## Types of Network Topology
Computer network topology has 5 types, such as:
1. Bus topology
2. Ring topology
3. Tree topology
4. Star topology
5. Mesh Topology

![Coding Studio - Types of Network Topology.png](https://github.com/eightball270/CodingStudio-ComputerNetworkFundamentals/blob/main/Coding%20Studio%20-%20Types%20of%20Network%20Topology.png)

[Project File Link](https://github.com/eightball270/CodingStudio-ComputerNetworkFundamentals/blob/main/Coding%20Studio%20-%20Types%20of%20Network%20Topology.pkt)

## Static IP Address and Ping (ICMP)
A network can be connected to each other if a static IP address is configured on each network device, then ping to make sure one device is connected to other devices.

![Coding Studio - Static IP and ICMP (Pinging).png](https://github.com/eightball270/CodingStudio-ComputerNetworkFundamentals/blob/main/Coding%20Studio%20-%20Static%20IP%20and%20ICMP%20(Pinging).png)

[Project File Link](https://github.com/eightball270/CodingStudio-ComputerNetworkFundamentals/blob/main/Coding%20Studio%20-%20Static%20IP%20and%20ICMP%20(Pinging).pkt)

## Static Routing
In this practice using 2 routers, router A is connected to network 192.168.2.0/24, router B is connected to network 192.168.3.0/24, and the network between routers is 192.168.1.0/24. In order for network 192.168.2.0 to reach network 192.168.3.0, a routing configuration must be made to forward traffic to another network. The method used is static routing, which is to create a routing table manually. The way to do static routing on router A is to add the destination network address (network address and subnet mask) and ip interface of router B which is directly connected to router A.
- ip route [destination network address] [subnet mask] [ip of another router that is directly connected]
- example command: RouterA(config)#ip route 192.168.3.0 255.255.255.0 192.168.1.2

![Coding Studio - Static Routing.png](https://github.com/eightball270/CodingStudio-ComputerNetworkFundamentals/blob/main/Coding%20Studio%20-%20Static%20Routing.png)

[Project File Link](https://github.com/eightball270/CodingStudio-ComputerNetworkFundamentals/blob/main/Coding%20Studio%20-%20Static%20Routing.pkt)

## Telnet and SSH
To remote a network device such as a router or switch from a PC/Laptop, it can be done using 2 methods, which are Telnet and SSH. Telnet and SSH are network protocols used to access remote devices. The difference between the two is that Telnet does not use data encryption, while SSH uses data encryption. Therefore, telnet is suitable for private networks, while SSH is suitable for public networks. The SSH used is SSH version 2, with a minimum rsa key requirement of 768 bits, here a configuration is made to generate an rsa key of 1024 bits. In order to be able to remote the switch device, configure the vlan1 interface by turning on and adding its ip address, then configure Telnet or SSH as well as the configuration on the router.

![Coding Studio - Telnet and SSH.png](https://github.com/eightball270/CodingStudio-ComputerNetworkFundamentals/blob/main/Coding%20Studio%20-%20Telnet%20and%20SSH.png)

[Project File Link](https://github.com/eightball270/CodingStudio-ComputerNetworkFundamentals/blob/main/Coding%20Studio%20-%20Telnet%20and%20SSH.pkt)

## Attachment
[Course Certificates (PDF)](https://github.com/eightball270/CodingStudio-ComputerNetworkFundamentals/blob/main/Coding%20Studio%20-%20Certificates.pdf)
