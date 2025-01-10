### About this Layer

- Packages data from the physical layer (Layer 1) and transmits those frames on the network.
- Performs error detection and correction, identifies devices using MAC addresses, and provides flow control.

### MAC Address (Media Access Control Address)

- A means for identifying a device physically and allowing it to operate on a logical topology.
- Every manufacturer of a network card must assign a unique 48-bit physical address system to every network interface card they produce.
  - MAC addresses are always written in hexadecimal.
  - Each of the letters and numbers is considered 4 bits.
  - **Example:** `D2:51:F1:3A:34:65`
  - The first 24 bits identify the manufacturer who made the card (e.g., `D2:51:F1`).
  - The second 24 bits represent the exact machine that this MAC belongs to.
  - MAC is crucial for logical topologies—identifying devices on the network.

### Logical Link Control (LLC)

- Provides connection services and allows recipients to acknowledge the messages at the destination, ensuring data flow.
- LLC is the most basic form of flow control:
  - Limits data sent by a sender to prevent receiver overwhelm.
- Uses checksums to detect corrupted data frames; if detected, the recipient will request a retransmission of those frames.

### Communication Across Layer 2 Can Be Synchronized According to 3 Different Schemes

#### 1. Isochronous Mode

- Networks use a common reference clock, similar to synchronous communication.
- They create time slots for transmission, similar to Time Division Multiplexing (TDM).
- Less overhead compared to the other two schemes since devices know when and how long they can communicate.

#### 2. Synchronous

- Devices use the same clock with beginning and ending frames and special control characters for synchronization.
- These characters indicate when communication starts and ends.

#### 3. Asynchronous

- Devices reference their own clock cycles, using their own start and stop bits.
- No real control over when devices can and can't communicate.

---

### Layer 2 Devices

- Network Interface Cards (NICs)
- Bridges
- Switches
