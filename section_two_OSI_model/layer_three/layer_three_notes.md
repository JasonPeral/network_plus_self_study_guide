## OSI = Open System Interconnection Model 

### 12 OSI Model Overview (Objective 1.1)

We will be focused on domain 1 Networking Concepts, specifically Objective 1.1, which states we must be able to explain concepts related to the OSI Reference Model.

- The 7 layers of the OSI reference model are useful during our troubleshooting process. When we have a problem, we can use our knowledge of all the different layers to pinpoint what might be going on.

- **Mnemonic to remember the layers:**
  - **P**lease = Physical Layer 1 (BITS)
  - **D**o = Data Link Layer 2 (FRAME)
  - **N**ot = Network Layer 3 (PACKET)
  - **T**hrow = Transport Layer 4 (SEGMENT)
  - **S**ausage = Session Layer 5 (DATA)
  - **P**izza = Presentation Layer 6 (DATA)
  - **A**way = Application Layer 7 (DATA)
  
- At a certain point within the OSI model, the term "data" changes. See above for when the names change.

---

### 13 Layer 1: Physical Layer

This is where bits are transmitted across the network and includes physical and electrical network characteristics.

#### **Transition Modulation**
- The switch between levels to represent `1` or `0`.
  - Copper wire uses voltages:
    - `0V = 0`, `±5V = 1`
  - Fiber optic cables use:
    - `Light = 1`, `No Light = 0`

#### **Physical Cabling**
- **CAT5 and CAT6 cables** use an RJ-45 connector.
- Cabling standards:
  - **TIA/EIA - 568A**
  - **TIA/EIA - 568B**

#### **Types of Cables**
- **Cross-over Cable**: One end is `568A`, the other is `568B` (for device-to-device communication).
- **Straight-through Cable (Patch Cable)**: Uses `568B` on both ends (for devices connecting to a switch or router).

#### **Physical Topology**
- Network topology considerations: Bus, Star, Ring, Full Mesh, Partial Mesh.

#### **Synchronization**
- **Asynchronous Communication**: Uses start/stop bits to indicate transmissions.
- **Synchronous Communication**: Uses a reference clock to coordinate transmissions.

#### **Bandwidth Utilization**
- **Broadband**: Divides bandwidth into separate channels (e.g., CATV).
- **Baseband**: Uses all frequencies at all times, often synchronous.

#### **Multiplexing**
- **Time Division Multiplexing (TDM)**: Time slots for data sharing.
- **Statistical Time Division Multiplexing (statTDM)**: Dynamically assigns time slots.
- **Frequency Division Multiplexing (FDM)**: Divides medium into frequency-based channels.

#### **Examples of Layer 1 Devices**
- **Cables**: Fiber Optic, Ethernet, Coaxial.
- **Wireless**: Bluetooth, Wi-Fi, NFC.
- **Infrastructure Devices**: Hubs, Access Points, Media Converters.

---

### 14 Layer 2: Data Link Layer

#### **Functions of Layer 2**
- Packages data from the **Physical Layer** and transmits frames on the network.
- Provides **error detection, MAC addressing, and flow control**.

#### **MAC Address (Media Access Control)**
- Unique **48-bit** identifier assigned to network interfaces.
- MAC addresses are written in **hexadecimal** (e.g., `D2:51:F1:3A:34:65`).
- First **24 bits** identify the manufacturer; last **24 bits** identify the specific device.

#### **Logical Link Control (LLC)**
- Ensures reliable data flow with **acknowledgments, error detection, and retransmission**.

#### **Layer 2 Synchronization Schemes**
1. **Isochronous** - Uses a reference clock for precise timing.
2. **Synchronous** - Uses a shared clock and control characters.
3. **Asynchronous** - Uses independent clocks with start/stop bits.

#### **Layer 2 Devices**
- **Network Interface Cards (NICs)**
- **Bridges**
- **Switches**

---

### 15 Layer 3: Network Layer

#### **Overview**
- Focused on **routing** and forwarding data using **logical addresses (IP addresses)**.
- Uses **IPv4 and IPv6** for logical addressing.

#### **Switching and Routing Methods**
- **Packet Switching**: Divides data into packets, forwards based on IP.
- **Circuit Switching**: Dedicated link between devices (e.g., phone calls).
- **Message Switching**: Messages are stored and forwarded (like postal mail).

#### **Route Discovery and Selection**
- Routers maintain a **routing table** to determine the best path.
- **View routing table on macOS:**
    ```sh
    netstat -rn
    ```
- **Dynamic Routing Protocols:** RIP, OSPF, EIGRP.

#### **Connection Services at Layer 3**
- **Flow Control**: Prevents overwhelming the receiver.
- **Packet Reordering**: Ensures correct order of received packets.

#### **ICMP (Internet Control Message Protocol)**
- Used for error messages and network diagnostics.
- **PING**: Tests connectivity and response times.
- **Traceroute**: Traces the route of a packet through the network.

#### **Layer 3 Devices and Protocols**
- **Devices**: Routers, Multi-layer switches.
- **Protocols**: IPv4, IPv6, ICMP.

---
