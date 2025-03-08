# ICMP

### **Definition and core summary**

Internet control message protocol operates on the network layer and is used for diagnostics, error reporting and network troubleshooting. It is mainly used by network devices like routers and hosts to communicate issues about data transmission.  

- ICMP is not used for data transmission between systems like how TCP and UDP is used
- Operates at the network layer of the OSI model

---

### ICMP Messages

- These are used for indicating host or service unreachability, expired time to live and router buffer issues

| Type  | Code | Message Name |
| --- | --- | --- |
| 0 | - | Echo Reply  |
| 3 | 0-15 | Destination Unreachable |
| 5 | - | Redirect |
| 8 | - | Echo Request |
| 11 | 0-1 | Time Exceeded |
| 12 | - | Parameter Problem  |

---

### Ping Util (ping command)

- Utilizes ICMP to test host reachability on an IP network
- Measures roundtrip time (latency). Basically how long it takes for a packet to go to the destination and back

---

### ICMP Reliability and design

- ICMP lacks reliability mechanisms or methodologies like TCP
    - There is no guaranteed delivery, ordering or error correction
- ICMP is designed for speed and simplicity not for data integrity or security

---

### Security Concerns with ICMP

- ICMP can be used in attacks
    - ICMP flood attacks
        - Overwhelms a target/endpoint/user with a bunch of echo request packets leading to Denial of Service attacks (DoS)
        - DoS can be amplified to DDoS with additional nodes sending the echo request packets
    - Ping of death
        - Exploits vulnerabilities in older systems where the attacker would send a larger than standard data packet where the system would not be able to reorder or process the packet ultimately causing the system to crash

---

### Modern day devices and security measures

- Modern systems are not vulnerable to ping of death due to improved security
- Network admins may choose to block ICMP traffic for security reasons but face challenges in troubleshooting network issues when blocked
