### Wireless Security and Encryption Options

- **Wired Equivalent Privacy (WEP)**
    - Uses a pre-shared key
        - 40-bit (initially)
        - 64-bits
        - 128-bits
    - Uses the Rivest Cipher 4 (RC4) encryption mechanism == weak
    - Initialization Vector Vulnerability (IV)
        - 24-bit (1s and 0s ) sent in plain text over the network
        - Attackers can reverse engineer WEP encryption keys with enough IV captured

- **Wi-Fi Protected Access (WPA)**
    - Developed to replace WEP of the IV vulnerabilities
    - WPA uses temporal Key Integrity Protocol (TKIP) instead of IV to enhance the security
        - New type of vector and uses 48-bit vector compared to WEPs 24-bit IV
    - Uses RC4 encryption like WEP but introduces new enhanced security features:
        - Message Integrity Check (MIC)
            - Ensures packets havent been tampered with during transmission to prevent on path attacks
            - Hashes data before transmission to verify integrity of packets being sent.
        - Enterprise Mode
            - Allows for individual authentication using personal/unique username and passwords via authentication server (ex. RADIUS)
            - Stronger encryption methods
            - Better scalability
            - Centralized key and user management

- **Wi-Fi Protected Access 2 (WPA2)**
    - Replaced WPA due to its vulnerabilities
    - Has **stronger** integrity checks, encryption and authentication
    
    - **Countermode with Cipher Blockchaining Message Authentication Code Protocol (CCMP)**
        - Protocol for enhanced security
        - Combines message integrity checks with a comprehensive encryption protocol for confidentiality and integrity assurance
    - Advanced Encryption Standard (AES)
        - AES replaces the less secure RC4 encryption algorithm
        - Uses 128-bit. 192-bit and 256-bit keys with 128-bit being the most used in WPA2 networks
    - Have the ability to use Personal Mode and Enterprise mode in this Encryption option
        - Personal Mode — you will have a pre-shared key and is common in home or small office networks
        - Enterprise Mode — Used in larger environments and utilizes a centralized management server like a RADIUS

- Wi-Fi Protected Access 3 (WPA3)
    - Introduced in 2018 and improved on WPA2
    - Simultaneous Authentication of Equal (SAE)
        - Security protocol to improve the handshake process in wifi auth
        - Replaces pre shared keys with a more secure auth mechanism == Dragonfly Key Exchange
        - Ensures secure initial key exchange between client and AP, this is done by requiring active interaction with the AP for each psw attempt
        - Offers forward secrecy, ensuring past communication remain encrypted should the session key be compromised
    - WIFI Protected Setup (WPS)
        - Simplifies secure network setup using a PIN or push button
        - Vulnerable to brute force because of PIN
        - Disabling this is recommended