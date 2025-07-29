# Network Access Control

### Network Access Control (NAC)

- NAC is a method for increasing the security of a given network which is done by inspecting devices attempting to connect to the network and analyzing/determining if they are secure enough to be granted network access

---

### NAC Process / work flow

1. Devices will present themselves for analyzation when first attempting to connect to the network
2. Devices will then be isolated and inspected based on its NAC configurations
- Inspection Process
    - **Port Security**
        - Is securing the **physical** network ports to prevent any unauthorized access to those ports
        - This adds a extra layer of device by limiting the number of devices that can connect to a network switch or hub
        - Port security mechanism/methodology can be configured to allow only a specific MAC address to access a port or a set of specified MAC addresses
    - **MAC FILTERING**
        - This controls the access to the network based on every devices unique MAC address
        - Maintaining a list of approved MAC addresses is good for security + if consistency between devices are important
            - Allow Listing == Only approved MAC addresses get access to network
            - Block Listing == Devices on this list are not allowed to access the network
    - **802.1x AUTHENTICATION**
        - This provides a authentication framework for our network where only authenticated users can access network services
        - This works by encapsulating the extensible authentication protocol (EAP) within the network frames to allow for a more robust authentication mechanism.
        - 802.1x authentication involves 3 components
            1. Supplicant == User device that is looking to access the network
            2. Authenticator == Network device that the user device wants to connect to
            3. Authentication Server == Server on the network that will authenticate the users device via username and psw, smart card or digital certificate..etc..etc(there are more methods but these are just common examples)
                1. Most commonly we will use a Radius server as the authentication server. The authenticator acts as a gatekeeper where they will only open the virtual gate when there is successful authentication and from there the users device will be able to send normal data traffic.

---
    ### Implementation

- Implementation can include a combination of port security, MAC filtering and 802.1x auth to ensure each device meets the strict security requirements before getting access to a an organizations larger network
    - Persistent Agent: is usually installed on the company provided computers as these persistent agents can continuously monitor and enforce compliance
    - Non-persistent agents: for personally owned devices and uses captive portals where it asks the users if it can run a temporary agent while it assesses the devices compliance then removes itself once compliance scan is completed
    - For both persistent and non-persistent, when a device connects to the network its going to check the devices MAC address and whether if its on the approved or non approved list then proceed to verify the devices identity using the 802.1x protocol
- If a device fails any of the inspections they will either be denied access or placed in a quarantine zone for further remediation/inspection.

---

### Advanced NAC Features

- Time-based access control
    - Limits network access to a device to set specified hours based on the needs or organizations operational schedule
        - Have to be careful if your organization is global and has users working in different time frames as this would disrupt the access to those users
- Location-based access control
    - Uses geo location technologies to verify the physical location of a device that is requesting network access
        - This helps with security: if devices on a certain network are only expected to be working out of New York and you get a request from a device in Russia then the device can be flagged as a potential threat or blocked all together
- Role-based access control
    - A dynamic method to regulate access based on the users role within the organization
    - This method is a powerful way to enforce the principle of least privilege(*””Giving a user, system or process the minimum level of access rights or perms necessary to perform its required tasks and nothing more””*)
- Rule-based access control
    - This method operates using a set of predefined rules to strategically grant or deny access by assessing logical conditions and statements based on the specific users identity within the organization and the context behind the request
    - For Example: Allow access to financial records only to users within the finance department/group || Deny access to accounting logs to accounting group under probation.
    - This mechanism/feature can be as simple or complex as needed

---

### Benefits of NAC

- Strengthens network security with forward thinking by ensuring only authenticated devices can fully access the network which reduces the risk of unauthorized access or rogue devices getting into the network.
- NAC provides a scalable and dynamic solution for network infrastructures allowing for unique mechanisms to be tailored towards different users, devices and use cases