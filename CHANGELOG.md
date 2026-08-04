# 📜 Changelog

All notable changes to the **NOVATECH Enterprise Infrastructure** project are documented in this file.

This project follows a chronological approach, where major milestones are recorded as the infrastructure evolves.

---

# [1.0.0] - Initial Enterprise Infrastructure

## 🎉 Initial Release

The first complete version of the NOVATECH Enterprise Infrastructure project.

### 🖥️ Windows Server

- Installed Windows Server 2022
- Configured static IP addressing
- Renamed server to **DC01**

---

### 👥 Active Directory

- Installed Active Directory Domain Services
- Promoted server to Domain Controller
- Created the **novatech.local** domain

---

### 🌍 DNS

- Configured Active Directory Integrated DNS
- Verified Forward Lookup Zone
- Tested name resolution

---

### 📡 DHCP

- Installed DHCP Server
- Created DHCP Scope
- Authorized DHCP in Active Directory
- Verified client IP assignment

---

### 🏢 Organizational Units

Created enterprise Organizational Units for:

- Users
- Groups
- Computers
- Human Resources
- Finance
- Information Technology
- Marketing
- Sales
- Executive

---

### 🔐 Security

Implemented:

- Global Security Groups
- Domain Local Groups
- AGDLP permission model

---

### 📂 File Services

Configured:

- Departmental folders
- NTFS Permissions
- SMB Shares

---

### ⚙️ Group Policy

Implemented:

- Drive Mapping
- Password Policy
- Account Lockout Policy
- Interactive Logon Policy
- Windows Defender Firewall Policy

---

### 💻 PowerShell Automation

Developed automation to:

- Import users from CSV
- Automatically create Active Directory users
- Assign Organizational Units
- Add Security Group membership
- Detect duplicate accounts
- Log user creation

---

### 📚 Documentation

Completed:

- Technical documentation
- Project timeline
- Troubleshooting guide
- Lessons learned
- PowerShell explanation
- GitHub portfolio documentation

---

## 🚀 Future Development

The project will continue evolving with additional enterprise technologies, security improvements, and automation enhancements while maintaining comprehensive documentation.