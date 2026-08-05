# 📡 DHCP Configuration

> This document describes the deployment and configuration of the Dynamic Host Configuration Protocol (DHCP) service for the NOVATECH Enterprise Infrastructure project.

---

# 🎯 Objective

Deploy and configure a centralized DHCP service to automatically assign IP addresses and essential network configuration to Windows clients within the NOVATECH enterprise environment.

---

# 🏢 Enterprise Scenario

As NOVATECH expanded its infrastructure, manually configuring IP addresses for every workstation became inefficient and difficult to manage.

To improve scalability and simplify network administration, a DHCP server was deployed to automatically provide:

- 🌐 IP addresses
- 🖥️ DNS Server information
- 🏢 DNS Domain Name
- 🔄 Centralized address management

This ensures that newly deployed domain-joined computers receive the correct network configuration without manual intervention.

---

# 🏗️ Design Overview

The DHCP Server role was installed on the primary Domain Controller (**DC01**) and configured with an IPv4 scope to distribute IP addresses to client devices within the enterprise network.

The deployment includes:

- 📡 DHCP Server role
- 🌐 IPv4 Scope
- 🖥️ Address Leases
- ⚙️ Scope Options
- 🔄 Automatic IP address assignment

---

# 🛠️ Implementation

The following tasks were completed:

- Installed the DHCP Server role
- Authorized the DHCP server in Active Directory
- Created an IPv4 scope
- Configured the DHCP address pool
- Activated the DHCP scope
- Configured Scope Options
- Verified successful client lease assignment

---

# ⚙️ Configuration

| Setting | Value |
|---------|-------|
| DHCP Server | DC01 |
| Scope Name | NOVATECH-LAB-SCOPE |
| Network | 10.10.10.0/24 |
| Address Assignment | Dynamic |
| DNS Server | 10.10.10.10 |
| DNS Domain | novatech.local |

> **Note:** The DHCP scope was configured to distribute DNS server information and the Active Directory domain name. A default gateway option was not configured because routing outside the lab network was not required for this implementation.

---

# 📸 Screenshots

## DHCP Manager Overview

![DHCP Manager](../../screenshots/04-DHCP/01-dhcp-manager-overview.png)

**Description**

Displays the DHCP Manager console showing the configured IPv4 scope and DHCP server components.

---

## DHCP Scope

![DHCP Scope](../../screenshots/04-DHCP/02-dhcp-scope.png)

**Description**

Shows the configured IPv4 scope used to dynamically allocate IP addresses to enterprise clients.

---

## Address Leases

![Address Leases](../../screenshots/04-DHCP/03-address-leases.png)

**Description**

Demonstrates successful IP address allocation by displaying active DHCP leases for domain clients.

---

## Scope Options

![Scope Options](../../screenshots/04-DHCP/04-scope-options.png)

**Description**

Displays the DHCP options configured to automatically distribute DNS server information and the Active Directory domain name to client devices.

---

# 🧩 Challenges & Solutions

### Challenge

Providing consistent IP addressing and network configuration to client systems without manual configuration.

### Solution

Configured an authorized DHCP server with an active IPv4 scope and Scope Options to automatically distribute IP addresses and DNS configuration to domain-joined clients.

---

# ✅ Outcome

The DHCP infrastructure was successfully deployed and integrated with Active Directory. Client systems automatically received valid IP addresses and DNS configuration, reducing manual administration while improving consistency across the enterprise network.

---

# 💡 Key Takeaways

- 📡 DHCP centralizes IP address management.
- 🌐 Automatic address assignment reduces configuration errors.
- 🖥️ Scope Options simplify client network configuration.
- 🔄 DHCP integrates seamlessly with Active Directory and DNS.
- 🚀 Centralized IP management improves scalability in enterprise environments.