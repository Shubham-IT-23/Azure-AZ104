# Day 4 - Azure Advanced Networking (NIC, IP, Connectivity)

## Objective
To understand how Virtual Machine networking works in Azure using Network Interface (NIC), Public IP, and Private IP.

---

## What I Did

- Explored Virtual Machine networking settings
- Identified Network Interface (NIC) attached to VM
- Checked Public IP and Private IP configuration
- Verified network details using Command Prompt
- Tested internet connectivity using ping

---

## Key Concepts

### Network Interface (NIC)
- Acts as a network card for the Virtual Machine
- Connects VM to Virtual Network (VNet)
- Handles IP addressing and communication

---

### Public IP Address
- Used to access VM from the internet
- Required for RDP connection

---

### Private IP Address
- Used for internal communication within VNet
- Not accessible from the internet

---

## Commands Used

```bash
ipconfig
ping google.com

## Screenshots

### NIC Overview
![NIC](./image1.png)
<img width="2547" height="1425" alt="Screenshot 2026-03-24 225018" src="https://github.com/user-attachments/assets/015a4273-de1a-48e2-8b31-3913bfc289c6" />
<img width="2558" height="1443" alt="Screenshot 2026-03-24 225034" src="https://github.com/user-attachments/assets/de9b69fb-3a1e-4e33-b41a-87618975e794" />

### IP Configuration
![IP Config](./image2.png)
<img width="2520" height="1540" alt="Screenshot 2026-03-24 225922" src="https://github.com/user-attachments/assets/2534367f-d016-4e45-b35b-d702efe12447" />

### Ping Test
![Ping](./image3.png)
<img width="2535" height="1522" alt="Screenshot 2026-03-24 225959" src="https://github.com/user-attachments/assets/19ce95b1-0e81-46f4-a10d-3bd875ac0922" />

### VM Networking
![Networking](./image4.png)
<img width="2558" height="1443" alt="Screenshot 2026-03-24 225034" src="https://github.com/user-attachments/assets/0ef0b0a8-f291-48d1-8d21-499e47c4e1a1" />

