# Remote access ports and protocols

### Definition and core summary

- Build, manage and access systems and networks remotely from anywhere in the world, This is crucial for interconnected environments which allows our network admins and our users to control their systems, run commands and manage files across the world.

Key function of remote access and protocols

- To build and manage systems and networks across the  network or across the world

### **Core Ports and protocols to remember for this section**

| SSH | Operates over port 22 | Is the go to for SECURE command line based management |
| --- | --- | --- |
| TELNET | Operates over port 23 | Is a legacy method that is largely replaced by SSH as TelNet does not operate in a secure manner |
| RDP | Operates over 3389 | Secure graphical access to windows based system (provides a GUI) |

---

### Remote access protocols

- SSH (secure shell)
    - This protocol is used for secure remote login and network services over an unsecure network
    - Operates on port 22 and provides a secure channel over a insecure network that requires strong authentication and encrypted data communication
    - SSH is all about creating a secure encrypted tunnel so that we can operate text-based commands wherever we are located in the world on a remote server
    - SSH is used by network admins for remote control/access of web and server applications
- Telnet
    - Early remote log-in protocol
    - This protocol operates on port 23
    - allows remote login to another computer that is part of the same network
    - This protocol transfers data in plain text which makes it unsecure and susceptible to eavesdropping and on path attacks
    - This was replaced by SSH due to lack of encryption
- RDP (remote desktop protocol)
    - Proprietary protocol by microsoft for graphical user interface for remote connection
    - This operates on port 3389 and allows remote access to a window system supporting different network topologies
    - Supports data encryption, smart card authentication and bandwidth reduction

---

### Considerations on this section

- we have to choose the appropriate protocol based on security requirement and specific task
- SSH is recommended for secure cli management
- Telnet should be avoided all together due to lack of encryption
- RDP is essential for a secure GUI to windows based systems