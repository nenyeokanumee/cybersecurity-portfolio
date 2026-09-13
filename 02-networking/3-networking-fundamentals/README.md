# NETWORKING FUNDAMENTALS

A computer network is an interconnection of devices to share information and resources. Examples include the Internet, home Wi-Fi, and office LANs.

Networking matters in cybersecurity because you need to understand networks and devices to protect them. Also, every security threat exploits networks and devices. When a device is online or on a network, it has a chance of being vulnerable.

## Types of Networks

1.  PAN (Personal Area Network): Bluetooth devices connect via Bluetooth, like from a smartwatch to a phone. It has to be within a 10-metre radius.

2.  LAN (Local Area Network): A single building. Example: home or office network, school computer lab, etc

3.  MAN (Metropolitan Area Network): Within a geographical area. It is a region- or city-wide network.

4.  WAN (Wide Area Network): This refers to a global network. Example: the Internet.

## Network Topologies

Network topology is the visual map that tells you the structure of the computer network. Here you see the exact location and path of each device on the network.

Physical topology refers to how you can physically see the devices connected. You see the devices and the cables in real time in the space where the connection is set up.

Logical topology has to do with how data flows within a network. It shows you how packets of data move from source to destination.

## Types of Topologies

Go online to see pictures of these topologies. It will make it easier for you to understand.

1.  **Bus Topology**: Here, all the devices are connected to a single backbone cable. That one cable manages every device in the system. It is easy to set up, and it can work with cheap cables, so it is inexpensive. The major drawback with this topology is collisions on the backbone cable. Also, there is a single point of failure in this topology, and when this happens, the connection is ruined.

2.  **Star Topology**: Here, all devices are connected to a central hub or switch. It is easy to troubleshoot, such as isolating the problem and sorting it out. The major drawback here is a single point of failure. If the switch or hub is faulty, the entire network is affected. Another drawback is cabling cost.

3.  **Ring Topology**: In this topology, devices are connected in a circular chain. Data flows in one direction. Traffic is predictable, so it is easy to troubleshoot. If one of the cables connecting the PCs is faulty or if one of the PCs is faulty, it affects the entire network.

4.  **Mesh Topology**: Here, there is no point of failure as everything is interconnected. There is a lot of redundancy simply to ensure that a single point of failure does not affect the entire network. There is high availability of routes that packets can follow. The drawback is that it is too complex. It is expensive to set up.

5.  **Tree/Hierarchical Topology**: This is a star of stars. It is very scalable for an enterprise. One of the cons is that it is very complex to manage.

## Devices Found in a Network

1.  **Hub**: It is used to connect devices. The issue is that it is slow or not intelligent enough to identify the destination of a packet, so what it does is that it broadcasts every packet of data that passes through it. This device is not currently in use in most network setups.

2.  **Switch**: It is similar to a hub in that it connects devices. The advantage is that it learns the MAC addresses of devices connected to it and sends data only to the device(s) that the data is meant for.

3.  **Router**: This device connects networks. It uses IP addresses to connect different networks. A switch uses a MAC address, but a router uses IP addresses.

4.  **Firewall**: This device filters traffic based on defined rules that you set. It can be hardware or software.

5.  **Endpoint**: These are end-user devices that can send and receive services and resources. Examples are PC, laptops, printers, mobile phones, etc.

6.  **Server**: This is a device that provides services or data to other devices upon request. Devices making the request are known as clients.

## Network Media Types

Data is transmitted in binary. Computers convert our commands to binary and transmit them in binary. Data can then travel in either wired media or wireless media.

**Wired Media**: Here, data is encoded into electrical impulses and then transmitted through a copper cable. The cable could be either a twisted pair or a coaxial cable. It is susceptible to interference. Coaxial cables have a conductive metal shield, often aluminium foil or copper braid, that helps protect the signal from electromagnetic interference. Data can also be encoded in pulses of light. It has very high bandwidth and travels very long distances, e.g., a fibre optic cable.

**Wireless Media**: Wireless media uses electromagnetic waves for communication. Examples: Wi-Fi and radio.

## Network Model

The network model is a standard that all network device manufacturers follow when manufacturing a network device. It is this model that enables devices of different manufacturers to connect in a network. A Samsung printer can communicate with an HP laptop. So, any manufacturer that does not follow this model won't be able to communicate on a network. There are two major models: the OSI model and the TCP/IP model.

## OSI

This model is a 7-layer theoretical framework that was created by ISO (International Organisation for Standardisation) for network communication. It is a standard framework for how data travels.

OSI provides a detailed framework of how the network works, and it is best when it comes to troubleshooting.

The seven layers are: physical, data link, network, transport, session, presentation, and application.

1.  Physical Layer (Manage Cables/signals): Here we talk about the physical transport medium you can see, like cables and wireless. It works with 1s and 0s.

2.  Data Link Layer (MAC Addressing): It has to do with local delivery, delivering data within your local network using MAC addresses. Switches work here on Layer 2.

3.  Network Layer (Routing/IP addressing): Checks whether the packet is something that should go outside the local network and determines the destination path. It is the routing layer that uses the IP address of the destination to find the best path to the destination.

4.  Transport Layer (Reliable Delivery): This layer ensures reliable data delivery. It uses port numbers. At this layer, packets of data are broken into smaller chunks and then transmitted. It uses the TCP or UDP protocol. In UDP, some packets may be missing or lost, like in calls and video games. But in TCP, no packet must be lost because it works with sensitive data; for example, banking transfers and chats. The application chooses the transport protocol; the transport layer provides the chosen protocol.

5.  Session Layer (Manage connection): This layer establishes, manages, and terminates connections between applications.

6.  Presentation Layer (Data Formatting and Encryption): This is where the formatting is done. Here, data is formatted, encrypted, or decrypted into the correct format (before it is presented to you). Compression is also done here.

7.  Application Layer (User Interface): This is the user interface. This is where the user uses the software on the computer. It provides network services directly to end users. Example: HTTP, FTP. The application layer is in charge of what you see on your screen.

## Popular Mnemonic: Please Do Not Throw Sausage Pizza Away

## TCP/IP

This model is a 4-layer model that shows how the internet actually works in the real world.

1.  Application Layer (HTTP, FTP, SMTP, DNS) = OSI Layers 5, 6, 7

2.  Transport Layer (TCP, UDP) = OSI Layer 4

3.  Internet Layer (IP, ICMP) = OSI Layer 3

4.  Network Access (Ethernet, ARP, WIFI, Fibre) = OSI Layers 1, 2

OSI is used for troubleshooting, while TCP/IP is how the internet actually works.

## Encapsulation & De-encapsulation: Wrapping & Unwrapping Data Layer by Layer

The raw data is moved to the application layer and then transported to the transport layer, where it adds a segment header and specifies the protocol it will use (TCP or UDP). Next, it moves to the Internet layer, where it adds the packet header that defines the IP address it will use for routing. Next, it goes to the Network Access Layer, which adds the frame header that contains the MAC address information that it needs to move; then it goes to the last layer, where it will be converted to bits. When it gets to the destination, de-encapsulation (or unwrapping) begins.

## MAC Address

MAC address is a 48-bit physical address embedded in the hardware. It is the device's permanent identifier. It cannot change. The first 24 bits are the manufacturer's ID, and the second 24 bits are the device identifier. No two devices have the same MAC address. MAC addresses work at layer 2 of the OSI model via a switch. MAC addresses work best within a Local Area Network. A MAC address is assigned by the device's manufacturer.

## IP Address

Internet Protocol Address is the logical address that operates at layer 3 of the OSI model. It is assigned to every device connected to the network, and it can change. IP addresses are assigned by the ISP.

There are two types of IP addresses: IPV4 and IPV6.

IPV4 is 32-bit, i.e., 4 bytes or octets. Each octet ranges from 0 to 255. There are approximately 4.3 billion possible IP addresses. It is running out as more network devices and endpoints are being produced.

IPV6 is 128 bits and uses hexadecimal. It most likely cannot run out.

## Private Vs Public IP Address

A private IP address is used inside local networks. It is not routable on the internet but can be reused within a local network. Common ranges are 10.X.X.X, 172.16.X.X - 172.31.X.X, and 192.168.X.X.

Public IP addresses are globally unique addresses assigned by ISPs or registries. It is regulated across the internet. Example 203.22.45.6.

## IPV4 Address Classes

CLASS A: Extremely large and can accommodate approximately 16.7 million host addresses per network (2²⁴−2).

CLASS B: For SMEs, can host more than 65,000 host addresses

CLASS C: Small or personal networks and can host a maximum of 254 hosts

## Subnetting

A subnet is a small network within a local network. It divides one big network into subsidiary networks. Every subnet has its own pool of IP addresses, and subnets cannot share IP addresses.

IP addresses usually have certain properties, such as the subnet mask. The subnet mask consists of two main parts: the host portion and the network portion. Each subnet should represent a department in an organisation.

Subnetting is important in an organisation because it helps the infrastructure be organised. It helps to reduce network congestion by limiting broadcast traffic. It helps with network segmentation too. It isolates sensitive systems from general access. It makes troubleshooting easier.

## Subnetting for Security

Subnetting creates boundaries. Traffic between subnets must pass through a router or firewall. An infrastructure without a subnet is prone to breaches. Any device on one subnet cannot navigate to another subnet; the device can only share resources within the subnet it belongs to.

Organisations use subnetting to limit the scope of systems subject to PCI-DSS assessment. If segmentation is applied, PCI-DSS v4.0 mandates that this subnet must be tested twice a year to prove that it actually isolates the cardholder data environment (CDE) from the rest of the network.

## Network Transmission Classification

A network is classified into three different ways: unicast, multicast, and broadcast.

UNICAST: coming from one source and heading to one destination

MULTICAST: from one source to multiple destinations.

BROADCAST: from one source to all devices in the network.

## Ports and Port Numbers

Ports are virtual doors that applications in a device use to communicate over a network. There are 65,535 ports per IP address. See the IP address as the building address and the port number as the flat number. Port numbers are usually attached to the IP address. Example: 192.168.9.0:80, where 80 is the port number.

Examples of port numbers are:

1.  20/21 = FTP

2.  25 = SMTP

3.  80 = HTTP

4.  53 = DNS

5.  22= SSH, secure version of Telnet

6.  443 = HTTPS

## Network Protocol

A network protocol is a set of rules that adds context to the binary data in a computer. It determines how data is formatted, transmitted, and received to ensure network communication. Examples include: communication protocols, address resolution protocols, Internet protocols, Transmission Control Protocol, User Datagram Protocol, Dynamic Host Configuration Protocol.

## Address Resolution Protocol

ARP maps a logical address to a physical address just to make sure that the packet gets to the right device. Networks know logical addresses but don't know physical addresses, so it sends an ARP request (a broadcast). So, the right device replies with its physical address. Then the MAC address is cached in an ARP table so that it won't need to send another ARP.

## DNS

Domain Name System (DNS) is the internet's phonebook. It translates human-readable domain names into IP addresses. DNS exists because humans remember names easily but computers need numbers. DNS bridges the gap so that you won't need to memorize IP addresses.

DNS Poisoning can occur. DNS details can be corrupted, and you are directed to a different website without you even knowing. DNS is a single point of failure, so without DNS, the internet will be almost unusable.

## TCP Vs UDP

TCP is a network protocol that provides reliable and steady transmission. It uses the TCP three-way handshake to initiate a connection. The three-way handshake is a SYN, SYN-ACK, ACK communication where the SYN is initiated or sent by the client. TCP tracks packets, so it requires a connection.

UDP is connectionless. It doesn't require an active connection to establish communication. UDP doesn't track packets, so it doesn't require a connection. It is very fast since it doesn't need a three-way handshake, so it can be used for streaming.

## DHCP

Dynamic Host Configuration Protocol is a protocol that requires hosts within a network to automatically obtain an IP address. The DHCP server makes this pool of IP addresses available. It functions at layer 7 of the OSI model.

It uses DORA

D - Discover: the client sends a discover request to a DHCP server. Like, hey server, I need an IP address.\
O - Offer: the server replies with an offer of an available IP address\
R - Request: the client sends an official request. Something like, I will take this IP address that you are giving to me.\
A - Acknowledge: the server then approves the lease of the IP address

You can either configure the IP statically (manually), or you can use a DHCP server.

NB: The router assigns an IP address within a local network. But on the internet, it is the ISP that is the DHCP server. DHCP will collect an IP address from a client when its lease expires, and the client makes another DORA request.

## Network Threats

These threats exploit the fundamental aspects of how the network operates.

## DoS/DDoS

DoS (Denial of Service): Here, a device or IP overwhelms a server by sending multiple requests beyond the capacity of the server.

DDoS (Distributed Denial of Service): Here, an attacker leverages botnets (devices, IoT, people's PCs, anything that can communicate on the internet) to send multiple requests to a server just to overwhelm the server. The attacker can use as many as thousands of devices.

The goal is to make the server unavailable to legitimate users.

As a SOC analyst, you can block an IP address when it comes to DoS. It can be overwhelming for a SOC analyst when it comes to DDoS.

## Spoofing

This is when someone pretends to be something or someone trusted that they are not. Attackers use spoofing to carry out a Phishing attack. They use forged IP addresses, email headers, or other identifiers to carry out this attack.

## Sniffing

Here, an attacker is eavesdropping on network traffic. It is common on free public Wi-Fi. When you connect to such a service, someone could be sniffing what you are doing. A tool that can be used to do this is Wireshark. You can use Wireshark to capture traffic on a network. From Wireshark, you can see what is happening on everybody's device. You capture packets traveling in a network. You can't interrupt or interact with the communication.

## Man-in-the-middle

In this scenario, someone is in the middle of a communication between two people, intercepting and altering the traffic. An example is when someone asks a friend for account details to make a transfer; a MITM intercepts and changes the account details to their own.

The attacker positions themselves between the client and the server with the intent of relaying or modifying messages between them.

## Defence Mechanism: Firewalls

A firewall controls the flow of data or traffic on the internet. You set rules that your firewall follows to determine the traffic it will allow or drop. The firewall filters the traffic based on rules, and it is the IT department that gets to set the rules. These rules could be to allow or deny certain IP addresses based on the port or protocols being used. For example, on a sensitive server, you can create an allow list on the server based on the IP addresses you want to access the server and then block every other unauthorised person. It also logs security events.

## Types (The Evolution)

1.  Stateless/ Packet Filtering: This firewall only checks the packets alone. It does not have memory of the packet headers. It checks bits of the packet one by one. It cannot verify if fragmented bits are malicious.

2.  Stateful: This one tracks ongoing connections and only allows traffic that belongs to a recognised session. It judges based on the connection, not bits. Once it allows a packet, it will keep allowing it into the network and take note of the rules set in place. Once the stateful firewall sees a malicious packet, it will block everything out.

3.  3rd Generation: This one inspects the content of the packets. Even if the packet does not have malicious behaviour, it will check it.

4.  New Generation: This firewall is a combination of stateless, stateful, and 3rd generation firewalls, and then it adds deep packet inspection. It makes sure that nothing slips in by mistake.

## Real World Use

1.  Network Firewall: This firewall protects the entire network.

2.  Host Firewall: This one is for individual devices

Example Rules:

-   Allow HTTP (80) & HTTPS (443)

-   Block all other incoming traffic

-   Allow SSH (22) from admin IPs only

## Intrusion Detection System (IDS) / Intrusion Prevention System (IPS)

Intrusion Detection System monitors and alerts you when it notices or sees a threat. It doesn't engage with the threat; all it does is alert you when it finds a threat. It is configured using a signature-based approach (known attacks) and an anomaly-based approach (unusual patterns). IDS only detects and informs. It does not block. It logs suspicious activity.

Intrusion Prevention System: An IPS would detect and block the threat in real time. It will log the report, like telling you what it saw and what it did. It is the same as an IDS, just that it has an automatic response. It drops malicious packets and blocks the attacker's IP.

## Defence Mechanism: VPN

Virtual Private Network (VPN) is a technology that allows connection to a different network through remote access. You need to have the client software installed and connected to the VPN server. The VPN server will authenticate the client, and a connection is established. This connection is a secure tunnel that is extremely difficult to intercept.

VPN hides your IP address. All traffic appears to be coming from the VPN server when traced. It also protects data from untrusted networks such as public WIFI.

Remote workers use a VPN to access the company network. It protects privacy on public WIFI. VPN bypasses geographic restrictions.

## Defence-In-Depth Strategy

This is a security approach that uses multiple layers of defence. If one layer fails, others continue to protect. No single defence strategy is enough on its own. These layers are

1.  People & Policy: Security training, policy implementation, and background checks on new hires.

2.  Physical Security: Install locked doors, badges, access control, cameras, motion sensors, and secure server rooms.

3.  Perimeter Security: Firewall, VPN, email filtering, DMZ (demilitarized zone) for public-facing servers

4.  Network Security: Subnetting, IDS/IPS, Network monitoring

5.  Endpoint Security: Antivirus, EDR, Host Firewall, patching

6.  Application Security: Secure coding, updates, input validation, web application firewalls

7.  Data Security: encryption at rest and in transit, backups.

Example: an attacker sends phishing mail to an organisation

Here is how defence in depth works;

Layer 1 Email Filtering: Blocks 90% of phishing emails automatically\
Layer 2 Security Training: 8 trained employees recognised this threat and reported it. 2 clicked on the phishing link\
Layer 3 Web Filter: Blocks malicious websites for 1. 1 was able to reach the malicious site.\
Layer 4 Endpoint Protection: Antivirus attempts to detect and block downloaded malware. If it escapes detection, it moves to the next layer.\
Layer 5: If malware defeats the antivirus, EDR comes in to isolate the endpoint.\
Layer 6: Network Segmentation: Even if the malware works, it can only access that subnet\
Layer 7: Backups: If ransomware encrypts files, clean backups allow recovery; no ransom payment needed.\
Result: What targeted 100 employees results in zero data loss because of the multiple layers of defence.

The first three layers were bypassed, but Layer 4 is there to stop the malware. Layers 5 - 7 are unused reserves, which is the whole point of defence-in-depth.

## Conclusion

Networking is the foundation of cybersecurity. Every threat discussed in this document (spoofing, sniffing, man-in-the-middle, DoS/DDoS) exploits a specific part of networking. You can't find an anomaly in a network if you do not understand the OSI layer and how it works.

The defence mechanisms (firewalls, IDS/IPS, VPNs, subnetting, and defence-in-depth) discussed here should be taken seriously because no single control catches everything. It is important to understand where each one sits in the OSI model because it is what turns \"I know what a firewall is\" into \"I know when a firewall isn't enough.\"
