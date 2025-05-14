# Cable Distribution System

### Core Summary / Overview

- Cable distribution system is a organized system to connect the networks backbone in the Main Distribution Frame (MDF) to the → Intermediate Distribution Frame (IDF) and then to → End Users Wall Jacks and finally → End users device
- The design of a Cable Distribution System should be hierarchical for logical and functional placement within the building

There are many different components of a Cable Distribution System

| **Component**               | **Description**                                                                                                                                           |
|-----------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------|
| Demarcation Point           | - Locations where the ISP connection ends and the network infrastructure and cabling begins.<br>- Responsibility shifts onto the organization at this point. |
| Main Distribution Frame     | - Houses the Main Point of Presence Router and backbone switch.                                                                                            |
| Intermediate Distribution Frame | - Branches from the MDF to deliver to smaller areas or groups.<br>- Contains Edge switches to provide network access to end users.                        |
| Racks                       | - Holds various networking equipment for efficient space management.                                                                                       |
| Patch Panels                | - Convenient unit that allows for flexible connecting and routing circuits for monitoring, interconnecting, and testing.                                    |
| Fiber Distribution Panels   | - Facilitate fiber connections without punchdown blocks.<br>- Can act as a converter for types of fiber connections.                                        |

---

### Demarcation Point

- Location where the Internet service provider (ISP) connection ends and network infrastructure and cabling actually begins for an organization or individual
- This marks the entrance of the Wide Area Network into the facility
- After the Demarcation point the responsibility of the network shifts onto the organization

### Main Distribution Frame (MDF)

- This is the main/primary starting point for interior cabling after the **Demarcation handoff from the ISP**
- The MDF houses the main point of presence(PoP) router and backbone switch
    - The PoP router manages traffic going in and out of the network
    - The Backbone switch manages traffic within the network and connects all network components
        - Called the backbone switch because everything on the network will connect back into it

### Intermediate Distribution Frame (IDF)

- Branches out from the MDF to serve smaller areas or groups
- The IDF contains edge switches for local connections
    - **Edge switches provide network access to end users devices and is where the devices physically connect**
- Cable Trays
    - This is a unit or assembly of units that form a rigid structural system to securely support the cables and raceways as they move across the building
        - When we are installing cables Horizontally we are usually going to do this in the cable trays either in drop ceiling or beneath raised floor
        - Vertically — Vertical cross-connect, minimizing vertical cable crossing between floors so we usually only  run trunk cables to connect our MDF to our IDF through these vertical cross connects. (trunk cables = **high-capacity main transmission lines** that carry signals from the headend or Main distribution point to distribution nodes(edge switch) closer to end users)

 

### Racks

- Holds various network equipment for efficient space management and easy access for ongoing network maintenance
- Different types of racks
    - 2 post — for lighter equipment / Patch panels / network cabling
    - 4 post — for heavier equipment servers / ups systems
    - Wall Mounted — Space saving solutions for smaller equipment where there is limited floor space
    - Rack enclosure — for high - value equipment where it is a fully enclosed rack. Offers a protected environment for high value devices

### Patch Panels

- Device or unit that has a number of jacks for the use of connecting and routing circuits for monitoring, interconnecting and testing in a **convenient and flexible manner**.
- Patch panels will have 2 sides
    - Front side — network jacks (RJ-45 network ports)
    - Back side — 110 punchdown block
- 110 block
    - A type of punchdown block that is used for both voice and data applications that rely on CAT5 or newer copper based networks
    - 110 blocks are installed using a punchdown tool
- Patch panels are preferred over direct connections for network maintenance and port protection as it is easier to replace a patch panel than a whole switch or server
- Fiber distribution panels
    - Doesn't use punchdown blocks.
    - Facilitates fiber connections by basically being like a coupler
    - Uses SC, LC, ST or MTRJ and can act as a converted for types of fiber connection

---

### Cable Distribution Process

1. Computer connected to wall jack using a straight through patch cable (copper or can be fiber)
2. Wall jack terminates cable into punch down block
3. Cable runs through walls, ceilings or raised floors, across cable trays to intermediate distribution frame
4. Cable then gets terminated into patch panels punch down block 
5. Another patch cable connects patch panel to open port on edge switch in the IDF
6. For fiber the components would just replace the components with fiber counterparts
- This process breaks up long cable run into multiple pieces for flexibility and ease of repair
- We can troubleshoot and repair easily due to multiple connections points which avoids full cable reruns for minor issues

![image.png](https://d3ugq33b6jrffx.cloudfront.net/wp-content/uploads/2019/09/Enterprise_Infrastructure_network_diagram_11092017-1.png)