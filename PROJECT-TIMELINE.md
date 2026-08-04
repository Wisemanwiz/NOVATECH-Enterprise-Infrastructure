# 📅 Project Timeline

> This timeline documents the major implementation phases of the NOVATECH Enterprise Infrastructure project, from the initial planning stage to the final PowerShell automation.

---

# 🚀 Phase 1 – Project Planning

## 🎯 Objective

Design the overall enterprise infrastructure before deployment.

### Activities

- Defined project scope
- Planned the virtual lab environment
- Selected Windows Server 2022
- Planned IP addressing
- Designed the Organizational Unit structure
- Planned naming conventions

### Outcome

A clear implementation plan was established before any configuration began.

---

# 🖥️ Phase 2 – Windows Server Deployment

## 🎯 Objective

Prepare the server that would become the Domain Controller.

### Activities

- Installed Windows Server 2022
- Configured static IP addressing
- Renamed the server to **DC01**
- Installed the latest updates

### Outcome

The server was ready for Active Directory deployment.

---

# 👥 Phase 3 – Active Directory

## 🎯 Objective

Deploy centralized identity management.

### Activities

- Installed Active Directory Domain Services
- Promoted the server to a Domain Controller
- Created the **novatech.local** domain

### Outcome

The domain infrastructure became operational.

---

# 🌍 Phase 4 – DNS

## 🎯 Objective

Implement name resolution for the domain.

### Activities

- Verified Forward Lookup Zones
- Confirmed DNS functionality
- Tested domain name resolution

### Outcome

Active Directory services successfully relied on DNS.

---

# 📡 Phase 5 – DHCP

## 🎯 Objective

Automate IP address assignment for client devices.

### Activities

- Installed DHCP
- Created a DHCP Scope
- Authorized DHCP in Active Directory
- Verified client lease allocation

### Outcome

Client computers received network configuration automatically.

---

# 🏢 Phase 6 – Active Directory Organization

## 🎯 Objective

Create a scalable Active Directory structure.

### Activities

- Created Organizational Units
- Created Security Groups
- Implemented naming conventions
- Protected Organizational Units

### Outcome

A structured and manageable Active Directory environment was established.

---

# 🔐 Phase 7 – Enterprise Security Model

## 🎯 Objective

Implement role-based access control.

### Activities

- Created Global Security Groups
- Created Domain Local Groups
- Implemented AGDLP
- Planned departmental permissions

### Outcome

Permissions became scalable and easier to manage.

---

# 📂 Phase 8 – File Services

## 🎯 Objective

Provide secure departmental file sharing.

### Activities

- Created departmental folders
- Configured NTFS permissions
- Configured SMB Shares
- Verified user access

### Outcome

Users accessed only resources belonging to their department.

---

# ⚙️ Phase 9 – Group Policy

## 🎯 Objective

Centralize workstation management.

### Activities

- Created Group Policy Objects
- Configured Drive Mapping
- Applied Password Policies
- Configured Account Lockout
- Configured Interactive Logon settings

### Outcome

Administrative tasks became centralized and automated.

---

# 💻 Phase 10 – PowerShell Automation

## 🎯 Objective

Automate Active Directory user provisioning.

### Activities

- Created CSV-based user import
- Developed PowerShell automation
- Implemented duplicate detection
- Added logging
- Tested with sample users
- Imported over one hundred users

### Outcome

User provisioning became automated and scalable.

---

# 📚 Phase 11 – Documentation

## 🎯 Objective

Produce professional project documentation.

### Activities

- Documented every implementation phase
- Recorded troubleshooting steps
- Documented lessons learned
- Created GitHub portfolio

### Outcome

The project became fully documented and reproducible.

---

# 🎉 Project Status

| Phase | Status |
|--------|--------|
| Planning | ✅ Complete |
| Windows Server | ✅ Complete |
| Active Directory | ✅ Complete |
| DNS | ✅ Complete |
| DHCP | ✅ Complete |
| Organizational Units | ✅ Complete |
| Security Groups | ✅ Complete |
| AGDLP | ✅ Complete |
| File Services | ✅ Complete |
| Group Policy | ✅ Complete |
| PowerShell Automation | ✅ Complete |
| Documentation | ✅ In Progress |

---

> The NOVATECH Enterprise Infrastructure project continues to evolve through improved documentation, additional automation, and future enterprise enhancements.