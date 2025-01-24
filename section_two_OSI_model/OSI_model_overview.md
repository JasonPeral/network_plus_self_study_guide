# OSI Model Overview

The OSI (Open Systems Interconnection) model is a conceptual framework that standardizes the functions of a communication system into seven distinct layers. Each layer serves specific purposes and interacts with the layers directly above and below it. Here's an overview of the seven layers:

---

## **1. Physical Layer**
- **Purpose**: Handles the transmission of raw binary data (bits) over a physical medium.
- **Key Responsibilities**:
  - Defines hardware specifications (e.g., cables, switches, hubs, connectors).
  - Manages data encoding, signaling, and bit synchronization.
  - Oversees the physical transmission medium (e.g., copper wire, fiber optics, radio waves).
- **Examples**: Ethernet cables, Wi-Fi signals, Bluetooth, USB.

---

## **2. Data Link Layer**
- **Purpose**: Ensures reliable data transfer between nodes on the same physical network.
- **Key Responsibilities**:
  - Frames data into manageable units.
  - Manages error detection and correction.
  - Controls access to the physical transmission medium (MAC - Media Access Control).
- **Examples**:
  - Protocols: Ethernet, PPP (Point-to-Point Protocol), ARP (Address Resolution Protocol).
  - Devices: Switches, network interface cards (NICs).

---

## **3. Network Layer**
- **Purpose**: Handles routing, addressing, and forwarding of data packets between networks.
- **Key Responsibilities**:
  - Determines the best path for data delivery.
  - Provides logical addressing (e.g., IP addresses).
  - Manages packet fragmentation and reassembly.
- **Examples**:
  - Protocols: IP (IPv4, IPv6), ICMP (Internet Control Message Protocol), OSPF (Open Shortest Path First), BGP (Border Gateway Protocol).
  - Devices: Routers.

---

## **4. Transport Layer**
- **Purpose**: Ensures end-to-end communication, reliability, and flow control.
- **Key Responsibilities**:
  - Segments data and reassembles it at the destination.
  - Provides error detection and correction for data integrity.
  - Implements flow control and congestion management.
- **Examples**:
  - Protocols: TCP (Transmission Control Protocol), UDP (User Datagram Protocol).

---

## **5. Session Layer**
- **Purpose**: Manages sessions or connections between applications.
- **Key Responsibilities**:
  - Establishes, maintains, and terminates communication sessions.
  - Handles session recovery and synchronization.
- **Examples**: Remote Procedure Call (RPC), NetBIOS, APIs for session management.

---

## **6. Presentation Layer**
- **Purpose**: Translates data between the application and the network in a format both can understand.
- **Key Responsibilities**:
  - Converts data formats (e.g., encryption, compression, encoding).
  - Ensures data is presented in a readable format.
- **Examples**: JPEG, PNG, ASCII, SSL/TLS (encryption standards).

---

## **7. Application Layer**
- **Purpose**: Provides interfaces for end-user applications to communicate over the network.
- **Key Responsibilities**:
  - Supports application services like email, file transfer, and web browsing.
  - Implements high-level protocols for communication.
- **Examples**:
  - Protocols: HTTP, FTP, SMTP, DNS, SNMP.
  - Applications: Web browsers, email clients, file transfer tools.



