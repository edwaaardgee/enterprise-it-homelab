# Account Lockout Policy

## Overview

This lab demonstrates the configuration and testing of an Account Lockout Policy using Group Policy Management in Active Directory.

The policy was implemented to help protect domain accounts against password guessing and brute-force attacks.

## Policy Settings

| Setting                             | Value                    |
| ----------------------------------- | ------------------------ |
| Account Lockout Threshold           | 5 Invalid Logon Attempts |
| Account Lockout Duration            | 30 Minutes               |
| Reset Account Lockout Counter After | 30 Minutes               |

## Validation

The policy was applied and verified using:

```cmd
gpupdate /force
```

Testing procedure:

1. Log in to CLIENT01 using a domain account.
2. Enter an incorrect password multiple times.
3. Observe the account becoming locked after reaching the configured threshold.
4. Verify the lockout status within Active Directory Users and Computers.
5. Unlock the account from the domain controller.

## Skills Demonstrated

* Group Policy Management
* Active Directory Administration
* Account Security Management
* Windows Server Administration
* User Authentication Controls
* Security Troubleshooting

## Enterprise Concept

Account lockout policies are commonly used in enterprise environments to protect user accounts from brute-force password attacks. By locking accounts after a specified number of failed login attempts, organizations reduce the risk of unauthorized access while maintaining centralized control through Active Directory and Group Policy.
