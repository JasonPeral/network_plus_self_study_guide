# Wireless network Types

### Core summary

- Wireless networks revolutionized connectivity by eliminating the need for physical direct cabling it offers flexibility and scalability that wired networks cannot match

The different types of wireless networks can be

1. Ad Hoc 
2. Infrastructure
3. Point to point 
4. Mesh

---

### Ad Hoc Network / Independent Basic Service set (IBSS)

- Devices connect directly to each other rather than a central access point
- Operates like a peer to peer network
- Benefits: Quick and temporary networks as it does not rely on existing network infrastructure
    - Ad Hoc does not provide internet access
- Use Case: Direct filing sharing between 2 devices that are in range of each other

---

### Infrastructure Networks

- More organized setup, devices / end users will connect to a network via wireless access point (AP) which bridges into the wired local area network(LAN)
- Configuration will go as follow:
    - Basic Service Set Identifier (BSSID)
        - Each AP will have a unique identifier which is by default set to the mac address of the wireless AP
    - Service Set Identifier (SSID)
        - Common alphanumeric name given to the network
- Larger Setup configuration will go as follow:
    - May require multiple AP devices installed and then utilize Extended Service Set (ESS)
    - Extended Service Set (ESS)
        - Creates a larger network that shares the same SSID to allow seamless connectivity with end users
        - SSID becomes the ESSID in this instance (extended server set identifier)

---

### Point to Point Networks

- Connects 2 distinct locations over longer distances using High Gain Antennas
- Static in nature because each end is a fixed locations
- This network offers dedicated bandwidth and is ideal for linking buildings of the same company or areas without feasible cabling options

---

### Mesh Networks

- Adaptable and resilient network, nodes connecting to multiple others which creates infinite paths for data
- Has self healing capabilities which ensures stability by reconfiguring broken pathways on the fly
- Mesh networks are good for large scale deployment where laying cable everywhere is not feasible or too expensive
- Two types of mesh networks
    1. Using ESS configuration in a wireless network which is operating in infrastructure mode
    2. Other mesh networks can be involving multiple different types of wireless networks all operating together to provide services to end users.
        1. Can combine wifi devices, cellular networks, micro wave links and satellite connections into a single wireless mesh network.

---

### Autonomous vs Lightweight AP

**Autonomous AP**

- Where the standalone device has all of the intelligence to handle wireless networking functions independently
- Useful in small setups where centralized controller is not necessary
    - For example home router / modem is an Autonomous AP

**Lightweight AP**

- Managed by a centralized controller and is a simpler and cheaper configuration
- Basically offloads all the processing to the centralized controller which makes it easier to manage large scale networks as any rules or policies can be applied globally.

---

### Consideration in choosing a wireless network type

- Performance, reliability and ease of use will vary on the network type you choose
- Always access specific environment needs as each network type has its own advantages and disadvantages which range from simplicity to robustness