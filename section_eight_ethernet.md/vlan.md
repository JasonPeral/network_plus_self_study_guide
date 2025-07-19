# VLAN

### Core summary

- **VLANs logically segment a network into separate broadcast domains at Layer 2(Data Link || frame)**, enabling grouped devices without regard to physical cabling location on a switch .
- **They reduce hardware needs** (vs. traditional LANs) by enabling multiple VLANS to share the same switch using trunking (802.1Q tagging).
- **Each VLAN frame is tagged with a VLAN ID**, allowing switches to route traffic within the correct VLAN.
- **Benefits of VLANs** include enhanced security, performance (smaller broadcast domains), easier management, and cost efficiency.
- **SVIs provide Layer 3 routing between different VLANs**, allowing inter-VLAN communication without separate routers; VLAN configs are stored in the VLAN database (e.g., `vlan.dat` on Cisco).

---

### Virtual Local Area Network || VLAN

- Logical subdivisions of a whole network that segments/divides it into separate broadcast domains
- Unlike traditional LANs, VLANs allow us to group hosts together regardless of their physical connection to the same network switch
- VLANs are achieved through software configuration rather than hardware and its physical cabling
- Benefits to VLANS include:
    - Flexibility when configuring a network
    - Efficient resource allocation and management when used correctly

---

### Traditional LAN vs VLAN

- Before VLAN, network segmentation needed additional routers, cables and switches
- VLAN’s significantly reduce hardware requirements by allowing different logical networks to share the same physical hardware like a switch and even cabling by methods like VLAN trunking

---

### How VLANs Work

- Operates at layer 2 Data Link Layer of the OSI model
- When a switch is configured to utilize a VLAN its going to tag each data frame with a VLAN Identifier(ID) as it passes through that switch essential defining what VLAN a frame will belong to
- These tags will be used to determine/set the path the frames will take essentially ensuring they stay within their respective VLAN

---

### Reasons for using VLANs

1. Enhanced Security
    - When the network is segmented into VLANs it allows sensitive data to be isolated which reduces the potential for data breaches
2. Improved Performance
    - Reduces the broadcast domain size which decreases unnecessary traffic and in turn helps the performance of the overall network
3. Increased Management
    - Greater control over management of networks, easier policy implementation and troubleshooting due to each VLAN being a separate network segment
4. Improved Cost Efficiency
    - Uses existing infrastructure more effectively reducing the need for extra hardware for network segmentation.

---

### VLAN Database

- For a VLAN to be effective network switches and other associated network devices need to maintain a **VLAN DATABASE** that contains all the vlan config for a particular switch
    - Database will include information:
        - VLANIdentifier
        - VLAN Name
        - VLAN Max transmission unit size (MTU Size)
    - If using a cisco switch
        - stored in a flat file called VLAN.DAT

---

### Switch Virtual Interface (SVI)

- A virtual interface on a switch that provides layer 3 processing for our different VLANs
- Allows routing between different VLANs without the need for a separate router/device
- Essentially helps network efficiency by minimizing the need for additional routing devices