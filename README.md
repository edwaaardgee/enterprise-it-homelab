# Enterprise IT Homelab

## Overview

This project demonstrates the deployment of a Windows Server 2022 Active Directory environment in VMware Workstation.

The lab includes:

- Domain Controller deployment
- Active Directory Domain Services (AD DS)
- Organizational Unit (OU) design
- User and group administration
- Security group membership
- Shared folder creation
- NTFS and Share permissions
- Windows 11 domain join
- Client access validation

---

## Technologies Used
- VMware Workstation
- Windows Server 2022
- Windows 11
- Active Directory Domain Services (AD DS)
- Organizational Units (OUs)
- Users and Groups
- DNS
- Shared Resources
- NTFS Permissions


---

## Virtual Machines

| VM | Purpose |
|----|---------|
| DC01 | Windows Server 2022 Domain Controller |
| CLIENT01 | Windows 11 Domain-Joined Workstation |

---
## Lab Architecture

```text
DC01 (192.168.10.10)
│
├── Active Directory
├── DNS
├── Users & Groups
└── File Shares

CLIENT01 (192.168.10.20)
│
├── Domain Joined
└── Share Access Testing
```

---

## Screenshots
### 1. Domain Controller Configuration
![DC01](screenshots/01_DC01_Configured.png)

### 2. Organizational Unit Structure
![OU Structure](screenshots/02_OU_Structure.png)

### 3. Users and Groups
![Users and Groups](screenshots/03_Users_and_Groups.png)

### 4. User and Group Details
![User and Group Details](screenshots/04_Users_and_Groups_Detail.png)

### 5. Group Membership
![Group Membership](screenshots/05_Group_Membership.png)

### 6. Share Permissions
![Share Permissions](screenshots/06_File_Share_Permissions.png)

### 7. Client Domain Join
![Client Domain Join](screenshots/07_Client_Joined_Domain.png)

### 8. Client Object in Active Directory
![Client In AD](screenshots/08_Client_In_Active_Directory.png)

### 9. Share Access Verification
![Share Access](screenshots/09_Share_Access_Verified.png)

### 10. Password Policy (Before)
![Password Policy Before](screenshots/10_Password_Policy_Before.png)

### 11. Password Policy Configured
![Password Policy Configured](screenshots/11_Password_Policy_Configured.png)

### 12. Password Policy Verified
![Password Policy Verified](screenshots/12_Password_Policy_Verified.png)
---

## Skills Demonstrated

- Active Directory Administration
- User and Group Management
- Organizational Unit Design
- Security Group Management
- Windows Server Administration
- DNS Configuration
- SMB File Sharing
- NTFS Permissions
- Windows Client Administration
- Troubleshooting
- Group Policy Management
- Password Policy Administration
- Active Directory Security

This project demonstrates core Windows enterprise administration skills commonly used in help desk, systems administration, infrastructure support, and IT operations roles.
