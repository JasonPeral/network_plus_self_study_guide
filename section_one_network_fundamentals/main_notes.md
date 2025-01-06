# Network+ Study Notes

## 4 Network Fundamentals
### What is a Network?
Encompasses a diverse range of connections extending to both wireless networks (Wi-Fi and cellular) and wired networks (Ethernet and direct fiber connections). Networks serve the essential purpose of connecting a multitude of devices while also providing a seamless continuous flow of data.

---

## 5 Network Components (Objective 1.2)
### Clients
Devices that users access the network with, such as workstations, laptops, tablets, smartphones, smart TVs, and anything that connects to the network.

### Servers
Provide resources to the network, such as email servers, file servers, web servers, etc. These servers can exist on dedicated hardware or use specialized software to act as a server for clients.

### Hubs
- Older network devices connecting clients and servers over a LAN.
- Limitations include increased network errors due to broadcasting nature.
- Developed into Bridges and then Switches.

### Switches
- "Smarter" hubs with better security and efficient bandwidth utilization.
- Connect devices and forward traffic to intended destinations, reducing unnecessary broadcasting.

### Wireless Access Points (WAPs/APs)
- Enable wireless devices to connect to wired networks using RF waves.
- Common in homes, businesses, and large networks.

### Routers
- Connect different networks and make intelligent forwarding decisions using IP addresses.
- Use routing protocols for traffic management.

### Firewalls
- Security barriers between internal networks and external environments (Internet).
- Control traffic using pre-defined security rules.

### Load Balancers
- Distribute traffic across servers to improve efficiency, capacity, and reliability.

### Proxy
- Acts as an intermediary between user devices and the internet.
- Features include web filtering, shared connections, data caching, and enhanced security.

### IDS/IPS
**Intrusion Detection System (IDS):** Detects unauthorized access or anomalies and alerts admins.
**Intrusion Prevention System (IPS):** Detects and prevents threats by blocking harmful traffic.

### Controllers
- Manage flow control in SDN environments.
- Provide flexibility and efficiency by dictating network behavior.

### Network-attached Storage (NAS)
- Dedicated file storage accessible by authorized clients on the network.

### Storage Area Network (SAN)
- High-speed network providing block-level data storage for large amounts of data.

### Media
- Physical materials used to transmit data, such as copper cables, fiber optics, or wireless signals.

### Wide Area Network (WAN) Links
- Connect geographically distant networks using leased lines, satellite communications, or cellular networks.

---

## 6 Network Resources (Objective 1.2)
### Client/Server Model
- Utilizes a dedicated server for resources like files, scanners, and printers.
- **Pros:** Centralized admin, easy management, scalability.
- **Cons:** Higher cost, requires specialized skills.

### Peer-to-Peer Model
- Direct resource sharing among devices.
- **Pros:** Low cost, no specialized infrastructure.
- **Cons:** Decentralized management, poor scalability.

---

## 7 Network Geography (Objective 1.6)
### PAN
- Smallest network covering ~10 feet. Example: Bluetooth, USB connections.

### LAN
- Limited to ~100 meters; connects home, office, or school networks.

### CAN
- Spans several buildings in a localized area, e.g., a university campus.

### MAN
- Covers a city or ~50km. Example: city department networks.

### WAN
- Connects global networks using leased lines or VPNs.

---

## 9 Wired Network Topology (Objective 1.6)
### Physical Topology
- Represents physical cabling and layout.

### Logical Topology
- Represents data flow and logical connections.

### Types
1. **Point-to-Point:** Direct connection between two devices.
2. **Ring:** Circular data path; prone to single points of failure.
3. **Bus:** Central cable shared by devices; prone to bottlenecks.
4. **Star:** Devices connect to a central switch; reliable but central dependency.
5. **Hub-and-Spoke:** Variation of star topology; cost-effective for large networks.
6. **Mesh:** Point-to-point connections between all devices for redundancy.

---

## 10 Wireless Network Topology (Objective 1.6)
### Infrastructure Mode
- Devices communicate through a centralized device (e.g., WAP).

### Ad Hoc Mode
- Decentralized, peer-to-peer wireless communication.

### Wireless Mesh
- Combines technologies like Bluetooth, Wi-Fi, cellular, and satellite for robust networks.

---

## 11 Datacenter Topology (Objective 1.6)
### Three-tiered Hierarchy
1. **Core Layer:** High-performance routers, backbone of the network.
2. **Distribution Layer:** Enforces policies, routes between subnets.
3. **Access Layer:** Connects endpoint devices and converts packets to frames.

### Collapsed Core
- Merges core and distribution layers for smaller setups.

### Spine-and-Leaf Architecture
- Enhances speed and reduces latency in datacenters.

### Traffic Flow
- **North-South:** Data entering or leaving the datacenter.
- **East-West:** Data flowing within the datacenter.
