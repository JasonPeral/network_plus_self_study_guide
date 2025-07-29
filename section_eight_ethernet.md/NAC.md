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