# File Transfer Ports and Protocols

### **Definition and Core Summary**

File transfer protocols are specialized rules and procedures used for the **transmission of files across networks**. These protocols operate on designated **ports**, acting as doorways for data transfer activities.

When managing file transfers over a network, there are several protocols, each with its own **designated port(s)**:

- **Considerations for choosing a protocol:**
  - Security requirements
  - Network environment
  - Functionality

| **Protocol** | **Purpose** | **Port(s)** |
|-------------|------------|-------------|
| **FTP** | Basic file transfer | 20 (Data), 21 (Control) |
| **SFTP** | Secure file transfer | 22 |
| **TFTP** | Simple, unsecure file transfer | 69 |
| **SMB** | Windows file sharing (LAN) | 445 |

---

## **1. FTP (File Transfer Protocol)**

- One of the **oldest** protocols for file transferring.
- **Operates over Port 20 and 21**:
  - **Port 20** → Used for the **actual data transfer**.
  - **Port 21** → Used for **sending control commands** to the server (e.g., upload/download requests).
- **How it works:**
  1. The user connects via **Port 21** for authentication and setup.
  2. Once commands are sent, the actual file transfer happens over **Port 20**.
- **Security risk:**
  - FTP **does not encrypt transmissions**; data is sent in **plain text**, making it vulnerable.
- **Why use FTP?**
  - Simple and widely used across platforms.

---

## **2. SFTP (Secure File Transfer Protocol) / SSH File Transfer Protocol**

- Addresses **FTP security concerns**.
- **Operates over Port 22** (same as SSH).
- **How it works:**
  - FTP is **tunneled through an SSH connection**, making use of SSH's built-in encryption.
  - Provides **all FTP functionalities** with added security features.
- **Why use SFTP?**
  - Ensures **confidentiality and integrity** of file transfers.

---

## **3. TFTP (Trivial File Transfer Protocol)**

- A **basic version of FTP** with limited features.
- **Operates over Port 69**.
- **Key characteristics:**
  - No **authentication** or **directory browsing**.
  - Used in **low-security environments**.
- **Common use cases:**
  - Booting diskless workstations.
  - Booting up VoIP phones (which need configuration files for startup).
- **Why use TFTP?**
  - Simple, lightweight, and fast.
  - Suitable for **non-sensitive, automated file transfers**.

---

## **4. SMB (Server Message Block)**

- A protocol used for **network file sharing**, allowing applications to:
  - **Read and write files**.
  - **Request services** from servers.
- **Operates over Port 445**.
- **Primarily used for Windows file sharing**.
- **SAMBA:**
  - A **cross-platform version of SMB** available on Linux systems.
- **Important note:**
  - SMB is used **inside Local Area Networks (LANs)**.
  - It **is not meant** for transferring files over the **public internet**.

---

### **Key Considerations for File Transfer Protocol Selection**

| **Protocol** | **Use Case** | **Security** |
|-------------|-------------|-------------|
| **FTP** | Basic file transfer | ❌ Insecure (plain text) |
| **SFTP** | Secure file transfer | ✅ Secure (SSH encryption) |
| **TFTP** | Simple, automated transfers | ❌ No authentication or encryption |
| **SMB** | Windows file sharing (LAN) | ✅ Secure within LAN |

Choosing the right file transfer protocol depends on **security needs, network type, and required functionalities**. 🚀
