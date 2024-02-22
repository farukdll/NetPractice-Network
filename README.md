<h1 align="right"> <a name="up"></a>

<h1 align="center"> NetPractice(Network Addressing)

<h1 align="center">
</br>
<p>
  <img width="150" alt="Host" src="https://user-images.githubusercontent.com/97880185/211656437-609c2afe-8673-4b69-b960-9a8247a855c3.png">
  <img width="160" alt="Switch" src="https://user-images.githubusercontent.com/97880185/211656464-3daa6f82-578b-4c6b-8d54-ff28b93e670f.png">
  <img width="150" alt="Router" src="https://user-images.githubusercontent.com/97880185/211656451-11235c84-f555-427b-916e-93a428a816b9.png">
  <img width="130" alt="Internet" src="https://user-images.githubusercontent.com/97880185/211656370-91ad141f-d7c5-4877-8136-0f7f6237c646.png">
</h1> <p> </p>


### Description
  * ###### NetPractice is a project that provides an understanding of networking concepts with a focus on solving TCP/IP addressing and network configuration problems. In this way, you will learn basic concepts such as IP addressing, subnet mask calculation, router and switch usage, while improving your network management skills.


### Table of Contents
  * [What is TCP/IP ?](#witcpip)
  * [What is TCP ?](#witcp)
  * [What is a IP ?](#wiaipadd)
  * [Binary number system calculation for IP addresses](#bnscfipaddss)
  * [What is the difference between TCP and IP ?](#witdbtcpaip)
  * [What are Network ID and Host ID ?](#wanidahid)
  * [What are Private and Public IP addresses ?](#wapapipaddd)
  * [What are Network address and Broadcast address ?](#warnaabtadd)
  * [What is subnet mask ?](#wisubmaskkk)
  * [What is a switch ?](#wiasch)
  * [What is a router ?](#wiarer)
  * [What is the difference between a switch and a router?](#hasarwwitdbt)
  * [What is a diversion table ?](#wiadttle)
  * [Questions and Solutions](#quesaslti)


#### What is TCP/IP ? <a name="witcpip"></a>
  * ###### TCP/IP stands for Transmission Control Protocol/Internet Protocol and refers to a family of protocols that enable data communication over the Internet. This protocol family sets the standards and rules that make communication between computers possible. The TCP/IP protocol family includes many sub-protocols, such as IP (Internet Protocol) and TCP (Transmission Control Protocol), and is the foundation of the internet. IP is used for routing data packets and delivering them to the destination device, while TCP is used to ensure reliability in data communication. Together, the TCP/IP protocol family ensures reliable and efficient data communication over the internet.
  * ###### To summarize, the TCP/IP family of protocols is a generic structure for data communication over the Internet, consisting of four main layers: the application layer, which includes applications with which users interact directly; the transport layer, which provides reliability in data communication; the internet layer, which provides routing of data packets; and the network access layer, which provides physical network connectivity.
  * ###### If you want me to explain it in a simpler way, In the TCP/IP Protocol, there are 4 layers. At the top layer is the application layer. The application layer receives data from the user and processes it, converting it into data packets; such as web browsers, email clients, etc. Then it sends these packets to a lower layer, the transport layer. The transport layer receives these data packets and delivers them reliably to the next lower layer, the internet layer, reaching the destination. It also controls the data flow and performs error correction. The internet layer, in turn, receives the data packets from the transport layer and directs them to the next lower layer, the network access layer. Each device is assigned a unique IP address, and the packets are transmitted according to these addresses. The network access layer provides the physical network connection and transmits the data packets in binary format over the physical network; for example, using technologies like Ethernet or Wi-Fi.
  * ###### Here is a sample TCP/IP Protocol Diagram
  <h1 align="center">
  <p>
      <img height="280" width="430" src="https://github.com/farukdll/NetPractice-Network/assets/97880185/733c2f9c-4bdd-4bdc-b814-fd74a5fb22be">
      <img height="280" width="330" src="https://github.com/farukdll/NetPractice-Network/assets/97880185/13b44816-49cb-4daf-9441-8b9b3a89897a">
  </h1> <p> </p>


#### What is TCP ? <a name="witcp"></a>
  * ###### TCP (Transmission Control Protocol) is a communication protocol used to establish reliable connections between computers. TCP ensures secure packaging, sending, receiving, and reordering of data packets. This protocol operates on top of IP (Internet Protocol) and includes important features such as connection establishment, correct sequencing of data packets, error detection, and correction. These features provided by TCP ensure reliable and orderly data communication over the Internet.
  * ###### In simpler terms, TCP (Transmission Control Protocol) guarantees the integrity of data transmitted over a network. It establishes a connection between the source and destination before data transmission and maintains this connection until communication begins. It then divides large amounts of data into small packets during the data flow and ensures that it is delivered end-to-end without any data loss.
    * ###### TCP's main tasks at the layer where it resides are the following: Data Transmission, Flow Control, Error Correction, Connection Management.
    * ###### Data Transmission: TCP is responsible for reliably transmitting data packets between computers. It ensures that data packets are not lost and arrive at the destination intact.
    * ###### Flow Control: TCP regulates the flow of data. It adjusts the speed of data packets and controls traffic on the network, preventing overload.
    * ###### Error Correction: TCP detects and corrects errors that may occur in data packets. This maintains the integrity of the data packets.
    * ###### Connection Management: TCP establishes a connection before communication starts and closes the connection when communication ends. This ensures that data transmission takes place in a successful and orderly manner.
  <h1 align="center">
  <p>
      <img height="280" width="330" src="https://github.com/farukdll/NetPractice-Network/assets/97880185/a6dc9757-fc20-4afa-b294-cfd09c947478">
      <img height="280" width="430" src="https://github.com/farukdll/NetPractice-Network/assets/97880185/df2eac38-a7eb-4c19-8cee-5eefd57b9db8">
  </h1> <p> </p>


#### What is a IP ? <a name="wiaipadd"></a>
  * ###### IP (Internet Protocol) is a communications protocol used to enable data communication in computer networks. This protocol manages the routing, addressing and forwarding of data packets. IP enables communication between different devices on a network. IP resides at the Internet Layer, the third layer of the TCP/IP protocol stack. The Internet Layer handles the addressing and routing of data packets. IP works closely with TCP (Transmission Control Protocol) at the transport layer. TCP manages the flow of data while IP handles the addressing and routing of data packets. These two protocols work together to ensure reliable and accurate communication between computers.
  * ###### An IP address is a sequence of numbers separated by dots. IP addresses are expressed as a set of four numbers; an example address would be 192.158.1.38 Each number in the set can range from 0 to 255. So the full IP addressing range is from 0.0.0.0 to 255.255.255.255
  * ###### IP's main tasks at the layer where it resides are the following: Addressing, Routing, Fragmentation, Error Detection, Protocol Management
  * ###### Addressing: IP assigns each device a unique address. This address determines the location of the device on the network and ensures that data packets reach the correct destination. These addresses can usually be in IPv4 or IPv6 format.
  * ###### Routing: IP routes data packets based on their source and destination addresses. This ensures that data packets reach the correct destination and manages communication on the network.
  * ###### Fragmentation: IP enables communication by dividing data packets into portable sizes (fragmentation) between different networks during transmission. This is necessary because different network technologies support different maximum data packet sizes.
  * ###### Error Detection: IP performs error detection to ensure the integrity of transmitted data packets. It detects erroneous or corrupted packets and sends an alert for retransmission if necessary.
  * ###### Protocol Management: Provides management of upper layer protocols such as IP, TCP and UDP. This determines which upper layer protocol data packets use and carries information about these protocols with the data packets.
  <h1 align="center">
  <p>
      <img height="280" width="330" src="https://github.com/farukdll/NetPractice-Network/assets/97880185/947bc78c-0951-4ea2-9d97-961c6f775fe2">
      <img height="280" width="430" src="https://github.com/farukdll/NetPractice-Network/assets/97880185/df2eac38-a7eb-4c19-8cee-5eefd57b9db8">
      <img height="180" width="760" src="https://github.com/farukdll/NetPractice-Network/assets/97880185/87f5a6a6-bba1-42d3-a51e-fcbd450e0acf">
  </h1> <p> </p>
  
#### Binary number system calculation for IP addresses <a name="bnscfipaddss"></a>
  * ###### Let's calculate 192.168.11.10 sample ip address in binary → 11000000.10101000.00001011.00001010
  * ###### 192
  <h1 align="center">
  <p>
      <img height="150" width="700" src="https://github.com/farukdll/NetPractice-Network/assets/97880185/5a4305fc-84eb-409c-8e35-ba2d42095ea7">
  </h1> <p> </p>
  
  * ###### 168
  <h1 align="center">
  <p>
      <img height="150" width="700" src="https://github.com/farukdll/NetPractice-Network/assets/97880185/4ff7e2b3-6563-4b69-8634-7ad82b5c7332">
  </h1> <p> </p>
  
  * ###### 11
  <h1 align="center">
  <p>
      <img height="150" width="700" src="https://github.com/farukdll/NetPractice-Network/assets/97880185/52b2998a-bd92-4075-98f0-f6f2a2cfbbe2">
  </h1> <p> </p>
  
  * ###### 10
  <h1 align="center">
  <p>
      <img height="150" width="700" src="https://github.com/farukdll/NetPractice-Network/assets/97880185/be1fb690-be8d-4971-b064-6ff7edfa2fa8">
  </h1> <p> </p>


#### What is the difference between TCP and IP ? <a name="witdbtcpaip"></a>
  * ###### TCP and IP are two separate computer network protocols.
    * ###### TCP (Transmission Control Protocol):
      * ###### TCP is a communication protocol used to ensure reliable communication between computers.
      * ###### It manages the data flow, sorts data packets, performs error correction and provides flow control.
      * ###### It is a connection-based protocol; it manages connection establishment, data exchange and connection termination.
      * ###### It is located at the Transport Layer and works together with IP to form the second layer for data transmission.
    * ###### IP (Internet Protocol):
      * ###### IP is responsible for addressing and routing data packets in computer networks.
      * ###### Thanks to IP addresses, computers find each other and perform data flow.
      * ###### It is located at the Internet Layer and forms the third layer of the TCP/IP protocol stack.
      * ###### It routes data packets according to source and destination addresses and thus enables communication.
      * ###### Identifies devices with unique addresses, usually in IPv4 or IPv6 format.


#### What are Network ID and Host ID ? <a name="wanidahid"></a>
  * ###### Network ID :
    * ###### The network ID of an IP address indicates that all devices on the network belong to a common network.
    * ###### The network ID represents the first parts of the IP address in a particular network. This indicates that all devices on the network share the same network and belong to the same network.
  * ###### Host ID :
    * ###### The host ID is the unique identifier of devices on a given network and each device has its own unique ID.
    * ###### Each device utilizes its unique identifier to communicate with other devices on the network.
  * ###### To summarize, the Network ID represents the general location of an IP address within a network, while the Host ID represents the unique identity of a specific device within this network. In other words, Network ID and Host ID form the basis of the inter-network communication and addressing systems of IP addresses.
  <h1 align="center">
  <p>
      <img height="130" width="500" src="https://github.com/farukdll/NetPractice-Network/assets/97880185/5b40110b-0ad0-4416-ae52-5c1941b4f651">    
  </h1> <p> </p>


#### What are Private and Public IP addresses ? <a name="wapapipaddd"></a>
  * ###### Public IP addresses :
    * ###### Public IP addresses are the unique identifier of a device on the internet and are used to communicate with other internet users or devices.
    * ###### Public IP addresses are IP addresses that are open to the internet and accessible worldwide. Public IP addresses are used for websites, servers, network devices and other internet accessible devices.
    * ###### Public IP addresses are obtained by internet service providers from IANA (Internet Assigned Numbers Authority) or other authorized organizations. 
    * ###### Public IP addresses are usually globally unique as they are accessible over the internet and are used to identify millions of individual devices.  This means that they are unique across all devices connected to the internet and are therefore considered a limited resource.
    <h1 align="center">
    <p>
        <img height="400" width="600" src="https://github.com/farukdll/NetPractice-Network/assets/97880185/f5bd2d42-b7d0-4657-a56a-de8a248857c6">
    </h1> <p> </p>

  * ###### Private IP addresses :
    * ###### Private IP addresses are IP addresses that are used on a private network and are not accessible over the internet.
    * ###### These addresses are used to communicate between devices within private networks.
    * ###### Private IP addresses are not assigned by IANA or other authoritative organizations; instead, they are assigned by a specific network administrator.
    * ###### We cannot use private IP addresses directly on the internet because they are designed for use in closed networks that are not directly accessible to the internet. These addresses are only used for communication between devices within a specific network and are not intended for internet traffic.
    * ###### Finally, the range 127.0.0.0 - 127.255.255.255 is reserved for a special IP address "localhost". This IP address represents the self-connection of a device and usually refers to the local loopback interface of the computer. This address is usually used for local testing and development purposes and is not accessible over the internet. Therefore, this address is also one of the private IP addresses.
    <h1 align="center">
    <p>
        <img height="140" width="500" src="https://github.com/farukdll/NetPractice-Network/assets/97880185/4435cb8d-8ab8-4bd7-824e-6e6fb8164a27">
    </h1> <p> </p>


#### What are Network address and Broadcast address ? <a name="warnaabtadd"></a>
  * ###### Network address :
    * ###### The network address is the first IP address on the network, indicating that all devices on the same network belong to a common network.
    * ###### For example, "192.168.1.0" can be thought of as the network address. Here, "192.168.1" represents the network number and the next number "0" is the address of the first device on the network.
  * ###### Broadcast address :
    * ###### Broadcast address is a special IP address used to send messages or packets to all devices in a network, typically utilized in tasks such as network management, for instance, configuration updates or discovery requests. In IPv4, the broadcast address is usually the last IP address in a subnet; for example, if the IP address range of a subnet is 192.168.1.0/24, the broadcast address would be 192.168.1.255.
  * ###### For example :
    * ###### In a network with a subnet mask of 255.255.255.240, IP addresses are divided into 4-bit fields. This means that we can get 2^4, or 16 different values. However, since two addresses are reserved for the network address and the broadcast address, only 14 of these 16 addresses can be used.
    * ###### If a network address is 192.168.1.0 and the subnet mask is 255.255.255.240, the available IP addresses on this network are 192.168.1.1 through 192.168.1.14. 192.168.1.0 represents the network address, while 192.168.1.15 represents the broadcast address.
  * ###### Why can't we use the network address and broadcast address? Because these addresses are usually excluded from assignable IP addresses. Sending data to these addresses can unnecessarily increase network traffic and interfere with the normal communication of devices on the network. Therefore, network and broadcast addresses are usually excluded from assignable IP addresses and are not used for normal communication. Instead, these addresses are used by network routers and other network devices for internal network communication and routing.
  * ###### In simpler terms, the main reason for excluding network and broadcast addresses from assignable IP addresses is that these addresses are used  to route network traffic and facilitate internal network communication, rather than being directly used for communication between devices. For instance, a network address indicates that devices are connected to the network and is used by network devices like routers to route internal network traffic. The broadcast address, on the other hand, is used to send data to all devices on the network simultaneously but is typically not assigned to devices as a usable IP address. Utilizing these addresses differently from assignable IP addresses helps in organizing communication within the network and efficiently managing network traffic. Therefore, the primary reason these addresses are not used for direct communication is because they are reserved for routing operations by network routers and other network devices.


#### What is subnet mask ? <a name="wisubmaskkk"></a>
  * ###### Subnet mask is a structure used by network routers. This structure divides IP addresses into subnets and distinguishes between network and host sections while determining IP addresses within the same network for communication. For example, the "255.255.255.0" subnet mask specifies the network portion of the first three octets (24 bits) of the IP address and the host portion of the last octet (8 bits). This allows communication by identifying which network IP addresses belong to and facilitates the management of large networks.
  <h1 align="center">
  <p>
      <img height="400" width="600" src="https://github.com/farukdll/NetPractice-Network/assets/97880185/d9278719-16d4-4b88-835a-5b827b557b56">
      <img height="400" width="600" src="https://github.com/farukdll/NetPractice-Network/assets/97880185/826d616e-693f-4d5b-8daa-0675b7c9478e">
  </h1> <p> </p>


#### What is a switch ? <a name="wiasch"></a>
  * ###### Switches are devices that enable communication between devices on a network and manage data traffic. Each switch comes with multiple ports, and each port is a port to which a device can connect. For example, different devices such as computers, printers, servers and other network devices can be integrated into the network by connecting to one of these ports.
  * ###### When a data packet reaches a switch, the switch first looks at the destination MAC address of the packet and determines the port associated with this MAC address. Then, the switch forwards the packet only to the destination device. During this process, the switch also records the port on the incoming direction, so it knows from which port to receive the packet on the return path. For example, when one computer sends a file to another computer, the switch identifies the MAC address of the sending computer and forwards the packet directly to the receiving computer. Then, when the receiving computer sends a response packet, the switch forwards the incoming packet to the previously determined exit port, allowing the incoming packet to be delivered directly to the sending computer. This process optimizes network traffic, prevents unnecessary transmissions, and accelerates data communication.
  <h1 align="center">
  <p>
      <img height="250" width="700" src="https://github.com/farukdll/NetPractice-Network/assets/97880185/8089135d-2156-404c-ba9a-fee7f5096de0">
  </h1> <p> </p>


#### What is a router ? <a name="wiarer"></a>
  * ###### Routers are devices that enable data transmission in computer networks. They enable communication between computers, servers and other network devices by routing data communication between different networks.
  * ###### When a data packet arrives at the router, the router first looks at the destination IP address of the packet and determines the network where the device with that IP address is located. Next, the router performs traffic checks on the network, then determines the most appropriate path to route the packet and ensure that it is forwarded to the correct destination. This process regulates data traffic on the network, optimizes network resources, and ensures secure and efficient data transmission. In addition, routers often provide network security functions and monitor, manage and control data traffic on the network. They prevent unnecessary transmissions and speed up data communication.
  <h1 align="center">
  <p>
      <img height="250" width="700" src="https://github.com/farukdll/NetPractice-Network/assets/97880185/1b200284-425c-4a14-b82d-029b3cf4c8e2">
  </h1> <p> </p>


#### What is the difference between a switch and a router? <a name="hasarwwitdbt"></a>
  <h1 align="center">
  <p>
      <img width="160" alt="Switch" src="https://user-images.githubusercontent.com/97880185/211656464-3daa6f82-578b-4c6b-8d54-ff28b93e670f.png">
      <img width="150" alt="Router" src="https://user-images.githubusercontent.com/97880185/211656451-11235c84-f555-427b-916e-93a428a816b9.png">
  </h1> <p> </p>

  * ###### Switch :
    * ###### Manages data transmission between devices on the network. It uses MAC addresses to forward data packets between different devices and deliver them to the destination device.
    * ###### It usually operates at the second layer of the network (data link layer). It works with MAC addresses and connects devices on the network over physical links.
    * ###### Data transmission between devices usually takes place within the same network. So a switch enables communication between devices on the same network.
    * ###### Recognizes and manages devices using MAC (Media Access Control) addresses.
    * ###### It can directly connect multiple devices and manage traffic density on the network.
    * ###### It simply routes incoming packets based on the destination MAC address.
  * ###### Router :
    * ###### Manages the transmission of data between different networks. It uses IP addresses to forward and route data packets between two or more different networks.
    * ###### It operates at the third layer of the network (network layer). It works with IP addresses and enables communication between different networks.
    * ###### Data is transmitted between different networks. So the router enables and routes communication between different networks.
    * ###### It routes between different networks using IP (Internet Protocol) addresses.
    * ###### It is often used as a gateway and can connect multiple switches or devices.
    * ###### It routes incoming packets according to the destination IP address, and this routing process is usually more complex because it communicates between different networks.
  <h1 align="center">
  <p>
      <img height="400" width="600" src="https://github.com/farukdll/NetPractice-Network/assets/97880185/925598ec-420c-403d-b017-e709df7c4453">
  </h1> <p> </p>


#### What is a diversion table ? <a name="wiadttle"></a>
  <h1 align="center">
  <p>
      <img height="250" width="600" src="https://github.com/farukdll/NetPractice-Network/assets/97880185/332020d9-35db-44a5-8e32-9c1219863545">
  </h1> <p> </p>
  
  * ###### A routing table is a data table that lists the paths taken by devices on a network to reach specific destinations. Each entry specifies the address of the destination network and the next hop that packets should use to reach that network.
    * ###### Destination :
      * ###### This indicates the address of the network and the CIDR (Class IIDR) of the network the packet wants to reach. For example, the entry "190.3.2.252/30" specifies a route for packets to be routed to the address 190.3.2.252 and the CIDR of the network where this address is located.
    * ###### Next Hop :
      * ###### This specifies the next router or gateway address to which packets should be routed to reach a specific destination network. For example, the entry "192.168.1.1" indicates the next router address that will be used to access the network 190.3.2.252/30. 

#### Questions and Solutions : <a name="quesaslti"></a>
<details>
  <summary>Level 1</summary>
  <br>
  <img width="1223" alt="Level-1" src="https://user-images.githubusercontent.com/97880185/212213694-7524003c-d261-4f73-ae1b-df7a0012a9ac.png">
  <br> 
</details>

---
<details>
  <summary>Level 2</summary>
  <br>
  <img width="1223" alt="Level-2" src="https://user-images.githubusercontent.com/97880185/212213738-7536bda7-3bbf-4910-95d1-d689836d0856.png"> 
  <br>
</details>

---
<details>
  <summary>Level 3</summary>
  <br>
  <img width="1223" alt="Level-3" src="https://user-images.githubusercontent.com/97880185/212213866-f30c18c5-5ad7-4205-a0c1-b915e0293dcd.png">
  <br>
</details>

---
<details>
  <summary>Level 4</summary>
  <br>
  <img width="1223" alt="Level-4" src="https://user-images.githubusercontent.com/97880185/212213928-5cec0a99-ce40-4f20-89d7-2368cdde68ba.png">
  <br> 
</details>

---
<details>
  <summary>Level 5</summary>
  <br>
  <img width="1321" alt="Level-5" src="https://user-images.githubusercontent.com/97880185/212213967-74620659-7f35-40ef-ad5e-bf7c4d420045.png">
  <br>
</details>

---
<details>
  <summary>Level 6</summary>
  <br>
  <img width="1241" alt="Level-6" src="https://user-images.githubusercontent.com/97880185/212214010-98d800ca-b6af-4876-8bdd-6f95b66ce1b5.png">
  <br>
</details>

---
<details>
  <summary>Level 7</summary>
  <br>
  <img width="1419" alt="Level-7" src="https://user-images.githubusercontent.com/97880185/212214041-19c5b633-6f48-4a15-90e4-387a1a344180.png">
  <br> 
</details>

---
<details>
  <summary>Level 8</summary>
  <br>
  <img width="1126" alt="Level-8" src="https://user-images.githubusercontent.com/97880185/212214101-7c97ee4e-791d-454a-8a23-54a15be54024.png">
  <br>
</details>

---
<details>
  <summary>Level 9</summary>
  <br>
  <img width="1101" alt="Level-9" src="https://user-images.githubusercontent.com/97880185/212214179-ac1a2755-4994-46e4-bed1-a2fef5b4913f.png">
  <br>
</details>

---
<details>
  <summary>Level 10</summary>
  <br>
  <img width="1124" alt="Level-10" src="https://user-images.githubusercontent.com/97880185/212214241-bcca2d94-e5dd-4f18-a8be-eb9bc1b89794.png">
  <br>
</details>

---










|[ ⬆︎  Up](#up)|
|      :-:     |
