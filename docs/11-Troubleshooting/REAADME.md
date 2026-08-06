# 🛠️ Troubleshooting

## 📌 Overview

During the implementation of the NOVATECH Enterprise Infrastructure project, several configuration and documentation challenges were encountered. This section documents the issues, root causes, and resolutions.

---

# Issue 1 – Missing Reverse Lookup Zone

### Problem

The Reverse Lookup Zone was not available in DNS Manager during documentation.

### Cause

The reverse lookup zone had not been created during the initial DNS deployment.

### Resolution

A new IPv4 Reverse Lookup Zone was created and verified inside DNS Manager.

### Result

Reverse DNS records could now be resolved correctly.

---

# Issue 2 – DNS Documentation

### Problem

There was uncertainty regarding which DNS views should be documented.

### Cause

DNS Manager contains multiple views including server properties, forward lookup zones, and reverse lookup zones.

### Resolution

The documentation was standardized to include:

- Forward Lookup Zone
- Reverse Lookup Zone
- DNS Server Properties

---

# Issue 3 – NTFS Permissions

### Problem

The Security tab could not be found while documenting File Services.

### Cause

The folder properties were opened from Server Manager instead of Windows Explorer.

### Resolution

The shared folder was opened directly from:

C:\Shares

The Security tab was then available.

### Result

NTFS permissions were successfully documented.

---

# Issue 4 – DHCP Documentation

### Problem

It was initially unclear which DHCP components should be included.

### Cause

DHCP contains many configuration sections.

### Resolution

Documentation focused on the most important enterprise components:

- DHCP Scope
- Address Leases
- Scope Options

---

# Issue 5 – Group Policy Navigation

### Problem

Finding the correct Group Policy Objects for drive mapping required navigating multiple Organizational Units.

### Cause

Policies were linked to different OUs.

### Resolution

The correct Drive Mapping GPOs were opened directly from the Group Policy Objects container and documented.

---

# Issue 6 – PowerShell Automation

### Problem

The automation script required exact Distinguished Names for Organizational Units.

### Cause

Active Directory commands fail when OU paths are incorrect.

### Resolution

All OU Distinguished Names were validated before executing the script.

### Result

Users were successfully created and automatically assigned to the correct OUs and Security Groups.

---

# Issue 7 – Documentation Organization

### Problem

Maintaining consistency between documentation and screenshots became increasingly important as the project grew.

### Resolution

Each project section was standardized using:

- Dedicated documentation
- Matching screenshot folders
- Embedded screenshots
- Git version control

---

# ✅ Lessons from Troubleshooting

- Verify Active Directory Distinguished Names before automation.
- Validate DNS configuration before troubleshooting clients.
- Configure both Share and NTFS permissions.
- Test Group Policy after linking it to the correct OU.
- Keep documentation synchronized with screenshots.
- Commit changes frequently using Git.