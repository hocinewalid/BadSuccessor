# Exploit-BadSuccessor.ps1

## 🧠 Purpose

Demonstrates **privilege escalation** via the **BadSuccessor vulnerability** in **Windows Server 2025**, allowing a malicious Delegated Managed Service Account (**dMSA**) to inherit permissions from a high-privilege user (e.g., Domain Admin).

---

## ⚙️ Requirements

- PowerShell with the **Active Directory module**
- At least one **Windows Server 2025 Domain Controller**
- A valid **Organizational Unit (OU)** path
- **CreateChild** and **write permissions** on the OU where the dMSA will be created or modified

---

## ⚠️ Disclaimer

This script is intended **only for educational purposes** and **authorized test environments**.  
**Do not** use this script on production systems or for malicious purposes.

---

## 🚀 Usage

1. Update the following variables in the script to match your environment:
   - `DMsaName`: The name of the malicious dMSA
   - `TargetUser`: A high-privileged user (e.g., Domain Admin)
   - `TargetOU`: Distinguished Name (DN) of the target OU
   - `FQDN`: Fully Qualified Domain Name of the dMSA

2. Run the script from a domain-joined host with proper permissions.



