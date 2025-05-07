# Transceivers

### Core Summary

 Generalized term for any device that can both transmit and receive data and is a blend of the word transmit + receive

- Media converters and transceivers are considered Layer 1 devices because all they do is take an input signal convert it to the new format and repeat it out the other side

### **Notes**

**Transceiver** 

- Device that is capable of both transmitting and receiving data
- Utilizes specific protocols for data transmission and reception

**Protocols**

- Protocols are a set of rules and standards governing data transmission and reception over a network to ensure reliability and continuity
- 2 Main protocols(~~data link layer protocols L2)~~ we rely on for transceiving
    - Ethernet
        - Family of computer networking technologies which are commonly used for LANs, MANs and WANs
        - Facilitates communication and data transfer between different devices
        - Defines the physical standards, electrical standards for the networking cabling and connectors as well as the data formats and rules for transmitting that data over the network infrastructure
        - Supports various data rates and media types
    - Fibre Channel (FC)
        - High speed network technology that connects computer data storage to servers inside a storage area network
        - Handles large data volume quickly and reliably
        - Supports optical fiber and copper-based media
        - Key features of FC protocol
            - High throughput
            - Low Latency
            - Advanced data integrity

- How can we convert data from ethernet to fiber channel or vice versa?(see below)
- Transceiver functions
    - Converts or translates data between different protocols
    - Allows communication between ethernet and fiber channel networks which facilitates data exchange between different network infrastructures
    - Converts media types in Layer 1(fiber to copper, copper to fiber, copper to wireless..etc..etc)

- Form Factors
    - SFP (small form factor pluggable) (older)
        - A compact hot pluggable optical module
        - Can be pulled in or pulled out without turning off the associated router or switch
        - Considered to be a transceiver and supports up to 4.25 Gbps
    - SFP+
        - Faster version of an SFP modules
        - Supports up to 16 Gbps
    - QSFP (quad small form factor pluggable)
        - A compact hot pluggable optical modules like the SFP and SFP+
        - Supports up to 4 Gbps
    - QSFP+
        - Faster version of QSFP
        - Supports up to 40 Gbps
    - QSFP+
        - Slightly faster version of QSFP
        - Supports up to 41.2 Gbps
    - QSFP28
        - Supports up to 100 Gbps
    - QSFP56
        - Supports up to 200 Gbps

**Exam Tips**

- You dont have to memorize the different speeds of the transceivers but just know that QSFP modules are faster than SFP Modules
- The form factors above are just different transceivers that will be installed into a router or switch or other network device that converts a light into an electrical signal where it will be a 1 or 0 so our copper based equipment like switches can understand and utilize

SFP+ modules

![image.png](attachment:2ff2d644-a218-445b-bb37-ff7c3ea66f66:image.png)

QSFP Module

![image.png](attachment:3e224498-76d2-4fe4-bfcb-d81db36a01c1:image.png)