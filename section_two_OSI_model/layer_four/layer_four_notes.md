# Layer 4 (Transport Layer)

## Transport Layer (Layer 4)

### Dividing Line in the OSI Model

- Acts as the dividing line between the **upper layers** and **lower layers** of the OSI model.

#### Upper Layers:
- **Transport**
- **Session**
- **Presentation**
- **Application**

### Segments

- **Data Type in Transport Layer:** Segments

### Protocols in Layer 4

#### **TCP (Transmission Control Protocol)**

- **Connection-oriented** protocol that reliably transports segments across the network.
- Implements **acknowledgment** mechanisms.
- Uses the **Three-Way Handshake**:
  - **SYN** – Synchronization
  - **SYN-ACK** – Synchronization-Acknowledgment
  - **ACK** – Acknowledgment
- Utilizes **Windowing** for flow control.
- Suitable for data that must reach its destination reliably.

#### **UDP (User Datagram Protocol)**

- **Connectionless** protocol that is **unreliable** for transporting segments (datagrams).
- Commonly used for **audio and video streaming**.
- No **Three-Way Handshake** and minimal overhead.
- Lacks acknowledgment and retransmission mechanisms.

### Data Types in Layer 4 (Important for Exam)

- **Segment** – Data type for **TCP**
- **Datagram** – Data type for **UDP**

### TCP vs. UDP

#### **TCP**

- **Reliable** communication
- Uses **Three-Way Handshake**
- **Connection-oriented**
- **Segment retransmission** and **flow control** through windowing
- Supports **sequencing** and **acknowledgment** of segments

#### **UDP**

- **Unreliable** communication
- No **Three-Way Handshake**
- **Connectionless**
- No **retransmission**, **windowing**, or **sequencing**
- No acknowledgment of datagrams

### Windowing

- Allows clients to adjust the data size in segments during transmission.
- Optimizes **throughput** and **bandwidth**.
- **Opens** or **closes** the window based on retransmissions.

### Buffering

- Occurs when devices allocate memory to store segments if bandwidth is limited.
- **Buffer:** Temporary storage for segments.
- Prevents overflow by clearing segments.

### Layer 4 Devices

#### **Protocols:**
- **TCP**
- **UDP**

#### **Devices:**
- **WAN Accelerators**
- **Load Balancers**
- **Firewalls**
