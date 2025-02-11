### 16 Layer 4: Transport Layer

Layer 4 is the dividing line between the upper layers and the lower layers of the OSI model.

- Segments are our data type within this transport layer.

#### **Protocols in the Transport Layer**
- **TCP - Transmission Control Protocol**
  - Reliable, connection-based protocol that uses a **3-way handshake** (SYN, SYN-ACK, ACK).
  - Ensures segment retransmission if acknowledgment is not received.
  ![Alt text](https://scaler.com/topics/images/steps-of-a-3-way-handshake-for-establishing-the-connection.webp)


- **UDP - User Datagram Protocol**
  - Connectionless, unreliable protocol for audio and video streaming.
  - No handshake, no acknowledgment, and less overhead.

#### **TCP vs UDP**
- **TCP**: Reliable, connection-oriented, supports retransmission and sequencing.
- **UDP**: Unreliable, connectionless, no retransmission or sequencing.

#### **Windowing**
- Adjusts segment size to optimize bandwidth and throughput.
- Reduces retransmissions by limiting the amount of data sent at once.

### **Buffering**

- Occurs when devices allocate memory to store segments if bandwidth is not readily available
- Data is stored temporarily in a buffer before being sent to its destination
- Buffer compensates for speed differences between the sender and receiver
- Buffers help prevent data loss when networks are congested or latency occurs

## Benefits Of Buffering

- Smoothens data flow in case of varying network speeds
- Reduces packet loss by temporarily holding data
- Prevents jitter in real-time applications like VoIP or video conferencing

---

## **Layer 4 Devices**

- **TCP and UDP** - Protocols operating in Layer 4
- **WAN Accelerators** - Apply compression to IP packets and send the segments over WAN accelerators to improve network speed
- **Load Balancers** - Distribute network traffic across multiple servers using transport layer information
- **Firewalls** - Inspect transport layer information (like TCP/UDP port numbers) to allow or block traffic

