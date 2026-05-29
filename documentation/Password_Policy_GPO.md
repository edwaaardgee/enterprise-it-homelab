# Password Policy Configuration

## Overview

This lab demonstrates the configuration of a domain-level password policy using Group Policy Management in Active Directory.

## Policy Settings

| Setting                  | Value                   |
| ------------------------ | ----------------------- |
| Enforce password history | 24 passwords remembered |
| Maximum password age     | 90 days                 |
| Minimum password age     | 1 day                   |
| Minimum password length  | 12 characters           |
| Password complexity      | Enabled                 |
| Reversible encryption    | Disabled                |

## Validation

The policy was applied and verified using:

```cmd
gpupdate /force
net accounts
```

## Skills Demonstrated

* Group Policy Management
* Active Directory Security
* Password Policy Administration
* Domain Security Controls
* Windows Server Administration

## Enterprise Concept

Password policies are used to enforce strong authentication standards across an Active Directory domain. Organizations use these controls to reduce the risk of credential compromise and improve overall security posture.
