# Network Infrastructure devices

The primary devices that we use today are Routers and Switches but have evolved from Bridges and Hubs

---

### Hubs

- Is a layer 1 device (Physical layer)
- Known as a multi port repeater and is used to connect multiple network devices and work stations
- Types of hubs:
    - Passive: repeats signal without amplifying the signal
    - Active: Takes the signal in and boosts the signal to overcome cable length limitations
    - Smart: Has features of an active hub with enhanced features like SNMP for remote config
- Hubs connect collision domains together which makes the collision potential bigger
- Typical symbol of a hub on a diagram
    
    ![Screenshot 2025-07-09 at 10.46.06 PM.png](attachment:b1fb55ec-7762-47ee-ae94-38ea533a176c:Screenshot_2025-07-09_at_10.46.06_PM.png)
    

---

### Bridges

- Is a layer 2 Device (Data Link Layer)
- Bridges analyze source MAC addresses to populate a MAC address tables
- From there makes forwarding decisions based on the destination MAC address requested
- Bridges essentially breaks the collision domains up and adds security and efficiency to networks. They allow devices on one network segment to communicate without affecting other segments, only forwarding data across segments when needed. This helps reduce collisions and adds a layer of traffic control between segments

---

### Switch

- Layer 2 Device
- Very modern alternative to hubs and is known as a multiport bridge
- Each port on the switch acts as a separate and single collision domain on each port
- Learns MAC addresses of devices associated with a certain port and makes forwarding decisions based on MAC tables just like a bridge
- Full duplex support allows simultaneous(RX and TX) communication without interference
- Efficiently manages traffic, reduces collisions and improves security

---

### Routers

- Is a layer 3 Device (Network Layer)
- Operates based on IP addresses
- Connects different networks together like different IP address ranges, subnets and media types/ interface types
- Separates broadcast domains which enhances the network efficiency
    - A router separates broadcast domains by only forwarding traffic between different networks when necessary — it blocks local broadcast traffic from spreading across subnets.

---

### Layer 3 Switches (Multilayer Switches)

- Combines functions of a switch and router
- Operates at layer 3 (Network Layer) like routers with each port being a broadcast domain
- Multilayer Switches are efficient for internal networks but less effective for large-scale routing operations as these multi layer switches are not as efficient as a dedicated router.

---

### Exam tips

- Switches are layer 2 devices focused on MAC addresses unless specified as a multilayer switch or layer 3 switch
- Routers are always considered layer 3 devices focused on IP addresses
- If the exam question mentions multi layer or layer 3 switch treat it as a ROUTER