# Email Ports and Protocols

### **Definition and Core Summary**

Email ports and protocols govern the transmission of **emails across the internet**. These protocols ensure the **efficient sending, receiving, and management of messages**.

### **Main Protocols**

#### **Used for Sending Emails:**
- **SMTP / SMTPS** (Simple Mail Transfer Protocol / Secure SMTP)

#### **Used for Receiving Emails:**
- **POP3 / POP3S** (Post Office Protocol v3 / Secure POP3)
- **IMAP / IMAPS** (Internet Message Access Protocol / Secure IMAP)

### **Key Notes:**
- There are **secure variants** of each mailing protocol, identified with `-S` (e.g., SMTPS, POP3S, IMAPS).
- The **base protocols** send emails in **plain text**, making them vulnerable to interception.
- Secure variants **encrypt data** using **SSL/TLS**, protecting email communication.
- While **POP3 and IMAP** are both used for receiving emails, **IMAP is more advanced** and better for managing emails across multiple devices.

---

## **Main Email Protocols and Ports**

### **1. SMTP (Simple Mail Transfer Protocol) - Sending Emails**
- The standard protocol used for **sending** emails over the internet.
- **Operates over Port 25** (default, but insecure as data is sent in plain text).

#### **SMTPS (Secure SMTP)**
- A **secure** version of SMTP, using **SSL/TLS** for encryption.
- **Operates over Port 465 or Port 587**.
- Port **587** is commonly used today for **secure email submission**.

---

### **2. POP3 (Post Office Protocol v3) - Receiving Emails**
- Retrieves emails from a remote server **to a local client**.
- **Operates over Port 110**.
- POP3 is designed to **download and delete** messages from the mail server.
- **Insecure** as it transmits emails in **plain text**.

#### **POP3S (Secure POP3)**
- A secure variant of POP3 that encrypts data via **SSL/TLS**.
- **Operates over Port 995**.

---

### **3. IMAP (Internet Message Access Protocol) - Receiving Emails**
- Offers more **flexibility than POP3**.
- **Operates over Port 143**.
- Allows users to **manage emails directly on the email server**, synchronizing across multiple devices.
- **Insecure** as it sends emails in **plain text**.

#### **IMAPS (Secure IMAP)**
- A secure version of IMAP that encrypts emails using **SSL/TLS**.
- **Operates over Port 993**.

---

### **Comparison of Email Protocols**

| **Protocol** | **Purpose** | **Default Port** | **Secure Variant** | **Secure Port** |
|-------------|------------|----------------|----------------|--------------|
| **SMTP** | Sending Emails | 25 | SMTPS | 465 / 587 |
| **POP3** | Retrieving Emails | 110 | POP3S | 995 |
| **IMAP** | Managing Emails | 143 | IMAPS | 993 |

Using **secure email protocols (SMTPS, POP3S, IMAPS)** i