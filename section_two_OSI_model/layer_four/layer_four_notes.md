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

#### **Buffering**
- Allocates memory for storing segments when bandwidth is limited.
