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
