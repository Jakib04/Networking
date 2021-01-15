## OSI model
---
![](https://media.geeksforgeeks.org/wp-content/uploads/computer-network-osi-model-layers.png)

The Open Systems Interconnection (OSI) model describes seven layers that computer systems use to communicate over a network. It helps network device manufacturers and networking software vendors: Create devices and software that can communicate with products from any other vendor, allowing open interoperability.

 The important layers are 

 **Application Layer  :**

  At the very top of the OSI Reference Model stack of layers, we find Application layer which is implemented by the network applications. These applications produce the data, which has to be transferred over the network. Applications such as  Browsers, facebook works in this layer.

**Transport Layer  :**

   It is responsible for the End to End Delivery of the complete message. The data in the transport layer is referred to as Segments.
   This layer adds Sender and Receiver’s port number.

**Network Layer :**

  Network layer works for the transmission of data from one host to the other located in different networks. Segment in Network layer is referred as Packet. This layer adds Sender and Receiver’s IP address.Routers are device of this layer.

**Data Link Layer (DLL) :** 

  The data link layer is responsible for the node to node delivery of the message. DLL also encapsulates Sender and Receiver’s MAC address in the header. The Receiver’s MAC address is obtained by placing an ARP(Address Resolution Protocol) request onto the wire asking “Who has that IP address?” and the destination host will reply with its MAC address. Switch & Bridge are Data Link Layer devices.

**Physical Layer :**

   The lowest layer of the OSI reference model is the physical layer. It is responsible for the actual physical connection between the devices. The physical layer contains information in the form of bits. Hub, Repeater, Modem, Cables are Physical Layer devices.



## Browser sender port selection while establishing TCP connection
---
  A TCP connection consists of two endpoints, and each endpoint consists of an IP address and a port number. Therefore, when a client user connects to a server computer, an established connection can be thought of as the 4-tuple of (server IP, server port, client IP, client port).

  Usually three of the four are readily known -- client machine uses its own IP address and when connecting to a remote service, the server machine's IP address and service port number are required.
  What is not immediately evident is that when a connection is established that the client side of the connection uses a port number. Unless a client program explicitly requests a specific port number, the port number used is an ephemeral port number.

  An ephemeral port is a temporary communication hub used for Internet Protocol (IP) communications. It is created from a set range of port numbers by the IP software and used as an end client's port assignment in direct communication with a well-known port used by a server.
  After communication is terminated, the port becomes available for use in another session. However, it is usually reused only after the entire port range is used up.

  Different operating systems (OS) use different port ranges for ephemeral ports. Many Linux versions use port range 32768-61000, while Windows versions (until XP) use 1025-5000, by default.
  Later Windows versions, including Vista, Windows 7 and Server 2008, use the Internet Assigned Number Authority (IANA) suggested range of 49152-65535.

![](Images/D.png)




