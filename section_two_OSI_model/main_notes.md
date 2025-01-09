# OSI Model Overview

## 12 OSI Model Overview (Objective 1.1)

The **OSI (Open System Interconnection) Model** is a framework used to understand and troubleshoot networking concepts. In Domain 1, Networking Concepts, Objective 1.1 emphasizes explaining concepts related to the OSI Reference Model.

### Importance of the OSI Model
- The 7 layers of the OSI model are invaluable during troubleshooting. By understanding each layer, you can pinpoint where issues occur in the network.

### Mnemonic to Remember the Layers:
- **P**lease = Physical Layer 1 (BITS)
- **D**o = Data Link Layer 2 (FRAME)
- **N**ot = Network Layer 3 (PACKET)
- **T**hrow = Transport Layer 4 (SEGMENT)
- **S**ausage = Session Layer 5 (DATA)
- **P**izza = Presentation Layer 6 (DATA)
- **A**way = Application Layer 7 (DATA)

### Key Note
While networks facilitate data flow, the terminology for "data" changes as it moves through different layers of the OSI model.

---

## 13 Layer 1: Physical Layer

The **Physical Layer** is where bits are transmitted across the network. This layer includes physical and electrical network characteristics.

### Transition Modulation
- Represents 1s and 0s:
  - **Copper Wire:** Voltage levels (e.g., 0V = 0, ±5V = 1)
  - **Fiber Optic Cables:** Light = 1, No Light = 0

### Physical Cabling
- **Common Cables:** CAT5 and CAT6 with RJ-45 connectors.
- **Wiring Standards:**
  - **TIA/EIA-568A**
  - **TIA/EIA-568B**

#### Cable Types:
- **Crossover Cable:** One end uses 568A, the other 568B.
- **Straight-Through/Patch Cable:** Both ends use 568B.

### Physical Topology
- Consider the layout of the network:
  - **Bus, Star, Ring, Full Mesh, Partial Mesh**

### Synchronization
- **Asynchronous Communication:** Uses start and stop bits for transmission.
- **Synchronous Communication:** Uses a reference clock to synchronize sender and receiver.

### Bandwidth Utilization
- **Broadband:** Divides bandwidth into separate channels (e.g., CATV).
- **Baseband:** Uses all frequencies of the cable at all times with a reference clock.

### Multiplexing
- Allows multiple users to share a connection efficiently.

#### Types of Multiplexing:
- **Time Division Multiplexing (TDM):** Sessions take turns using time slots.
- **Statistical Time-Division Multiplexing (statTDM):** Dynamically allocates time slots based on need.
- **Frequency Division Multiplexing (FDM):** Divides the medium into frequency-based channels.

### Examples of Layer 1 Devices
#### Media (Cables)
- **Fibre Optic**
- **Ethernet**
- **Coaxial**

#### Wireless
- **Bluetooth**
- **Wi-Fi**
- **Near Field Communication (NFC)**

#### Infrastructure Devices
- **Hubs:** Repeat received signals.
- **Access Points (APs):** Provide wireless connectivity.
- **Media Converters:** Convert media types (e.g., fiber to Ethernet).

---


# Layer 2 (Data Link Layer)

## Data Link Layer (Layer 2)

The Data Link Layer is responsible for:

- Packaging bits from Layer 1 into frames and transmitting them across the network.
- Performing error detection and correction.
- Identifying devices using MAC addresses.
- Providing flow control to ensure smooth data transmission.

## MAC Address (Media Access Control Address)

A MAC address is a physical identifier that allows a device to operate on a logical topology. Key points about MAC addresses include:

- A unique 48-bit physical addressing system assigned to every network interface card (NIC).
- Written in hexadecimal format:
  - **First 24 bits**: Identify the manufacturer (Organizationally Unique Identifier).
  - **Remaining 24 bits**: Identify the specific device.
- Crucial for logical topology, as it identifies devices within the network.

## Logical Link Control (LLC)

The LLC sublayer provides critical connection services, including:

- Acknowledging message receipt and ensuring controlled data flow.
  - Implements basic flow control by limiting the data sent by a sender and preventing the receiver from being overwhelmed.
  - Uses a checksum to detect corrupted data frames.

## Synchronization Methods at Layer 2

### Isochronous Mode
- Uses a common reference clock.
- Allocates time slots for transmissions.
- Reduces overhead during communication.

### Synchronous Method
- Devices share the same clock for synchronization.
- Utilizes control characters and markers to define the beginning and end of data frames.

### Asynchronous Method
- Devices operate based on their own clock cycles.
- No strict timing control for communication.

## Layer 2 Devices

### Network Interface Cards (NICs)
- Provide the hardware interface for network connectivity.

### Bridges
- Connect and filter traffic between different network segments.

### Switches
- Use intelligent logic to learn and direct data to specific devices based on their MAC addresses.
- Operate using Content Addressable Memory (CAM) tables to map MAC addresses to physical ports.
- Enable selective data transmission to targeted areas of the network, improving efficiency.
