### Layer 3 is all about routing

- We are going to be focused on how we forward traffic (routing) using logical addresses
    - For example, our computers have an IP address, and it's going to either be an IPv4 or an IPv6 or both (both are considered Layer 3 protocols)

---

### Logical Addressing

- IP variants — common logical addressing schemes
    - **IPv4**
        - Written in dotted octet notation, which is 4 sets of numbers separated by dots (e.g., 192.168.0.0)
    - **IPv6**
        - The latest version of IP with a much larger address space
    - These two are the most common, but they are not the only logical addressing schemes that exist.

---

### Switching/Routing Methods

- **Layer 3 switching (routing)**
    - Switches, the physical device, are Layer 2 devices.
    - Switching (routing) is how we transfer data in Layer 3.

- **Packet Switching**
    - Data is divided into packets and forwarded based on its IP address.
    - Most commonly used method of switching.

- **Circuit Switching**
    - A dedicated communication link is established between two devices.
    - An example of circuit switching could be a phone call, where a dedicated and constant communication path is maintained for the duration of the conversation.

- **Message Switching**
    - Data is divided into messages, which may be stored and then forwarded.
    - For example, if mail is sent to a closed post office, it would be stored until the post office opens. If this were packet switching, the mail sent to a closed post office would be shredded or deleted.

---

### Route Discovery and Selection

How we are going to decide which network path to take to send that “message”.

- **Routers maintain a routing table** for determining the best path based on the destination IP the packet wants to get sent to.
    - Dynamic protocols (e.g., RIP, OSPF, EIGRP) enable routers to share and update route information.
- **Routing protocols** help decide how data is going to flow across the network and how the routers are going to communicate that information.

---

### Connection Services at Layer 3

- Augment Layer 2 connection services and provide improved reliability.
- **Improves flow control**
    - Prevents the sender from overwhelming the receiver by ensuring the sender doesn’t send packets faster than the receiver can process them.
- **Packet Reordering**
    - Ensures data packets arrive and are reassembled in the correct order.

---

### ICMP — Internet Control Message Protocol

- Used for sending error messages and operational information to an IP destination.
- Most commonly used ICMP command is:
    - **PING**
        - Helps troubleshoot network issues by testing connectivity and response times.
    - **Traceroute**
        - Traces the route of a packet through the network.

---

### Devices and Protocols on Layer 3

- **Routers**
- **Multi-layer switches**
    - Combines Layer 2 switch and Layer 3 router features.
    - A physical switch is always a Layer 2 device unless specifically mentioned as a multi-layer switch; then it is considered a Layer 3 device.
- **Protocols**
    - IPv4
    - IPv6
    - ICMP

---

### Exam Relevance

- **IP** and **routers** are commonly encountered Layer 3 concepts (both devices and protocols) on networking certification exams, including the CompTIA Network+ exam.
