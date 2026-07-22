# Active Directory Design

## Organizational Unit Structure

The NovaTech Solutions Active Directory environment uses a custom Organizational Unit (OU) structure instead of relying on default Active Directory containers.

The design separates users, computers, administrative accounts, and groups to support future Group Policy implementation and delegated administration.

## OU Structure



## Design Rationale

Custom OUs were created to allow future application of Group Policy Objects (GPOs), simplify administration, and provide a scalable structure for the organization.