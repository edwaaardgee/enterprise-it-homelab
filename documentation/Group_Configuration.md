# Group Configuration

## Overview

This lab demonstrates the use of Active Directory security groups to manage access to departmental resources.

Security groups were created to simplify permission management and implement Role-Based Access Control (RBAC). Rather than assigning permissions directly to individual users, permissions are assigned to groups and users are added as members of those groups.

---

## Security Groups

### IT_Admins

**Purpose**

Provides administrative access to IT department resources.

**Members**

* Edward IT
* Manager IT

**Permissions**

* Full Control on IT_Share
* Administrative access to IT resources

---

### HR_Users

**Purpose**

Provides access to Human Resources department resources.

**Members**

* Edward HR

**Permissions**

* Read
* Modify

Applied to:

* HR_Share

---

### Sales_Users

**Purpose**

Provides access to Sales department resources.

**Members**

* No users assigned during this phase of the lab

**Permissions**

* Read
* Modify

Applied to:

* Sales_Share

---

## Access Model

Role-Based Access Control (RBAC)

```text
Users
  ↓
Security Groups
  ↓
Permissions
  ↓
Resources
```

Example:

```text
Edward IT
    ↓
IT_Admins
    ↓
Full Control
    ↓
IT_Share
```

---

## Validation

The following tests were completed:

* Created Active Directory security groups
* Added users to appropriate groups
* Verified group membership in Active Directory Users and Computers
* Applied permissions through group membership
* Verified resource access after domain authentication

---

## Skills Demonstrated

* Active Directory Administration
* Security Group Management
* Role-Based Access Control (RBAC)
* User Provisioning
* Access Control
* Windows Server Administration
* Permission Management

---

## Enterprise Concept

Enterprise environments commonly use security groups to manage permissions rather than assigning permissions directly to users.

This approach improves scalability, simplifies administration, and supports the Principle of Least Privilege by granting users only the access required for their job role.
