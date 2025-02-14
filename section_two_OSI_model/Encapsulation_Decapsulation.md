### Encapsulation

- Is the process of putting headers and sometimes trailers around data
- An example can be if we want to send mail to our friend. We have to put it inside an envelope to be able to send it securely. Putting it in an envelope is the encapsulation process

### Decapsulation

- Removing the applied encapsulation to access the original data

### OSI Model Layers

- When moving down from Layer 7 to Layer 1 we are encapsulating our data
- When moving up from Layers 1 to Layer 7 we are decapsulating our data

### Protocol Data Unit (PDU)

- A single unit of information transmitted within a computer network
    - PDUs are formatted or written as L(Layer number) PDU
    - Example for Layer 7 PDU → L7 PDU

- There are some special names for the PDUs for Layer 1, 2, 3, and 4:
    - Layer 1 - Bits
    - Layer 2 - Frames
    - Layer 3 - Packets
    - Layer 4 - Segments (TCP) or Datagrams (UDP)

### TCP Header (Layer 4)

- There are 10 mandatory fields within this header, totaling 20 bytes of information:
    - Source Port
    - Destination Port
    - Sequence Number
    - Acknowledgment Number
    - TCP Data Offset
    - Reserved Data — Always set to zero
    - Control Flags:
        - SYN - Synchronizes connection in 3-way handshake
        - ACK — Acknowledgment of the successful receipt of data
        - FIN (Finished) - Tears down connection created by 3-way handshake
        - RST (Reset) — Used when an unexpected packet is received
        - PSH (Push) — Ensures data is given priority
        - URG (Urgent) — Identifies incoming data as urgent
    - Window Size
    - TCP Checksum
    - Urgent Pointer
    - mTCP - Optional

### UDP Header (Layer 4)

- 8-byte header:
    - Source Port
    - Destination Port
    - Length — Indicates the total packet bytes
    - Checksum — Not mandatory

### IP Header (Layer 3)

- Contains various fields:
    - IP Version
    - Length of IP Header
    - Type of Service
    - Total Length of Packet and Header
    - Identifier
    - Flags
    - Fragmented Offset
    - Time to Live (TTL)
    - Protocol
    - Header Checksum
    - Source IP Address
    - Destination IP Address
    - Options and Padding

### Ethernet Header (Layer 2)

- Features a few things:
    - Destination MAC Address
    - Source MAC Address
        - About MAC Addresses:
            - Physical address that is used to identify a network card on a local area network
            - Allows our source to find our destination by using this type of Layer 2 addressing
            - Processed by switches
    - EtherType Field:
        - Used to indicate which protocol is encapsulated in the payload of a frame
            - IPv4 or IPv6
    - VLAN Tag - Optional:
        - Uses either:
            - IEEE 802.1Q
            - IEEE 802.1AD
- A frame being sent at Layer 2 will also contain a payload:
    - Data being sent across the network
    - In Ethernet, the minimum payload is 42 bytes if VLANs are being used
    - If no VLANs are being used, then the minimum payload is 46 bytes
    - When we are trying to send a payload, there is a maximum size for this known as an **MTU (Maximum Transmission Unit)**:
        - 1500 bytes for Ethernet
    - Should the payload exceed the MTU, then we would need to allow for what’s known as a **Jumbo Frame**:
        - Frames larger than 1500 bytes
        - Require reconfiguration of MTU

### Data Transmission

- As data moves from L7 to L1, the data undergoes encapsulation and also adds headers to each layer:
    - L4 - We add our Source/Destination Ports
    - L3 - Source/Destination IP Addresses
    - L2 - We add our Source/Destination MAC Addresses
    - L1 - We are transmitting our L2 frames as 1s and 0s over the medium
- When it is received by its next device, it starts to decapsulate L2 information by reading the Ethernet header. If the destination MAC is on one of the switch ports, for example, it routes that information there.
- If the destination MAC address is not on L2, it forwards it to its default gateway, which is a router.
- The router decapsulates its data to L3, and if the destination IP address is within the network, it forwards that information to the device. If not, the router re-encapsulates the data and sends it out its default gateway.
- Then, the process keeps on going until the destination is found.
