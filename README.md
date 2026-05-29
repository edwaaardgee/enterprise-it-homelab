# Enterprise IT Homelab

## Overview

This project demonstrates the deployment and administration of a Windows Server 2022 enterprise environment using Active Directory, DNS, DHCP, Group Policy, file sharing, and Windows 11 domain integration in VMware Workstation.

The lab includes:

- Domain Controller deployment
- Active Directory Domain Services (AD DS)
- Organizational Unit (OU) design
- User and group administration
- Security group membership
- Shared folder creation
- NTFS and Share permissions
- Windows 11 domain join
- Password policy configuration
- Account lockout policy
- Drive Mapping Group Policy
- DHCP scope configuration
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
- SMB File Shares
- NTFS Permissions
- Group Policy Management
- DHCP


---

## Virtual Machines

| VM | Purpose |
|----|---------|
| DC01 | Windows Server 2022 Domain Controller |
| CLIENT01 | Windows 11 Domain-Joined Workstation |

---
## Lab Architecture

```text
DC01 (Windows Server 2022)
│
├── Active Directory
├── DNS
├── DHCP
├── Group Policy
├── File Shares
└── Security Policies

CLIENT01 (Windows 11)
│
├── Domain Joined
├── Mapped Network Drive
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

### 4. Share Permissions
![Share Permissions](screenshots/06_File_Share_Permissions.png)

### 5. Client Domain Join
![Client Domain Join](screenshots/07_Client_Joined_Domain.png)

### 6. Share Access Verification
![Share Access](screenshots/09_Share_Access_Verified.png)

### 7. Password Policy Verified
![Password Policy Verified](screenshots/12_Password_Policy_Verified.png)

### 8. Locked Account Verification
![Locked Account](screenshots/14_Account_Lockedout_Verified.png)

### 9. Drive Mapping GPO
![Drive Mapping](screenshots/15_Drive_Mapping_GPO.png)

### 10. DHCP Scope Configuration
![DHCP Scope](screenshots/16_DHCP_Scope.png)

---

## Project Outcomes

- Deployed a Windows Server 2022 domain controller in VMware Workstation
- Created and managed Organizational Units, users, and security groups
- Configured password and account lockout policies through Group Policy
- Implemented shared folders with NTFS and share permissions
- Mapped network drives automatically using Group Policy Preferences
- Configured a DHCP scope for automated IP address assignment
- Successfully joined a Windows 11 workstation to the domain
- Verified authentication, authorization, and resource access across the environment

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
- Password Policy Administration
- Active Directory Security
- DHCP Administration
- Group Policy Administration
- Drive Mapping Automation
- Account Lockout Management
- Windows Security Policy Configuration

This project demonstrates core Windows enterprise administration skills commonly used in help desk, systems administration, infrastructure support, and IT operations roles.
