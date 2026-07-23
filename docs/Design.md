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