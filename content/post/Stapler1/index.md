---
title: Stapler:1 – VulnHub
description: The solution for the "Stapler:1" challenge.
slug: Stapler:1
date: 2025-05-15
image: cover.jpg
categories:
    - Write-Up
tags:
    - FTP
    - VulnHub
    - Write-Up
weight: 1
---

Stapler:1 – VulnHub

Stapler:1 is a vulnerable machine hosted on VulnHub that simulates a real-world misconfiguration scenario through an FTP server. In this challenge, the machine allows anonymous FTP access without authentication, exposing files that provide initial footholds into the system. This misconfiguration is commonly encountered in penetration testing and can lead to serious security risks if exploited properly.

The approach begins with reconnaissance and network scanning to discover the target and its open ports. Once the FTP service is identified, the attacker leverages the anonymous login to gather information such as potential usernames from exposed files. With this data, brute-force attacks are performed using Hydra to crack credentials for both FTP and SSH services. Successful authentication provides access to user directories, where more sensitive files and credentials are discovered. Eventually, privilege escalation is achieved by using one of the compromised users with sudo access to gain root privileges.

Each phase is executed using tools like netdiscover, nmap, ftp, hydra, and ssh, offering hands-on experience in enumeration, brute-force tactics, and privilege escalation methods commonly used in cybersecurity assessments.

For a detailed step-by-step walkthrough of the solution, refer to the attached PDF file:

📄 [Solution: Stapler:1.pdf](/writeups/files/Stapler1_WriteUp.pdf)

> Photo by [Philipp Katzenberger](https://unsplash.com/@fantasyflip?utm_content=creditCopyText&utm_medium=referral&utm_source=unsplash) on [Unsplash](https://unsplash.com/photos/closeup-photo-of-turned-on-blue-and-white-laptop-computer-iIJrUoeRoCQ?utm_content=creditCopyText&utm_medium=referral&utm_source=unsplash)
