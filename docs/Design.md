# Active Directory Design

## Overview

The NovaTech Solutions identity environment uses Microsoft Active Directory Domain Services (AD DS) to provide centralized authentication, authorization, and identity management.

The Active Directory environment consists of:

- Forest: novatech.local
- Domain: novatech.local
- Domain Controller: DC01

---

# Organizational Unit Design

The environment uses custom Organizational Units (OUs) instead of relying on default Active Directory containers.

This design separates users, computers, administrative accounts, and groups to support:

- Better organization of objects
- Future Group Policy targeting
- Delegated administration
- Scalable identity management

## OU Structure


---

# Design Decisions

## User Separation

Users are separated by department to allow future application of department-specific policies.

Example:

Finance users may later receive:

- Finance drive mappings
- Additional security restrictions
- Finance application access

## Computer Separation

Computers are separated into Workstations and Servers to allow different security policies.

## Group Separation

Security groups and distribution groups are separated because they serve different purposes.

### Security Groups

Used for:

- Permissions
- Resource access
- Application access

### Distribution Groups

Used for:

- Communication lists
- Email organization


---

# Security Group Design

## Overview

NovaTech Solutions uses role-based security groups to manage access permissions.

Users will be assigned to department-based security groups rather than receiving permissions directly.

## Security Groups Created

| Group | Purpose |
|---|---|
| GG-Executive-Users | Executive department users |
| GG-HR-Users | Human Resources users |
| GG-Finance-Users | Finance department users |
| GG-IT-Users | Information Technology users |
| GG-Sales-Users | Sales department users |
| GG-Marketing-Users | Marketing department users |

## Group Design Principles

The environment follows the principle:

Users → Groups → Permissions

This approach simplifies administration, improves security management, and allows future delegation.