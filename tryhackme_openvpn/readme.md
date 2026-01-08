# OpenVPN – TryHackMe Lab

## 📌 Lab Overview
This lab focuses on understanding how OpenVPN enables secure access to private lab networks used in cybersecurity training environments like TryHackMe.

---

## 🎯 Objective
- Understand the role of VPN in cybersecurity labs
- Verify secure connection to an internal network

---

## 🖥️ Environment
- Operating System: Windows
- VPN Client: OpenVPN
- Platform: TryHackMe

---

## 🔧 Tasks Performed

### 1️⃣ VPN Connection Established
- Downloaded OpenVPN configuration file
- Connected successfully to TryHackMe VPN

📷 Screenshot:  
`screenshots/vpn-connected.png`

---

### 2️⃣ Network Adapter Verification
- Verified creation of virtual VPN adapter
- Observed private IP assignment (10.x.x.x)

📷 Screenshot:  
`screenshots/ipconfig.png`

---

### 3️⃣ Internal Network Access Test
- Successfully pinged internal lab machine
- Verified access only works when VPN is active

📷 Screenshot:  
`screenshots/ping-test.png`

---

## 🧠 Key Learnings
- VPN creates a secure encrypted tunnel
- A virtual network adapter is added to the system
- VPN is mandatory to access private lab networks
- Internal IP ranges (10.x.x.x) are not reachable without VPN

---

## 🛠 Commands Used
```text
ipconfig
route print
ping <internal-ip>
