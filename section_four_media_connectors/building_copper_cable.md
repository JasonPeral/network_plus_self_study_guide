# Builder a copper cable

### Straight-Through Cable (Patch Cable) 568B — 568B

- Contains the exact same pinout on both ends of the cable (e.g pin 1 on one end of the cable goes straight through to pin 1 on the other end of the cable)

### Standard pin out

- 568B standard used for wiring jacks inside the building
- A lot of the time people prefer to configure 568B to 568B for straight through (patch cables)

### Data Terminal Equipment (DTE)

- Endpoint devices that connect to a piece of data communications equipment or DCE (for example a **laptop, desktop, servers and routers**)
- In short DTE is the device that generates or receives data in a network and it is usually the end device that interacts with the user

### Data Communications Equipment (DCE)

- Includes things like **switches, modems, hubs and bridges**

### Cross over cable 568A — 568B

- Type of ethernet cable where the transmit and receive wires are crossed where it allows two similar devices to communicate directly(without a switch or hub)
- 1 end will need a 568A and the other end 568B
- A switch to a switch requires a crossover cable (need to know for exam)
    - Although we say that a switch to a switch needs a crossover cable most modern switches allow us to connect DCE to DCE(switch to a switch) using a patch cable using MDIX (Medium Dependent Interface Crossover)
    - FOR THE EXAM: Assume a switch is an older device that does not support MDIX unless the exam question states otherwise
    - So during the exam if theres a problem with 2 switches being unable to communicate we can assume that the user may have used a patch or straight through cable.

### What is Medium Dependent Interface Crossover(MDIX)?

- An automated way to electronically simulate a crossover cable even if using a straight-through patch cable

---

![Diagram](attachment:baf391cb-8823-4ee1-a4cd-b073fe2e9f12:image.png)

### Patch cable use cases

- DTE to DCE || DCE to DTE
    - Computer to a switch

### Crossover cable use cases

- DTE to DTE || DCE to DCE
    - For example: connecting a computer to a laptop