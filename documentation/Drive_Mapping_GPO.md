
# Drive Mapping GPO

## Objective

Configure a Group Policy Object (GPO) to automatically map a network drive for users in the IT Organizational Unit (OU).

## Environment

* Domain: gallegos.local
* Domain Controller: DC01
* Shared Folder: IT_Share
* Target OU: IT
* Drive Letter: I:

## Steps Performed

### 1. Open Group Policy Management

1. Log in to DC01.
2. Open **Group Policy Management**.
3. Navigate to:

   Forest → Domains → gallegos.local → IT

### 2. Create a New GPO

1. Right-click the **IT** OU.
2. Select **Create a GPO in this domain, and Link it here**.
3. Name the policy:

   IT Drive Mapping

### 3. Configure Drive Mapping

1. Edit the GPO.

2. Navigate to:

   User Configuration → Preferences → Windows Settings → Drive Maps

3. Right-click and select:

   New → Mapped Drive

4. Configure the following settings:

| Setting      | Value          |
| ------------ | -------------- |
| Action       | Create         |
| Location     | \DC01\IT_Share |
| Label        | IT Share       |
| Drive Letter | I:             |

5. Click **OK**.

### 4. Apply the Policy

1. Log on to CLIENT01 using a domain user account.

2. Run:

   gpupdate /force

3. Sign out and sign back in if required.

### 5. Verify Results

1. Open **This PC** on CLIENT01.
2. Confirm that the **IT Share (I:)** drive appears automatically.
3. Verify access to the shared folder.

## Result

The Group Policy successfully mapped the network share to drive letter **I:** for users in the IT OU. Users can access shared resources without manually connecting to the network path.

## Skills Demonstrated

* Group Policy Management
* Active Directory Administration
* Windows Server Administration
* User Configuration Policies
* Drive Mapping Automation
* Enterprise File Share Management
