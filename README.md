# Azure File Server with Secure SFTP Access (POC)

## 📌 Project Overview
This project demonstrates a **Proof of Concept (POC)** for implementing a **centralized file server in Microsoft Azure** with **strict folder-level access control**.  
Each user can securely access **only their assigned folder** using **SFTP** via tools like **WinSCP / FileZilla**.

The solution is designed using **Azure Virtual Machines**, **NTFS permissions**, and **OpenSSH**, following enterprise-grade security practices.

---

## 🎯 Objective
- Create a centralized file server in Azure
- Enforce folder-level access control
- Provide secure, encrypted remote file access
- Prevent users from accessing unauthorized folders

---

## 🏗️ Architecture Overview
**High-level flow:**

User Laptop (WinSCP / FileZilla)  
→ Secure SFTP (SSH – Port 22)  
→ Azure Windows Server VM  
→ NTFS Restricted Folders (Billing / HR)

---

## ☁️ Azure Services Used
- Azure Virtual Machine (Windows Server 2019/2022)
- Azure Network Security Group (NSG)
- Public IP Address
- Windows OpenSSH Server

---

## 📂 Folder Structure
```text
C:\CompanyData
 ├── Billing
 ├── HR
