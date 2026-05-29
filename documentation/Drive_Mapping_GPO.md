# Drive Mapping GPO

## Overview

This lab demonstrates the configuration of a Group Policy Object (GPO) to automatically map a network drive for users within the IT Organizational Unit (OU).

## Configuration Details

| Setting      | Value            |
| ------------ | ---------------- |
| GPO Name     | IT Drive Mapping |
| Target OU    | IT               |
| Action       | Create           |
| Drive Letter | I:               |
| Share Path   | \DC01\IT_Share   |
| Label        | IT Share         |

## Validation

The policy was applied and verified using:

```cmd
gpupdate /force
```

Verification steps:

1. Log in to CLIENT01 using a domain account.
2. Open **This PC**.
3. Confirm that the **IT Share (I:)** network drive is automatically mapped.
4. Verify access to the shared folder.

## Skills Demonstrated

* Group Policy Management
* Active Directory Administration
* Windows Server Administration
* Drive Mapping Automation
* Enterprise File Share Management

## Enterprise Concept

Organizations commonly use Group Policy Preferences to automatically map network drives for users. This reduces manual configuration, provides consistent access to shared resources, and simplifies administration across enterprise environments.
