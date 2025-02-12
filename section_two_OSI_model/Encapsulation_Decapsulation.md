### Encapsulation

- Is the process of putting headers and sometimes trailers around data
- An example can be if we want to send mail to our friend. We have to put it inside an envelope to be able to send it securely. Putting it in an envelope is the encapsulation process

### Decapsulation

- Removing the applied encapsulation to access the original data

### OSI Model Layers

- When moving down from Layer 7 to Layer 1 we are encapsulating our data
- When moving up from Layer 1 to Layer 7 we are decapsulating our data

### Protocol Data Unit (PDU)

- A single unit of information transmitted within a computer network
    - PDUs are formatted or written as L(Layer number) PDU
    - Example for Layer 7 PDU → `L7 PDU`

- There are some special names for the PDUs for layers 1, 2, 3, and 4:
    - **Layer 1** - Bits
    - **Layer 2** - Frames
    - **Layer 3** - Packets
    - **Layer 4** - Segments (TCP) or Datagrams (UDP)

### TCP Header (Layer 4)

- There are 10 mandatory fields within this header, totaling 20 bytes of information:
    - **Source Port**
    - **Destination Port**
    - **Sequence Number**
    - **Acknowledgment Number**
    - **TCP Data Offset**
    - **Reserved Data** — Always set to zero
    - **Control Flags**
        - **SYN** - Synchronizes connection in a 3-way handshake
        - **ACK** — Acknowledgment of the successful receipt of data
        - **FIN (Finished)** - Tears down connection created by a 3-way handshake
        - **RST (Reset)** — Used when an unexpected packet is received
        - **PSH (Push)** — Ensures data is given priority
        - **URG (Urgent)** — Identifies incoming data as urgent
    - **Window Size**
    - **TCP Checksum**
    - **Urgent Pointer**
    - **mTCP** - Optional

### UDP Header (Layer 4)

- 8-byte header:
    - **Source Port**
    - **Destination Port**
    - **Length** — Indicates the total packet bytes
    - **Checksum** — Not mandatory

### IP Header (Layer 3)

- Contains various fields:
    - **IP Version**
    - **Length of IP Header**
    - **Type of Service**
    - **Total Length of Packet and Header**
    - **Identifier**
    - **Flags**
    - **Fragmented Offset**
    - **Time to Live (TTL)**
    - **Protocol**
    - **Header Checksum**
    - **Source IP Address**
    - **Destination IP Address**
    - **Options and Padding**

### Ethernet Header (Layer 2)

- Features a few things:
    - **Destination MAC Address**
    - **Source MAC Address**
        - **About MAC Addresses**
            - Physical address that is used to identify a network card on a local area network
            - Processed by switches
    - **EtherType Field**
        - Used to indicate which protocol is encapsulated in the payload of a frame
            - IPv4 or IPv6
    - **VLAN Tag** - Optional
        - Uses either:
            - IEEE 802.1Q
            - IEEE 802.1AD
