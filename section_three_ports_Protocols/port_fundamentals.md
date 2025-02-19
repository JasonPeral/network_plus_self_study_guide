# Network Port Fundamentals

### Core Summary and Definition

- ***A PORT is a logical opening in a computer that represents a service or application that is listening and waiting for traffic.***
- Using the building example, a building address would be like your IP address, where the ports are the different doors that can be accessed within the building. Each door in the office has a different use case—some lead to a lounge, restaurant, gym, or administration office.

---

- IP addresses are used to direct data to the correct system in a network. BUT how do we know what application is listening on a particular system? This is where ports come into play.
    - **Real-world example**: If I give you my street address, that is like giving my IP address—you will be able to find my exact home within the neighborhood. But how would you be able to find my bedroom, kitchen, living room, or home office? These are like ports, as they have different use cases within the home.

### Ports in Computer Networks

- A logical opening in a computer which represents a service or application that is listening and waiting for traffic on a specific port.
- Ports are listed or range from 0 to 65,535.
    
    Now, what does this mean? 
    
- Although we only have one IP address, we can have over 65,535 different openings for our network to run different services and applications on.

### 3 Different Groups of Ports

- **Well-Known Ports**
    - Numbered from ports **0 to 1,023**.
    - This group consists of well-known services like:
        - **FTP** (PORT 20, 21)
        - **SMTP** (PORT 25)
        - **HTTP** (PORT 80)
        - **HTTPS** (PORT 443)
- **Registered Ports**
    - Numbered from **1,024 to 49,151**.
    - Both well-known ports and reserved ports are registered with an online organization: **Internet Assigned Numbers Authority (IANA)**.
        
        What does this mean?
        
        - If you were creating a game and you wanted to use PORT **33,333** for your game to communicate with other systems, you would have to request that port to be reserved for your organization's use through IANA.
- **Ephemeral Ports**
    - Short-lived, temporary ports which are opened for just a small period of time from a predefined range of ports.
    - Can also be called **dynamic ports** or **private ports**.
    - Numbered from **49,152 to 65,535**.
    - No registration is required, and anyone can use them.

### *Both well-known and registered ports are registered with IANA for specific applications and services.*

---

### Data Transfer Example

- Whenever we transfer data, we need an **IP address** and a **port**. The client will communicate with a website using these two things so that we know what system we want to go to and what service or application we want to communicate with on that system.

Example from Wireshark capture:
- In the screen shot I had a capture of my device trying to communicate with github web server. Starts with my IP address 192.168.x.x with an ephemeral port as a temporary port for the session sending a SYN packet to github web server which has an IP of 140.82.114.5 and port 443 for HTTPS. (screen shot of capture not included for privacy)

- From this capture, where I was connecting to [github.com](http://github.com), it shows my system IP and an **ephemeral port** used for this session. We want to connect to their IP address with the **HTTPS application using PORT 443**.
- Ephemeral ports are opened for specific tasks and closed after data transmission.
    
    **Communication Flow:**
    
    - **Source IP** and **source PORT** initiate communication.
    - **Data is transmitted**.
    - The **random ephemeral port** is closed when the task is completed.
