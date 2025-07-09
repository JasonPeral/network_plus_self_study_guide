# Ethernet Fundamentals

*Ethernet emerged as the dominant protocol for L2 communication in LANs*

### Core Summary

Deterministic access == Organized and predictable without collisions

Contention Based Access == Chaotic but more efficient use of bandwidth 

CSMA/CD == Allows devices to listen, detect and manage network collisions

Ethernet switches allows us to break the network into smaller collision domains which == efficient network

---

### Evolution / some history

- Initially ethernet was ran over coxial cables that used BNC connectors and vampire tabs (10Base2 Thinnet || 10Base5 Thicknet)
- **Transitioned to 10Base-T Ethernet**
    - Used twisted pair cables(category 3 / Cat 3)
    - Speeds of up to 10Mbps which was significantly fast for the time(1980)
    - The only issue presented with 10Base-T was that it could only cover a distance of up to 100 meters before having to be repeated by a hub or a switch.

---

### Deterministic vs Contention based access

- **Deterministic Access**
    - Network access method where devices transmit in an organized, predictable manner without collisions (e.g Token Ring)
    - Each device has a reserved time slot to transmit frames(since its L2)
    - An example can be a classroom with students and a professor, the teacher only allows people to speak when they raise their hand and are given a token. Once done, they give the token back and they cant communicate anymore.
- Contention Based Access
    - Used to determine who gets to access and communicate on the network at any given time
    - Chaotic, but more efficient use of bandwidth which == less overhead (e.g Ethernet based)
    - Can have collisions in the communication
    - An example can be having a conversation with 5 friends, although there is no moderation about who gets to speak and when its just known that when theres a gap in the conversation its okay to start speaking.

---

### Carrier Sense Multiple Access with Collision Detection (CSMA/CD)

- Allows devices to detect collisions by “listening” to the network and manages network access accordingly and retrying after a random backoff time.
- Carrier Sensing (CS)
    - Devices will be listing for existing transmissions
    - Carrier == signals that carries information or data
- Multiple Access (MA)
    - Many devices share the same communication medium and can attempt to access the network simultaneously
- Collision Detection (CD)
    - Devices will listen, detect and handle collisions
    - Random Back-off Timer
        - Devices that detect collision pause and select a random back-off time before re-transmitting data
        - This allows the devices that were experiencing collisions to retransmit again when the back-off time hits 0

---

### Collision Domain

- Area of a network where collisions can occur over the same shared medium.

### Ethernet Switches

- We break networks into smaller collision domains with switches which in-turn improves efficiency of the network.
- Each switch port is its own collision domain, this allows full-duplex communication(Ability to transmit and receive data simultaneously on the same connection)

---

### Key Notes

- Ethernet is the primary L2 protocol for modern networks
- Switches are preferred over hubs for efficient network/collision traffic management