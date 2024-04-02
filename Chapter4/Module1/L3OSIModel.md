Open Systems Interconnection (OSI) Model
The OSI Model was developed to establish a common way to describe the communication structure for interconnected computer systems. The OSI model serves as an abstract framework, or theoretical model, for how protocols should function in an ideal world, on ideal hardware. Thus, the OSI model has become a common conceptual reference that is used to understand the communication of various hierarchical components from software interfaces to physical hardware.

The OSI model divides networking tasks into seven distinct layers. Each layer is responsible for performing specific tasks or operations with the goal of supporting data exchange (in other words, network communication) between two computers. The layers are interchangeably referenced by name or layer number. For example, Layer 3 is also known as the Network Layer. The layers are ordered specifically to indicate how information flows through the various levels of communication. Each layer communicates directly with the layer above and the layer below it. For example, Layer 3 communicates with both the Data Link (2) and Transport (4) layers.

The Application, Presentation, and Session Layers (5-7) are commonly referred to simply as data. However, each layer has the potential to perform encapsulation. Encapsulation is the addition of header and possibly a footer (trailer) data by a protocol used at that layer of the OSI model. Encapsulation is particularly important when discussing Transport, Network and Data Link layers (2-4), which all generally include some form of header. At the Physical Layer (1), the data unit is converted into binary, i.e., 01010111, and sent across physical wires such as an ethernet cable.  

It's worth mapping some common networking terminology to the OSI Model so you can see the value in the conceptual model.

Consider the following examples: 

When someone references an image file like a JPEG or PNG, we are talking about the Presentation Layer (6). 
When discussing logical ports such as NetBIOS, we are discussing the Session Layer (5).
When discussing TCP/UDP, we are discussing the Transport Layer (4).
When discussing routers sending packets, we are discussing the Network Layer (3). 
When discussing switches, bridges or WAPs sending frames, we are discussing the Data Link Layer (2). 
Encapsulation occurs as the data moves down the OSI model from Application to Physical. As data is encapsulated at each descending layer, the previous layer’s header, payload and footer are all treated as the next layer’s payload. The data unit size increases as we move down the conceptual model and the contents continue to encapsulate.  
 
The inverse action occurs as data moves up the OSI model layers from Physical to Application. This process is known as de-encapsulation  (or decapsulation). The header and footer are used to properly interpret the data payload and are then discarded. As we move up the OSI model, the data unit becomes smaller. The encapsulation/de-encapsulation process is best depicted visually below: 

 -Application Layer:
  DATA
  The application layer in the OSI model is about the protocols that users interface with. That ends up being broad in scope. Protocols related to everything from email (SMTP, IMAP, and POP), to web browsing (HTTP and HTTPS), to IP address assignment (DHCP), to file transfer (FTP and TFTP), to text-based server administration (SSH), to authentication (LDAP) all reside at Layer 7.

  What data unit is associated with the session layer? Data.

  What protocols are associated with the presentation layer? SMTP, Telnet, HTTP(S), DHCP, FTP, SNMP, SSH, NTP, and LDAP

  What happens at the presentation layer? Users and devices interface with data sent between source and destination systems.

  What network devices are associated with the presentation layer? Servers, computers, load balancers, and Layer 7 firewalls
 
 
 
 -Presentation Layer:
  header+DATA
  Layer 6 deals with the way data is formatted or presented, it is also known as the syntax layer. This means concepts like ASCII encoding for text, encoding images as JPEG files, formatting data structures using XML, encryption/decryption, and compression/decompression happen here.

  What data unit is associated with the session layer? Data.

  What protocols are associated with the presentation layer? SSL & TLS (arguably)

  What happens at the presentation layer? Data is encrypted/decrypted, compressed, structured, and/or encoded/decoded before being passed up to Layer 7 or down to Layer 5.

  What network devices are associated with the presentation layer? Servers and computers
  
  
  

 -Session Layer:
  header+header+DATA
  As the name implies, the session layer is all about establishing and tearing down sessions. This gets murky because with TCP there is already a concept of "sessions" and those are what often get used in the real world. That being said, remote procedure calls (RPCs) are one example where you may run into the session layer in the wild.

  What data unit is associated with the session layer? Data. We're done with adding specific network headers from here on out.

  What protocols are associated with the session layer? SSL & TLS (arguably), SDP, SOCKS, PPTP, RPC, NetBIOS, and PAP.

  What happens at the session layer? Sessions are established and torn down. Data may be transformed to or from segments or datagrams as it makes its way to the transport layer.

  What network devices are associated with the session layer? Servers and computers
  
  


 -Transport Layer:
  TCP/UDP header+header+header+DATA Segments
  What data unit is associated with the transport layer? Segments for TCP. Datagrams for UDP. The encapsulation associated with the transport layer is the TCP or UDP headers used to describe the TCP or UDP connection.

  What protocols are associated with the transport layer? TCP and UDP.

  What happens at the transport layer? At Layer 4, end-to-end connections are established. Flow control, error-checking, and multiplexing can also occur at Layer 4. Between Layer 3 and Layer 4, packets are transformed to or from segments or datagrams. Between Layer 4 and Layer 5, segments or datagrams are transformed to or from protocol data units (PDUs).

  What network devices are associated with the transport layer? Load balancers and firewalls.





 -Network Layer:
  IPheader+TCP/UDP header+header+header+DATA Segment Packets
  What data unit is associated with the network layer? Frames. The IP header is the important addition here. The IP header, in addition to source and destination addresses, includes a protocol version, time to live (TTL), options, flags, and identification bits used to help reassemble packets.

  What protocols are associated with the network layer? IPv4, IPv6, ICMP (what ping uses), and IPsec.

  What happens at the network layer? Routing devices determine the best path for network traffic. Between the data link layer and the network layer, frames are transformed to, or from, packets. Similarly, between the transport layer and the network layer, packets are transformed to or from segments or datagrams.

  What network devices are associated with the network layer? Routers (Layer 3 switches)
 
 
 
 -Data Link Layer:
  MACheader+LLCheader+IPheader+TCP/UDPheader+header+DATA Segment Packet Frames+footerFCS
  The data link layer consists of two sublayers: the logical link control (LLC) and media access control (MAC) layers. The LLC layer handles flow control and error checking while the MAC layer determines what devices can send and receive data.

  Frames are the data unit of Layer 2. That means bits from Layer 1 and packets from Layer 3 are converted to and from frames here.

  MAC addresses, Layer 2 switching for LANs & WANs, and VLANs are some of the common Layer 2 concepts that come up regularly in day-to-day IT work.

  What data unit is associated with the data link layer? Frames. The frames at Layer 2 include information such as:

    -Preamble: This is a special series of zeros and ones that identifies the start of a frame. The idea here is that since this will never be seen in the middle of a frame, devices can reliably identify where they start.

    -Ethernet header: Includes the source and destination MAC addresses as well as a type. The type value lets us know what higher-level protocol we're dealing with. In most common cases, the type is IP.

    -Data: 46-1500 bytes of payload data. This is the data we're trying to deliver to the end user. If the payload is under 46 bytes, dummy data is added to the frame. The process of adding this dummy data is known as "padding."

    -FCS: The frame check sequence (FCS) is an algorithm, specifically a cyclic redundancy check (CRC), used for error detection.

  What protocols are associated with the data link layer? PPP, Ethernet (e.g. collision detection like CSMA/CD), Frame Relay, STP, ATM, ARP, and HDLC.

  What happens at the data link layer? Bits from the physical layer are converted to/from frames between Layer 1 and Layer 2. Packets are converted to/from frames between Layer 2 and Layer 3. MAC addresses are used to identify nodes.

  What network devices are associated with the data link layer? "Layer 2" switches, network interface cards (NICs), and modems.

  Pro tip: MAC addresses are a Layer 2 concept, and IP addresses are a Layer 3 concept. Understanding the difference between a Layer 2 switch and a router, basically comes down to that. Layer 2 switches deal with MAC addresses. Routers operate at Layer 3 and deal with IP addresses. With all the attention paid to Layer 2 and Layer 3 on modern networks, understanding this concept is important.
  
  
  
  
  
 -Physical Layer:
  header+(MACheader+LLCheader+IPheader+TCP/UDPheader+header+DATA Segment Packet Frames+footerFrameCheckSequence) in binary bits+footer
  The physical layer is where the "ones and zeros" are sent across copper or fiber cabling or radio waves like Wi-Fi signals. Devices here convert frames to bits and vice versa.

  What data unit is associated with the physical layer? Bits. Ones and zeros transported over a physical medium.

  What protocols are associated with the physical layer? Ethernet, Bluetooth, 802.11 (WiFi), SONET, T-carrier links (e.g. T1 and T3), and OTN.

  What happens at the physical layer? Frames from the data link layer are converted to bits to be transported across a physical medium (e.g. a cable) to another network. Once they reach their destination, the bits are converted back to frames to work their way back up the rest of the layers.

  What network devices are associated with the physical layer? Cabling, hubs, repeaters, wireless access points, and patch panels.


