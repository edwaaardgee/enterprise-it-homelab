# User Creation

## Overview

This lab demonstrates the creation and organization of Active Directory user accounts within departmental Organizational Units (OUs).

Users were assigned to security groups based on their department and role to support centralized administration and Role-Based Access Control (RBAC).

---

## IT Department

### Users Created

* Edward IT
* Manager IT

### Security Group

* IT_Admins

### Purpose

IT users were assigned administrative access to IT department resources through membership in the IT_Admins security group.

---

## HR Department

### Users Created

* Edward HR

### Security Group

* HR_Users

### Purpose

HR users were granted access to Human Resources resources through membership in the HR_Users security group.

---

## Sales Department

### Users Created

No Sales users were created during this phase of the lab.

### Security Group

* Sales_Users

### Purpose

The Sales_Users security group was created to support future user provisioning and access management.

---

## Organizational Structure

```text
gallegos.local
│
├── IT
│   ├── Edward IT
│   └── Manager IT
│
├── HR
│   └── Edward HR
│
├── Sales
│
├── Workstations
│
└── Servers
```

---

## Validation

The following tasks were successfully completed:

* Created user accounts in Active Directory Users and Computers
* Organized users into departmental Organizational Units
* Created departmental security groups
* Added users to appropriate security groups
* Verified group membership assignments
* Successfully authenticated domain users from CLIENT01

---

## Skills Demonstrated

* Active Directory User Management
* User Provisioning
* Organizational Unit Administration
* Security Group Administration
* Identity Management
* Role-Based Access Control (RBAC)
* Windows Server Administration

---

## Enterprise Concept

Enterprise environments typically organize users into Organizational Units and assign permissions through security groups rather than directly to individual accounts.

This approach improves scalability, simplifies administration, and supports centralized identity and access management.
