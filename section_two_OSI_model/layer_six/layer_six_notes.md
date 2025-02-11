# OSI Model - Layer 6: Presentation Layer

### What happens in the presentation layer

- Layer 6 formats the data to be exchanged and secures that data with proper encryption
  - Important words to remember for layer 6 are **DATA FORMATTING** and **DATA ENCRYPTION**

### Data Formatting

- Data is formatted by a computer to have compatibility between different devices
- There are common formats like below:
  - **American Standard Code For Information Interchange (ASCII)**
    - Text-based language
    - Ensures data is readable by receiving system
    - Provides proper data structures
    - Negotiates data transfer syntax for the application layer (7)
  - **GIFs** - Pictures that have motion
  - **JPEG** - Used for photographs
  - **PNG** - Used for internet images
- These formats allow compatibility for these files to be used between different devices and operating systems
- All these formats boil down to `1s and 0s` on our device’s hard drive or network

---

### Encryption

- Used to scramble data in transit to keep it secure from prying eyes and provide data confidentiality as it crosses our network and as it's stored
- **Transport Layer Security (TLS)**
  - Ensures secure data transfer
  - Creates an encrypted tunnel, protecting sensitive information during transmission
  - **How TLS Works (Handshake Process)**
    
    TLS establishes a secure connection using a **handshake** between the client and the server:
    
    1. **Client Hello**:
       - The client sends a request to the server, including supported TLS versions, cipher suites, and a random number.
    2. **Server Hello**:
       - The server responds with its TLS version, selected cipher suite, and its own random number.
       - The server provides its **digital certificate** (signed by a trusted Certificate Authority, CA) for authentication.
    3. **Key Exchange**:
       - The client and server exchange cryptographic keys (using RSA, Diffie-Hellman, or Elliptic Curve methods).
       - They agree on a **shared session key** to encrypt data.
    4. **Finished Message**:
       - Both client and server send a message verifying encryption is established.
       - **Secure communication begins**.

### Scripting languages in layer 6

- Controls how ASCII text is displayed on the screen. The following languages determine how ASCII text should be displayed:
  - **HTML**
  - **XML**
  - **PHP**
  - **JavaScript**

### Standard Text Formats

- Different ways of displaying text using ones and zeros:
  - **ASCII**
  - **Unicode**
  - **EBCDIC**

### Image Formats

- Ways to show graphical representations of `1s and 0s`:
  - **GIFs**
  - **JPEGs**
  - **TIFFs**
  - **SVGs**
  - **PNGs**

### Movie File Formats

- Formatted `1s and 0s` to create watchable videos:
  - **MP4**
  - **MPEG**
  - **MOV**

### Encryption Algorithms

- Scrambles data to provide confidentiality and security during transit and storage:
  - **TLS**
  - **SSL (Secure Socket Layer)**
- Focus on security
