# CodingStudio-ComputerNetworkFundamentals
Lessons on Computer Network Fundamentals from CodingStudio that have been learned:
1. Types of Network Topology
2. Static IP Address and Ping (ICMP)
3. Static Routing
4. Telnet and SSH

## Types of Network Topology
Computer network topology has 5 types, such as:
1. Bus topology
2. Ring topology
3. Tree topology
4. Star topology
5. Mesh Topology

![CodingStudio - Jenis-Jenis Topologi Jaringan](https://github.com/user-attachments/assets/7536e634-8e16-400b-84f6-e859251a0f2e)

## Static IP Address and Ping (ICMP)
A network can be connected to each other if a static IP address is configured on each network device, then ping to make sure one device is connected to other devices.

![CodingStudio - Static IP dan ICMP (Pinging)](https://github.com/user-attachments/assets/065238e0-1a3b-46e7-811b-2377bf828bce)

## Static Routing
In this practice using 2 routers, router A is connected to network 192.168.2.0/24, router B is connected to network 192.168.3.0/24, and the network between routers is 192.168.1.0/24. In order for network 192.168.2.0 to reach network 192.168.3.0, a routing configuration must be made to forward traffic to another network. The method used is static routing, which is to create a routing table manually. The way to do static routing on router A is to add the destination network address (network address and subnet mask) and ip interface of router B which is directly connected to router A.
- ip route [destination network address] [subnet mask] [ip of another router that is directly connected]
- example command: RouterA(config)#ip route 192.168.3.0 255.255.255.0 192.168.1.2

![CodingStudio - Static Routing](https://github.com/user-attachments/assets/122e67aa-a94e-4129-a12e-4a1d57b54ff4)

## Telnet and SSH
To remote a network device such as a router or switch from a PC/Laptop, it can be done using 2 methods, which are Telnet and SSH. Telnet and SSH are network protocols used to access remote devices. The difference between the two is that Telnet does not use data encryption, while SSH uses data encryption. Therefore, telnet is suitable for private networks, while SSH is suitable for public networks. The SSH used is SSH version 2, with a minimum rsa key requirement of 768 bits, here a configuration is made to generate an rsa key of 1024 bits. In order to be able to remote the switch device, configure the vlan1 interface by turning on and adding its ip address, then configure Telnet or SSH as well as the configuration on the router.

![CodingStudio - Telnet dan SSH](https://github.com/user-attachments/assets/c01b656c-235e-494e-96ff-339d4a96f845)
