# Web Ports and Protocols

### **Definition and Core Summary**

- When we refer to web ports and protocols, we are referring to the standardized rules and numerical gateways that govern data transmission and communication on the internet for websites and webpages specifically.

There are **two main fundamental ports** used for the web:

- **Port 80 (HTTP)**
    - Unsecure port and protocol as it sends data in plain text.
- **Port 443 (HTTPS)**
    - Secure port and protocol as it encrypts all its data—*by means of SSL or TLS*—before it is transmitted to an endpoint/server.

---

### **Two Main Web Ports**

#### **Port 80 (HTTP)**
- **Hypertext Transfer Protocol (HTTP)**
    - When we type in a website and don’t specify a port, our browser will use **Port 80** by default to request that webpage from the server. This is because it is the foundation of data communication on the World Wide Web.
    - HTTP is an **application layer protocol (L7)** that is designed to enable **plain text communication** between clients and servers.
    - HTTP works by sending a **plain text request** from a client (like a browser) to a server, which in turn **sends back a plain text response** with the requested content (e.g., HTML, images, etc.).
    
- **Security Concerns with HTTP over Port 80**
    - Data is sent **in plain text (not encrypted)**, making it vulnerable to **eavesdropping** and **on-path attacks**.
    - This lack of security is a major issue when sending **sensitive data** like login credentials, credit card information, or banking details.

#### **Port 443 (HTTPS)**
- **Hypertext Transfer Protocol Secure (HTTPS)**
    - Similar to HTTP but adds a **layer of encryption** by sending the data through a **Secure Socket Layer (SSL) tunnel** or the **newer Transport Layer Security (TLS) tunnel**.
    - These tunnels **ensure that any data** being sent from the client to the server is **encrypted**, securing it from **interception or tampering** by an attacker.

---

### **Importance of HTTPS (Port 443)**

- Essential for websites or web services that handle **sensitive information** like **banking, e-commerce, or login pages**.
- When you try to access a website using **HTTP**, and **HTTPS is available**, there is often an **automatic redirection** from the insecure **HTTP to HTTPS**, ensuring **secure data transmission**.

---

### **Key Differences Between HTTP and HTTPS**

| Feature | HTTP (Port 80) | HTTPS (Port 443) |
|---------|---------------|------------------|
| **Security** | No encryption (plain text) | Encrypted using SSL/TLS |
| **Data Integrity** | Vulnerable to interception and modification | Protected from interception and tampering |
| **Use Case** | Non-sensitive web browsing | Secure transactions and login pages |
| **SEO Ranking** | Lower ranking in search engines | Preferred by Google and other search engines |
| **Performance** | Faster but insecure | Slightly slower due to encryption overhead but secure |

HTTPS is the **modern standard for web security**, and **all major websites and browsers prioritize secure communication** using **Port 443**. 🚀
