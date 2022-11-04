

# Udemy - The Complete Networking Fundamentals Course. Your CCNA start 2020-7

# The Distance Between YOur Dreams and Reality is Called Persistance.

**if you continue you will get it you will understand it** 

# Basic Networking Terms

## what is network ?

**why do we have computer networks?**

**what's the whole point of the internet?**

**answer : sharing resources**

**now what is a resource ?**

in the old days a common example of a resource would be a printer

or another example would be a file or video. you can share file resources whit USB but it's much easier just to share files using a digital transmission mechanism 

![1](images/1.png) 

**computing device :** laptop, macbook, phone, server, printer

## most basic type of network

the internet is the biggest network that we have on earth today.
a small network would simply consist of 2 computers.

**wifi an example of using the air for transmission of data from one device to the other instead of using cable(RJ45)**

## a bit of networking history

**internet start with 10base5 cabling**

## servers, clients, ports, protocols

a server is providing a service or functionality ot clients in what's called a client server model.

client is a piece of computer hardware or software that accesses a service made available by a server.
the server is often on another computer system, in which case the client accesses the service by way of a network.

**the whole idea of a server is to provide resources or functionality to clients**

**a client device such as a laptop can act as a server**

now a server, will be listening on different prot numbers for different protocols.

**protocol basically a set of rules used for communication between devices.**

**server has to listen on specific prot numbers for specific protocols.**


## Networking Devices Repeaters, Hubs, Switches, Routers

### so in conclusion, hubs and switches are used to create networks while routers are used to connect networks.

**repeaters => hubs => bridges(learns MAC addresses in software) => switch(learns MAC addresses mu ch more quickly by using hardware ASICs Application Specific Integrated Circuits)**

1. **hub**: repeats the signal without understanding what's going on, work on layer 1.

**a wifi network or a wireless network is essentially a hub in the air**

2. **switch**: a switch actually reads the frames received on ethernet, so uses a MAC address table, and only forward the frames out of the correct port.and uses for local network(LAN) or vLAN(virtual local network), route from one subnet to another. and work on layer 2.

the big difference between a switch and a hub is a switch has intelligence.

so that's one of the features of switches they allow us to connect many devices in our local area network.

3. **routers** which use IP addresses to route from one network to another network, layer 3.

**typically little routes like(my home modem) allow us to go from our LAN onto the internet(WAN)**

## Firewalls

**firewall in front of the router**
![2](images/2.png) 

**firewall behind of the router**
![3](images/3.png) 

if i have 100 access points for manage them, they would connect to the Wireless LAN controller.

---------------------

# TCPIP Model

![4](images/4.png) 
![5](images/5.png) 


how many layers are there in networking? OSI or TCPIP Model.

people in the real world are saying the OSI model is rubbish. other people say's no OSI model is required. 

**you need to know both the OSI model and TCPIP model but concentrate on the TCPIP model**
![6](images/6.png) 

**the TCPIP protocol is what we use in the real world**

**so now in the new version of the CCNA we have what these called hybrid model or combined model of OSI and TCPIP model**
[ipspace](https://www.ipspace.net/Main_Page)

### RFC
**RFC allow us to agree on what protocol will be implemented by different vendors**

![7](images/7.png)

![8](images/8.png) 

## Bits, Frames, Packets, Segments

![9](images/9.png) 

on ethernet devices communicate using MAC address, and MAC addresses are burnt in address on a network interface card.

**ARP** resolution protocol requesting the MAC address, (so basically saying who has this IP address)

**TCp packet, so in TCP before communication takes place they do three way handshake**

how does one layer referred to the layer above it ?

at layer 2 on ethernet it uses a type field

when a device receives a frame at layer 2 it needs to know which protocol to use... in other words is it an IPv4 packet or is it an IPv6 packet? it's based on the type field at layer 2

> The "Type" field in Ethernet II frames tells the OS what kind of data the frame carries – 0x0800 means that the frame has an IPv4 packet; there's a list of different EtherTypes.

[answer](https://superuser.com/a/423281)

![10](images/10.png) 


-------------------------

# Binary

**2^n** = number of binary values

![11](images/11.png) 
 
![12](images/12.png) 

![13](images/13.png) 

![14](images/14.png) 

**octet**

![15](images/15.png) 

**ipv4** = 4 octet

**192.168.2.16** = 8bits . 8bits . 8bits .8bits

![16](images/16.png) 

**IP Address Example**

![17](images/17.png) 

------------------

# Hexadecimal 

**ARP is used to find the MAC address of another device in the network it's basically broadcast sent out into the network saying who has this IP address and that device will reply back with its MAC address**

![18](images/18.png) 

![19](images/19.png) 

![20](images/20.png) 

`ipconfig /all` in windows show MAC address

`arp -a` show MAC address

**some cisco switches command**

1. `en` takes us to privilege mode
2.  `show mac address-table`

-----------------------

# IP Addressing

## what is an IP Address

![21](images/21.png) 

**a lot of web sites don't permit PING which uses ICMP so the request times out, but the DNS server resolve**

**`nslookup` just does a DNS resolution of a domain name rather than trying to ping the server**

**IP Characteristics**

![22](images/22.png) 

![23](images/23.png) 

## Network vs Host Portion

![24](images/24.png) 

## IPv4 format

![25](images/25.png) 

**IPv4 classes**

![26](images/26.png) 

**Class A**

![27](images/27.png)

![28](images/28.png) 

![29](images/29.png) 

**Class B**

![30](images/30.png) 

![31](images/31.png) 

**Class C**

![32](images/32.png) 

![33](images/33.png) 

**Class D**

**Multicast** one device has talking to a group of devices

![34](images/34.png) 

**Class E**

**Reserved classes for broadcast**

![35](images/35.png) 

## summary

![36](images/36.png) 
![37](images/37.png) 
![38](images/38.png) 


## Directed Broadcast Address

![39](images/39.png) 

**CPU of every device will be interrupted to process the directed broadcast**

![40](images/40.png) 

## Local Broadcast Address

![41](images/41.png) 

## Local Loopback Address

![42](images/42.png) 

## Private Address

**Essentially a lot of the information that we're studying in networking, comes originally form RFCs**

**RFC1149 describe IP**

**RFC1948 Private IP**

![43](images/43.png) 

![44](images/44.png) 

## Link - Local Addresses

![45](images/45.png) 

**if you'r IP address in the range 169.254.0.0 that means the PC was not able to get an IP address via a DHCP.**

## Subnet Mask

**a subnet mask is used to determine which part of an IP address is the network portion and which part of the address is the host portion**



![46](images/46.png) 
![47](images/47.png) 
![48](images/48.png) 
![49](images/49.png) 
![50](images/50.png) 

**how does a device know whether another device is local or remote to itself??**

![51](images/51.png) 

**Example**

![52](images/52.png) 
![53](images/53.png) 

**Discontiguous Network Mask**

![54](images/54.png) 

## CIDR (Classless Inter-Domain Routing)

![55](images/55.png) 
![56](images/56.png) 


**Notice in class A B C addresses, the subnet mask is set on the Octet Boundary**

**with CIDR the subnet mask can be somewhere in the middle, It doesn't have to be on the octet boundary.**

![57](images/57.png) 

**so from 1993 CIDR is more preferable than classfull network mask.**

![58](images/58.png) 
![59](images/59.png) 

----------------------------------

# Initial Device Configuration


## switch initial configuration

**Do NOT plug direct pc to a cisco switch with RJ45 cable!!**

**just plug with USB!!**

1. **we connected a cisco switch to a computer**
2. **with putty and serial connection type we connected to the switch (COM Ports)**
3. **with `en` command go to the administrator mode**
4. `erase startup-config`
5. `show version`
6. `configure terminal` global configuration
7. `hostname <your_hostname>`
8. `end` take back to to enable mode
9. `copy running-config startup-config` or `wr` save config to the disk

## Router initial configuration

**connect CONSOLE cable to the RS-232 of pc to the CONSOLE prot of the router**

![60](images/60.png) 

## build a basic cisco network

**another difference between switches and routers is switch interfaces by default come up generally, but router interfaces all by default disabled or shut down you need to enable those interfaces by using the no shutdown command.**

**config ip address in the router :**

1. `en`
2. `show ip int brief` show interface_number
3. `conf t`
4. `interface <choose_interface> <interface_number>`
5. `interface GigabitEthernet 0/0/0` 
6. `ip address 10.1.1.1 255.255.255.0`
7. `no shutdown`
8. `end`
9. `hostname R1`
10. `end`
11. `copy running-config startup-config` or `wr`

1. `show ip interface <interface_name> <interface_number>`
2. `show arp`
3. `show running-config`

**set enable password**
1. `en`
2. `conf t`
3. `enable password <user_password>`

**encrypt enable password**
1. `en`
2. `conf t`
3. `service password-encryption`

**config secret password**
1. `en`
2. `conf t`
3. `enable secret <your_secret>`
### secret password overwrite the enable password

**telnet configuration**

1. `en`
2. `sh ru`
3. see the status of line vty 0 4
4. `conf t` 
5. `line vty 0 4`
6. `login`
7. set password `password <your_pass>`
8. `end`

**config console password**
1. `en`
2. `conf t`
3. `line console 0`
4. `login`
5. `password <your_pass>`
6. `end`

## Ethernet Cabling

### Straight-through Cable :

1. connect user to switch
2. connect router to switch or hub

![61](images/61.png) 

### Crossover Cable :

![62](images/62.png) 

### Rolled Cable :

![63](images/63.png) 

-----------------------------

# IP Subnetting

## Binary Method

![64](images/64.png) 

**Example 1**

![65](images/65.png) 

**Example 2**

![66](images/66.png) 

![67](images/67.png) 

![68](images/68.png)

![69](images/69.png) 

**Example 3**

![70](images/70.png) 

![71](images/71.png) 

![72](images/72.png) 


## Quick Method 

![73](images/73.png) 

**Example 1**

![74](images/74.png) 

![75](images/75.png) 

![76](images/76.png) 

![77](images/77.png) 

![78](images/78.png) 

![79](images/79.png) 

![80](images/80.png) 

## How to Subdivide a network

### why ?

![81](images/81.png) 

**It's not practically possible to have so many hosts on the subnet, a lot of network engineers will put a maximum of 254 hosts on a subnet, in other words they would subnet down to class C subnet**


**the formula to work out how many host are supported on a subnet**

![82](images/82.png) 

### how ?

![83](images/83.png) 

![84](images/84.png) 

![85](images/85.png) 

**Question 1**

![86](images/86.png) 

![87](images/87.png) 

![88](images/88.png) 

![89](images/89.png) 

![90](images/90.png) 

**we have taken 1 subnet supporting 254 hosts and change that into 16 subnets each supporting 14 hosts**


10-5