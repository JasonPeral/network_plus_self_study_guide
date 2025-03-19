# Remote access ports and protocols

### Definition and core summary

- Build, manage and access systems and networks remotely from anywhere in the world, This is crucial for interconnected environments which allows control over systems, commands and files

### Remote access protocols

- SSH (secure shell)
    - This protocol is used for secure remote login and network services over an unsecure network
    - Operates on port 22 and provides a secure channel, strong authentication and encrypted data communication
    - SSH is used by network admins for remote control/access of web and server applications
- Telnet
    - Early remote log-in protocol
    - This protocol operates on port 23
    - allows remote login to another computer on the same network
    - This protocol transfers data in plain text which makes it unsecure and susceptible to eavesdropping and on path attacks
    - This was replaced by SSH due to lack of encryption
- RDP (remote desktop protocol)
    - Proprietary protocol by microsoft for graphical user interface remote connection
    - This operates on port 3389 and allows remote access to a window system supporting different network topologies
    - Supports data encryption, smart card authentication and bandwidth reduction

---

### Considerations on this section

- we hae to choose the appropriate protocol based on security requirement and specific task
- SSH is recommended for secure cli management
- Telnet should be avoided all together due to lack of encryption
- RDP is essential for a secure GUI to windows based systems