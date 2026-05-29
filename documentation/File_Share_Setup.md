# File Share Setup

## Overview

This lab demonstrates the creation of departmental file shares on the domain controller and the assignment of access through Active Directory security groups.

---

## Shared Directory Structure

```text
C:\Shares
├── IT
├── HR
└── Sales
```

---

## SMB Shares

| Share Name | Path |
|------------|------|
| IT_Share | C:\Shares\IT |
| HR_Share | C:\Shares\HR |
| Sales_Share | C:\Shares\Sales |

---

## Access Control

### IT Department

| Security Group | Permission |
|---------------|------------|
| IT_Admins | Full Control |

### HR Department

| Security Group | Permission |
|---------------|------------|
| HR_Users | Modify, Read & Execute |

### Sales Department

| Security Group | Permission |
|---------------|------------|
| Sales_Users | Modify, Read & Execute |

---

## Validation

The following tests were performed:

- Verified SMB shares were created successfully
- Verified NTFS permissions matched department requirements
- Verified domain users could access authorized shares
- Verified CLIENT01 could access shared resources after joining the domain

---

## Skills Demonstrated

- Active Directory Security Groups
- SMB File Sharing
- NTFS Permissions
- Access Control
- Windows Server Administration
- User Authorization
- Enterprise Resource Management

---

## Enterprise Concept

In enterprise environments, permissions are assigned to security groups rather than individual users. This approach simplifies administration, improves scalability, and follows the principle of least privilege.

This lab implements role-based access control (RBAC) using Active Directory security groups to manage departmental access to shared resources.
