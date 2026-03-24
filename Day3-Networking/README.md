# Day 3 - Azure Networking (VNet, Subnet, NSG)

## Objective
To understand and implement Azure networking components including Virtual Network, Subnets, and Network Security Groups (NSG).

---

## What I Did

- Created Virtual Network (VNet-AZ104)
- Configured address space: 10.0.0.0/16
- Used default subnet and created:
  - Subnet-Frontend (10.0.1.0/24)
  - Subnet-Backend (10.0.2.0/24)
- Created Network Security Group (NSG-Frontend)
- Added inbound rule to allow RDP (Port 3389)
- Associated NSG with Network Interface (NIC)
- Tested firewall behavior by allowing and denying RDP

---

## Key Learnings

### Virtual Network (VNet)
- Private network in Azure
- Enables secure communication between resources

### Subnet
- Divides VNet into smaller segments
- Helps isolate frontend and backend workloads

### Network Security Group (NSG)
- Acts as a firewall
- Controls inbound and outbound traffic using rules

---

## NSG Rule Example

| Rule Name | Port | Action | Priority |
|----------|------|--------|----------|
| Allow-RDP | 3389 | Allow | 100 |

---

## Troubleshooting Performed

### Issue 1: RDP Not Working
- Cause: NSG rule was set to Deny or incorrect priority
- Fix: Updated rule to Allow with priority 100 and restarted VM

### Issue 2: Rule Conflict
- Learned that NSG at NIC level overrides subnet NSG

---

## Testing

- Verified RDP works when rule is Allow
- Changed rule to Deny → RDP blocked
- Reverted rule → RDP restored

---

## Real-World Use Case
<img width="2544" height="1492" alt="Screenshot 2026-03-24 220210" src="https://github.com/user-attachments/assets/e0d4853b-a545-4855-a87b-5660519d9c59" />

- Frontend subnet for web servers
- Backend subnet for databases
- NSG used to restrict and control access between layers

---

## Screenshots
<img width="2544" height="1492" alt="Screenshot 2026-03-24 220210" src="https://github.com/user-attachments/assets/93f698a3-84c3-4f2f-993e-5947de0cbca5" />
<img width="2548" h<img width="2547" height="1458" alt="Screenshot 2026-03-24 220750" src="https://github.com/user-attachments/assets/244ec5e0-5f91-421d-a7a2-2c29a881b4ce" />
eight="1434" alt="Screenshot 2026-03-24 220443" src="https://github.com/user-attachments/assets/d640270a-c1cd-446d-a7da-dba43157469b" />
<img width="2550" height="1446" alt="Screenshot 2026-03-24 220838" src="https://github.com/user-attachments/assets/1e8d8335-eab8-4d32-813d-9caf34cec911" />
<img width="2548" height="1501" alt<img width="2547" height="1595" alt="Screenshot 2026-03-24 221614" src="https://github.com/user-attachments/assets/8e64189f-3370-4cf3-8b0d-ef9d142085c6" />
="Screenshot 2026-03-<img width="2549" height="1460" alt="Screenshot 2026-03-24 221934" src="https://github.com/user-attachments/assets/8d803c1a-4335-43be-b8fa-617b72dc5bfa" />
24 220938" src="https://github.com/user-attachments/assets/cbec2e27-4786-4ad8-ba12-e8173083964f" />
<img width="2556" height="1491" alt="Screenshot 2026-03-24 221949" src="https://github.com/user-attachments/assets/57f6bd88-221c-4ac6-8492-7eafd05a18d1" />
<img w<img width="2556" height="1506" alt="Screenshot 2026-03-24 222342" src="https://github.com/user-attachments/assets/dba67095-dbea-44aa-8bae-38d5266454b9" />
idth="2559" height="1551" alt="Screenshot 2026-03-24 222211" src="https://github.com/user-attachments/assets/5688b238-7680-48b5-9156-e9fb286f4ab1" />
<img width="2556" height="1381<img width="2530" height="1505" alt="Screenshot 2026-03-24 223424" src="https://github.com/user-attachments/assets/38d1c4a2-1da5-4677-8a90-f51fa0b98aaf" />
" alt="Screenshot 2026-03-24 222829" src="https://github.com/user-attachments/assets/3c86293a-c3fa-4b50-af68-f7fcf34d5e58" />
