# Implementation Log

## Phase 1: Domain Controller Deployment

### Server Information

Server Name:
DC01

Operating System:
Windows Server 2022 Standard Evaluation (Desktop Experience)

Virtualization Platform:
Oracle VirtualBox 7.2.6

### Virtual Machine Resources

CPU:
2 cores

Memory:
2048 MB RAM

Storage:
50 GB dynamically allocated virtual disk

### Deployment Status

Completed

### Notes

A clean Windows Server 2022 installation was deployed as the foundation for the NovaTech Solutions identity environment. The server will later be configured as the primary Active Directory Domain Controller.


---

## Phase 2: Active Directory Deployment

### Objective

Deploy the first Active Directory forest for NovaTech Solutions.

### Domain Information

Forest:
novatech.local

Domain:
novatech.local

NetBIOS Name:
NOVATECH

### Server Configuration

Computer Name:
DC01

Static IPv4 Address:
10.0.2.10

Subnet Mask:
255.255.255.0

Default Gateway:
10.0.2.2

Preferred DNS:
10.0.2.10

### Roles Installed

- Active Directory Domain Services (AD DS)
- DNS Server

### Validation

The following validation checks were completed successfully:

- `hostname` returned **DC01**
- `$env:USERDOMAIN` returned **NOVATECH**
- `Get-ADDomain` confirmed the Active Directory domain was operational.

### Result

The server was successfully promoted to the first Domain Controller for the **novatech.local** forest and is now providing centralized identity and DNS services.

---

## Phase 3: Active Directory Organizational Unit Design

### Objective

Create an enterprise OU structure for NovaTech Solutions to support identity management and future Group Policy deployment.

### Organizational Units Created

Administrative:
- _ADM

Users:
- Executive
- Human Resources
- Finance
- Information Technology
- Sales
- Marketing

Computers:
- Workstations
- Servers

Groups:
- Security Groups
- Distribution Groups

### Status

Completed successfully.