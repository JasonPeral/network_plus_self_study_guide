# Spanning Tree Protocol (STP) = 802.1d

### Spanning Tree Protocol

- What is STP 802.1d
    - Can also known as 802.1d
    - This is an additional feature within ethernet that allows redundant links between different switches and prevents loops within our network traffic
- Why is STP important
    - Again it enables redundant links between switches which helps us with the below
    - Prevents broadcast storms and ensures network availability which is what we want when we think about the 5 9s of availability = 99.999% up time which equates to 5 minutes of down time each and every year(is it truly possible…?)

---

### Network Without STP

- Networks without STP functionality can lead to switching loops and broadcast storms because of the nature of how switches store mac addresses into a table as frames traverse through the network
    - Broadcast storm: when multiple copies of frames are forwarded back and fourth which then consumes/floods the network

---

### STP Functionality

- Utilizes a **root bridge** and **non-root bridge**
    - Root Bridge
        - This is where a switch is elected/chosen to act as a reference point for the entire spanning tree
        - The switch being chosen to be the root is chosen based off of which one has the lowest bridge ID (BID)
            - Bridge ID (BID): is made up of a priority value and a MAC address where the lowest value is considered the root bridge.
            - If the priority value ends up being equal the root will be chosen based on the lower mac address between the 2
    - Non-Root Bridge
        - Basically every other switch that is not root

---

### STP Port Types

- Root Port
    - Every non-root bridge(switch that is not root) has a single root port which is closest to the root bridge in terms of cost
    - How cost is determined in cable types:
        - If all the cabling in terms of speed are equal then the lowest port number on the switch will be chosen
        - Faster cables == lower cost (Cat 7 low cost)
        - Slower cables == higher cost (Cat 5 high cost)
        - If we have CAT 5, 6 and 7 on a switch — the port with the cat 7 cabling will be the root port
- Designated port
    - The ports closest to the root bridge in terms of cost will be the designated port
    - All ports on a root bridge are considered as a designated port
- Non-designated port
    - Ports that block traffic to prevent loops and create a loop free topology

---

### STP Port States

(Bridge protocol data unit — BPDUs)

- Blocking phases
    - BPDUs are received but not forwarded (On a non designated port)
- Listening
    - Populates the MAC address table but does not forward the frames just yet
- Learning
    - Processes the BPDUs and this is where the switch determines its role within the spanning tree(do I need to become a Root port? do I need to become a designated port or stay as a non designated port?)
- Forwarding
    - This is where the switch will determine whether its going to move into one of those states as a designated or root port
    - Once determined it will start to forward those frames over and over and starts taking over the process of being the root port

---

### Link Cost

- To go over again the link speed is associated with the cost
    - Lower the speed the higher the cost
    - Higher the speed the lower the cost
    | Speed | Ethernet Type | STP Port Cost |
    | --- | --- | --- |
    | 10Mbps | Ethernet  | 100 |
    | 100Mbps  | Fast ethernet | 19 |
    | 1 Gbps | Gigabit ethernet | 4 |
    | 10 Gbps  | Gigabit ethernet | 2 |