# Active Directory Home Lab

## Project Overview

This repository documents my hands-on Active Directory home lab, built to develop practical skills in Windows Server administration, enterprise networking, PowerShell automation, and Windows security.

The lab simulates a small enterprise environment where I can practice real-world IT administration and cybersecurity tasks.

---

## Lab Environment

* Windows Server 2022 (Domain Controller)
* Windows 11 Pro (Domain Client)
* Kali Linux (Security Testing Workstation)
* Oracle VirtualBox
* Bridged Networking

---

## Infrastructure Implemented

### Active Directory

* Installed Active Directory Domain Services (AD DS)
* Promoted Windows Server to a Domain Controller
* Created the **lab.local** domain
* Configured DNS
* Joined a Windows 11 client to the domain

### Organizational Units

* HR
* Finance
* Sales
* IT

### User & Group Management

* Created domain users
* Created security groups
* Assigned users to department groups
* Managed users with Active Directory Users and Computers
* Managed users using PowerShell

### File Server

* Created departmental shared folders
* Configured NTFS permissions
* Configured shared folder permissions
* Tested access using different domain users
* Troubleshot permission inheritance

### Group Policy

* Created and linked Group Policy Objects (GPOs)
* Applied desktop wallpaper policies
* Configured password policies
* Configured account lockout policies
* Updated policies using `gpupdate /force`

### PowerShell Administration

* Listed Active Directory users
* Exported users to CSV
* Reset user passwords
* Unlocked locked accounts

---

## Skills Demonstrated

* Windows Server Administration
* Active Directory
* DNS
* Group Policy
* NTFS Permissions
* File Sharing
* Windows Authentication
* PowerShell
* Troubleshooting
* Enterprise Networking

---

## Technologies

* Windows Server 2022
* Windows 11
* Active Directory Domain Services
* DNS
* PowerShell
* Group Policy
* NTFS
* Oracle VirtualBox
* Kali Linux
* TCP/IP Networking

---

## Screenshots

This repository includes screenshots documenting:

* Domain Controller deployment
* Domain join
* Active Directory Users and Computers
* Organizational Units
* Shared folders
* NTFS permissions
* Group Policy configuration
* Password policies
* PowerShell administration

---

## Current Progress

* ✅ Active Directory deployed
* ✅ DNS configured
* ✅ Windows 11 joined to the domain
* ✅ Organizational Units created
* ✅ Users and groups created
* ✅ Shared folders configured
* ✅ NTFS permissions implemented
* ✅ Group Policy deployed
* ✅ Password policy configured
* ✅ Account lockout policy configured
* ✅ PowerShell administration completed

## Learning Outcome

This home lab provides practical experience with enterprise Windows administration and serves as the foundation for learning Active Directory security, Windows monitoring, and SOC operations.
