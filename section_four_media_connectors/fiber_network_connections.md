# Fiber Network Connections

- Created by connecting a fiber optic cable to 2 different devices

- Note ** Each type of connector can be polished or shaped**

### Fiber connectors

- Enables a quicker connection and disconnection from the network or devices rather than splicing the fiber directly into the piece of equipment would
- You need 2 Different sets of connectors on the cable
    - 1 for transmission side
    - 1 for receive side
- Types:
    - **SC Connector (subscriber connector)**
        - Square shape design with push-pull design
        - Widely used in single-mode fibers
        - Very common in telecommunications and data networking
        - Used in FTTH(fiber to the home) deployments to connect individual houses to the main fiber network of the ISP
        - The ease of disconnection and reconnection makes it ideal for environments where modification or maintenance might be needed
        
        ![image.png](https://af69ccbb-9481-4aa7-bc67-49183d02483d:image.png)
        
    - **LC Connector (Lucent Connector)**
        - Is compact in size with a push and pull mechanism
        - Favoured in high-density applications like data centres because of its smaller form factor
        - Often shipped as a paired cable for a transmit and receive side where their connectors are bound together but can be separated based on use case.
        - Features high-precision alignment which ensures efficient data transmission and minimizes potential data loss
        
        ![image.png](https://79d5a943-636d-41bb-9bba-006ad76453fe:image.png)
        
    - **ST Connector (Straight Tip Connector)**
        - Round tip with a twist lock mechanism almost like the BNC connector that is for copper based application
        - Critically important when operating in any harsh kind of environment where movement or vibrations might occur
        - Reliable connection which is commonly used for in a multi-mode fiber optics(shorter distances)
        - Well suited for outdoor applications due to its durability
        
        ![image.png](https://39a245e0-ce9c-45d8-8e64-874a5084d1ad:image.png)
        
    - **MTRJ Connector (Mechanical Transfer-Registered Jack)**
        - Small, rectangular design which houses the transmit and receive fibers within a single connector
        - Offers high-density capability with an RJ style latch mechanism
        - Suitable for space-constrained applications like office LANs where the compact design makes it well suited for connecting workstations to servers whenever space is limited
        - Is a cost effective solution for densely populated network environments
        
        ![image.png](https://0a9ea0ef-b77d-4e3d-a6c2-55e62c814992:image.png)
        
    - **MPO Connector (Multi Fiber Push on)**
        - Designed to have multiple fibers in a single connector
        - Because this connector can house multi fibers in a single connector it is essential in high density applications such as data centers and high speed networks
        - Used in backbone cabling
        - Enables quick and efficient connections which is crucial for environments that need rapid scalability
        
        ![image.png](https://d83a6879-0a9d-454f-9fee-04b0c892430a:image.png)
        
    
    ---
    
    ### Back Reflection

- This occurs when a portion of transmitted light in a fiber cable reflects back towards the source which potentially causes degradation to the signal
- Minimizing this back reflection is crucial for maintaining signal integrity and optimizing data transmissions

### Polish Types

- PC (physical contact) Style
    - Has a slight curvature in the fiber face to lower back reflection over standard straight-cut fiber
    - Least effective reduction in back reflection compared to UPC and APC
    - Best use cases is when back reflection isnt a big concern like short distances or lower-speed data transmissions
- UPC (ultra physical contact) style
    - Has a dome-shaped end face for better core alignment. It is like an updated and better version of the older physical contact style polish
    - Offers lower back reflection than PC style polish type
    - Usually found in general broadband, data and video applications
- APC (angled physical contact) style
    - Uses an 8-degree angled polish to greatly reduce back reflection
    - Lowest amount of back reflection out of the 3 polish types
    - This is well suited for high bandwidth and long distance applications such as undersea cable networks