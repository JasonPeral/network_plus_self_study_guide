# Other network service PnP

### Definition and Core Summary

The other service PNP refers to different network, services, ports and protocols that play a crucial role in the network, time synchronization and the establishment of communication sessions, as well as directory services

- These PNPs are essential for organizing and providing access to distributed information located all over the network

Breakdown

| NTP | PORT 123 | Ensures all devices in our network agree on a time to operate over which |
| --- | --- | --- |
| SIP | PORT 5060/5061 | Used in various forms of communication over IP networks to initiate, maintain and terminate. |
| LDAP | PORT 389 | Insecure: Provides directory services and the functionality of retrieval and management of relevant information across the network. |
| LDAPS | PORT 636 | SECURE: Provides directory services and the functionality of retrieval and management of relevant information across the network. |

---

### Network Time Protocol (NTP)

- This protocol is used to synchronize clocks of computers over a network
- Some would think this is not that important but on the contrary it is very import for time-dependant processes, time-stamping events, transaction logging and security protocols
- NTP operates over port 123 using UDP
- For Example:
    - If there is too much of a time discrepancy from client to server our domain controller wouldn't let the workstation log into the domain as the domain controller would see theres an issue with the time of the client and server, this would affect encryption and decryption functions as well.

---

### Session initiation protocol (SIP)

- This is widely used for initiating, maintaining and terminating real-time sessions for voice, video and messaging
    - COMMON usage includes VoIP sessions for internet phone calls
- Operates over port 5060 (traditionally) on both UDP and TCP for unencrypted signalling
- Uses port 5061 using TCP with TLS (Transport Layer Security) for encrypted signalling

---

### Lightweight directory access protocol (LDAP)

- Used for accessing and maintaining distributed directory information services over an IP network
    - For example to look up personal information in email programs from internal servers
- Ports
    - LDAP (insecure): communicates over port 389 using both TCP and UDP
    - LDAPS (Secure): Encrypted with SSL or TLS and operates over port 636 using TCP

# Finding Open Ports

NMAP

Short form for Network Mapper and its a powerful open source tool used for network discovery and security audit

- At its core NMAP has features to:
    - Scan networks to discover hosts and services
    - Detect open ports on a system
    - Identify operating systems and software versions
    - Map Network topology
    - Identify potential vulnerabilities
- Use cases
    - Pentesters use it to gether intel during reconnaissance phase
    - Sysadmins use it to monitor their networks and spot unauthorized devices
    - Cyber sec professionals use it for vulnerability scanning and compliance
- ZenMap
    - Provides a graphical user interface with NMAP functionality where you can choose the different profiles of scans for example quick scan and intense scan.

---

### Basic NMap commands
```python
# Scan a single host
nmap 192.168.1.1

# Scan a range of IPs
nmap 192.168.1.1-254

# Scan and detect OS
nmap -O 192.168.1.1

# Scan common ports with service/version detection
nmap -sV 192.168.1.1

# Run a more aggressive scan (includes OS, version, script, traceroute)
nmap -A 192.168.1.1

```