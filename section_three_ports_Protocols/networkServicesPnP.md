# Network Services PnP

### Definition and core summary

- Network services are fundamental protocols that ensure a smooth digital communication and network management
- The different services ensure that the network devices can discover each other, communicate efficiently and relay important system information to each other.

| DNS | PORT 53 | Resolving names to IP addresses |
| --- | --- | --- |
| DHCP | PORT 67 | PORT 68 | Used for assigning network parameters  |
| SQL Services | PORT 1433 | PORT 3306 | Databased management and data querying |
| SNMP | PORT 161 | PORT 162 | Network management |
| Syslog | PORT 514 | Used for event logging |

---

### DNS (Domain Name System)

- This service is used for translating human-friendly domain names like [udemy.com](http://udemy.com) to IP addresses that computers can use to identify each other on a network
- Operates on PORT53 and uses UDP by default for queries and responses
- Will use TCP for larger messages

### DHCP (Dynamic Host Configuration Protocol)

- **Automates** the assignments of IP addresses, subnets mass. gateways and other networking parameters to clients devices
- Listens on port 67 (UDP) for client requests
- Responds on port 68 (UDP)

### SQL Services

- Refers to protocols used by database servers for managing queries, control operations from the client applications that are requesting them.
- There isnt a standard port for all sql services as different providers will use different port numbers
- Microsoft SQL server operates over port 1433
- MYSQL server operates on port 3306
    - These ports will allow for the management of databases and the retrieval of data by authorized users and applications over these ports

### SNMP (Simple Network management Protocol)

- Used for collecting information from and configuring network devices like servers, printers, hubs, switches and routers over an IP network
- Operates over 2 ports… Port 161 SNMP Managers (UDP) for Polling and Port 162 AGENTS (UDP) for unsolicited trap messages
- Crucial for network diagnostics and performance monitoring

### Syslog(System Logging)

- This is a standard for message logging that allows devices to send event messages across IP networks to an event message collector known as a syslog server.
- This syslog server will store, process or forward the logs as needed based on what requirements you have
- Operates on PORT 514
    - Uses UDP by default
    - Can use TCP if reliability is a concern