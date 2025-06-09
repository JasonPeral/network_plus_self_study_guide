# Wireless Security

## Core Summary
Understanding wireless security involves both **authentication mechanisms** (how users prove who they are) and **encryption options** (how data is protected in transit).

---

## Authentication Mechanisms / Methodologies

### 🔑 Pre-Shared Key (PSK)
- Key shared between AP and client devices
- Usually a string of characters
- **Challenges:**
  - Less accountability for individual users (key is shared)
  - Maintenance/scalability issues in large environments (one key change affects all clients)

---

### 🔑 Enterprise Authentication
- Uses individual user credentials managed by an authentication server (e.g., **RADIUS**)

---

### 🔑 802.1X Authentication System
- Uses individual user authentication and stronger security protocols
- Relies on an **authentication server** (e.g., **RADIUS**)

---

## Wireless Security and Encryption Options

### 🔐 Wired Equivalent Privacy (WEP)
- Uses a pre-shared key
- Key lengths:
  - 40-bit (initially)
  - 64-bit
  - 128-bit
- Uses **RC4** encryption (considered weak)
- **Initialization Vector (IV) Vulnerability:**
  - 24-bit IV (sent in plaintext)
  - Attackers can reverse-engineer WEP encryption keys by capturing enough IVs
