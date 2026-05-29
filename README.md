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

### 13. Account Lockout Policy
![Account Lockout](screenshots/13_Account_Lockout_Policy.png)

### 14. Locked Account Verification
![Locked Account](screenshots/14_Account_Lockedout_Verified.png)

### 15. Drive Mapping GPO
![Drive Mapping](screenshots/15_Drive_Mapping_GPO.png)

### 16. DHCP Scope Configuration
![DHCP Scope](screenshots/16_DHCP_Scope.png)

### 17. DHCP Address Pool
![DHCP Pool](screenshots/17_DHCP_Address_Pool.png)
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
