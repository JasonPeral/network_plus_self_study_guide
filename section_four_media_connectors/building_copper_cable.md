### Straight-Through Cable (Patch Cable)

- Contains the exact same pinout on both ends of the cable (e.g pin 1 on one end of the cable goes straight through to pin 1 on the other end of the cable)

### Standard pin out

- 568B standard used for wiring jacks inside the building
- A lot of the time people prefer to configure 568B to 568B for straight through (patch cables)

### Data Terminal Equipment (DTE)

- Endpoint devices that connect to a piece of data communications equipment or DCE (for example a **laptop, desktop, servers and routers**)
- In short DTE is the device that generates or receives data in a network and it is usually the end device that interacts with the user

### Data Communications Equipment (DCE)

- Includes things like **switches, modems, hubs and bridges**

### Cross over cable

- Type of ethernet cable where the transmit and receive wires are crossed where it allows two similar devices to communicate directly(without a switch or hub
- A switch to a switch requires a crossover cable (need to know for exam)
    - Although modern switches allow us to connect DCE to DCE using a patch cable using MDIX (Medium Dependent Interface Crossover)
    - Assume a switch is an older device that does not support MDIX unless the exam question states otherwise

### Medium Dependent Interface Crossover (MDIX)

- Automated way to electronically simulate a crossover cable even if using a straight-through patch cable

### Patch cable use cases

- DTE to DCE || DCE to DTE
    - Computer to a switch

### Crossover cable

- DTE to DTE || DCE to DCE
    - For example: connecting a computer to a laptop