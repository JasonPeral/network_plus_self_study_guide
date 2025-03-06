## User Datagram Protocol (UDP)

### **Definition and Core Summary**

- A communication protocol that is used across the internet for very time-sensitive data transmission like video transmission or DNS lookups.
    - UDP is ideal for applications that need and prioritize speed over error checking and packet retransmission.
    - UDP has less overhead in processing and has low latency.
    - Does not have the error checking and recovery services like TCP does.
- UDP operates on the transport layer (4) of the OSI model just like TCP.
- Connectionless communication model.

---

### **Packet Structure of UDP**

- Data packets are known as **Datagrams**.
    - Datagrams are sent without prior setup of transmission channels.
    - A Datagram packet only contains the source and destination port numbers, length field, and checksum, so the headers are much smaller and simpler (8 bytes) compared to a TCP header (20-60 bytes).

---

### **UDP’s Stateless Nature**

- UDP does not maintain a connection state with an endpoint or track packets.
- Referred to as a "fire and forget" protocol.
- UDP does not wait for acknowledgments from the receiver/endpoint, which leads to faster transfer rates but is less reliable as datagram packets are not validated.

### **Reliability Trade-offs and Use Cases**

- UDP is less reliable only because there is a lack of packet tracking.
- This means UDP is suitable for scenarios where speed is crucial and packet loss is acceptable.
- **Use Cases:** Live broadcasts, online gaming, and VoIP calls. If there were retransmissions of packet losses in these use cases, it would have a more negative impact than a positive one.
