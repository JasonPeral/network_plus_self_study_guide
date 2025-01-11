## Layer 3 (Network Layer)

### Network Layer (Layer 3)

- Concerned with routing and forwarding traffic using logical addresses.

### Logical Addressing

- **IP Variants** – Common logical addressing schemes:
  - **IPv4** – Written in dotted octet notation with four sets of numbers separated by dots (e.g., `172.16.254.1`).
  - **IPv6** – Next-generation IP addressing.

- **Other Protocols** (Replaced by IP):
  - **AppleTalk**
  - **IPX** (Internetwork Packet Exchange)

### Switching/Routing Methods

- **Packet Switching (Routing):**
  - Data is divided into packets and then forwarded.
  - Most commonly used method.

- **Circuit Switching:**
  - A dedicated communication link is established between two devices.

- **Message Switching:**
  - Data is divided into messages, which may be stored and then forwarded.

### Route Discovery and Selection

- Routers maintain **routing tables** to determine the best path.
  - **Dynamic protocols** (e.g., RIP, OSPF) enable routers to share and update route information.
- **Routing protocols** help decide how data flows across the network and how routers communicate that information.

### Connection Services at Layer 3

- **Augments Layer 2 services** by adding:
  - **Flow control** to prevent the sender from overwhelming the receiver.
  - **Packet reordering** to ensure data packets arrive and are reassembled in the correct order.

### Internet Control Message Protocol (ICMP)

- Used for sending **error messages** and **operational information** to an IP destination.
  
- **PING**
  - Most commonly used ICMP tool.
  - Helps troubleshoot network issues by testing **connectivity** and **response times**.

- **Traceroute**
  - Traces the route of a packet through the network.

### Devices and Protocols

- **Routers**
- **Multi-layer Switches:**
  - Combines Layer 2 switch and Layer 3 router features.
  - A switch is always a Layer 2 device unless specified as a **multi-layer switch**, making it a Layer 3 device.

- **Layer 3 Protocols:**
  - **IPv4**
  - **IPv6**
  - **ICMP**

- **Common Layer 3 Devices in Exams:**
  - **IP** and **Routers**
