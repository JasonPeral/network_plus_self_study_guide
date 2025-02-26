# TCP

### **Definition and core summary**

- TCP is a fundamental protocol within the internet protocol suite that consists of a set of rules that govern the exchange of data
- Ensures reliable, ordered and error-checked data transmission between devices over a network by using
    - Error checking
    - Data sequencing
    - Acknowledgment
- TCP operates at the Transport Layer (L4) of our OSI model and it breaks down larger messages into smaller packets for efficient data transfer and reassembles them back at the destination

---

## Three way handshake

1. A client is going to send a SYN (synchronize) packet to the server to initiate communication session
2. The server will send back a SYN-ACK package letting the client know that the server is willing and ready to establish a connection 
3. The client will send an ACK back to the server to confirm the establishment of the connection 

- This 3-way handshake process ensures that both the sender and receiver are ready for data transmission and that the connection is reliable and secure

### Error checking and flow control

- **Error checking**
    - TCP uses a sequence number and acknowledgment message to assure the data is being received correctly and in the proper order
    - If it detects lost or corrupted packets, the protocol will notice that and require the sender to retransmit those lost packets
- **Flow Control**
    - This prevents the sender from overwhelming the receiver with too much data at one time
    - Flow control with TCP is achieved with a method called windowing
        - Controls the amount of data sent at a time
        - Allows for dynamic adjustment based on network conditions even while the connection is valid

## Ports

- A port is a numerical identifier for services or applications in the TCP/IP suite
- Distinguishes between different services or applications that are running on the same server/computer
- Each connection is identified by a source and destination IP address and port. For example, when connecting to GitHub, the client (source) will have a random ephemeral port, while GitHub's port will be associated with HTTPS (443)

## TCP’s Role within Internet Communication

- Ensures reliability and ordered delivery of data between client and server
- Always remember that TCP operates at the transport layer of the OSI model (Layer 4)
- Utilizes packetization, acknowledgment, and error checking
- The 3-way handshake is a very important concept of TCP as it establishes and ensures a reliable secure connection
- Ports facilitate the logical differentiation of services or applications running on a machine/device
