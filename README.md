# Active Directory Home Lab

## Overview

This project demonstrates the deployment and configuration of an Active Directory environment using Windows Server 2022 in Oracle VirtualBox.

The objective was to gain hands-on experience with core Active Directory administration tasks including domain services, organizational units, user management, security groups, DNS, and Group Policy.

---

## Technologies Used

- Windows Server 2022
- Active Directory Domain Services (AD DS)
- DNS
- Group Policy Management
- Oracle VirtualBox

---

## Project Objectives

- Install Windows Server 2022
- Deploy Active Directory Domain Services
- Promote the server to a Domain Controller
- Create an Active Directory domain
- Create Organizational Units (OUs)
- Create and manage user accounts
- Create and manage security groups
- Verify DNS functionality
- Configure a domain password policy using Group Policy

---

## Domain Information

| Setting | Value |
|----------|----------|
| Domain Name | adlab.local |
| Server Role | Domain Controller |
| Directory Service | Active Directory Domain Services |
| DNS | Integrated with AD |

---

## Organizational Unit Structure

```text
adlab.local
├── Users
├── IT
├── HR
├── Workstations
└── Servers
```

The OU structure was created to logically separate resources and simplify administration.

---

## User Accounts Created

| Name | Username |
|--------|--------|
| John Smith | jsmith |
| Sarah Jones | sjones |
| IT Admin | itadmin |

---

## Security Groups

### IT_Admins

Members:
- jsmith
- itadmin

### HR_Users

Members:
- sjones

Security groups were used to demonstrate role-based access control and centralized permission management.

---

## DNS Configuration

Active Directory-integrated DNS was automatically configured during Domain Controller promotion.

Verification included:

- Forward Lookup Zones
- Domain records
- _msdcs zone
- Name Server records

---

## Group Policy Configuration

A custom password policy was configured using Group Policy Management.

Settings:

- Minimum password length: 8
- Password complexity: Enabled
- Maximum password age: 90 days

This demonstrates centralized security policy management within Active Directory.

---

## Key Skills Demonstrated

- Active Directory Administration
- Domain Controller Deployment
- Organizational Unit Management
- User and Group Administration
- DNS Management
- Group Policy Configuration
- Windows Server 2022 Administration

---

## Lessons Learned

- Active Directory relies heavily on DNS.
- Organizational Units simplify administration and policy application.
- Security groups provide scalable access control.
- Group Policy allows centralized security management.
- Proper directory design improves maintainability and delegation.
