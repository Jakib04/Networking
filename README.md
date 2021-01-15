# OSI model
![layered image](https://media.geeksforgeeks.org/wp-content/uploads/computer-network-osi-model-layers.png)

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







