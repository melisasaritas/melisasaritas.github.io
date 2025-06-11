---
title: DC-1 – VulnHub
description: The solution for the "DC-1" challenge.
slug: DC-1
date: 2025-05-05
image: cover.jpg
categories:
    - Write-Up
tags:
    - Drupal
    - Metasploit
    - Write-Up
weight: 1
---

DC-1 – VulnHub

DC-1 is a beginner-friendly vulnerable machine hosted on VulnHub, featuring a web application running on an outdated version of Drupal, a popular content management system. The goal is to exploit the CMS and ultimately gain root access by progressing through multiple phases of attack.

The process begins with scanning the network to identify open services such as SSH, HTTP, and RPC. Once the target is mapped, exploitation is carried out using a known vulnerability—CVE-2018-7600, also known as Drupalgeddon2—through the Metasploit framework. Upon successful exploitation, a reverse shell is established and upgraded for better interactivity. The final stage involves privilege escalation by leveraging a misconfigured SUID binary to obtain root-level access.

Each phase is executed using tools like netdiscover, nmap, Metasploit, and native Linux commands, providing a realistic and hands-on experience with common offensive security techniques such as network enumeration, exploitation, and post-exploitation.

For a detailed step-by-step walkthrough of the solution, refer to the attached PDF file:

📄 [Solution: Chrome.pdf](/writeups/files/DC1_WriteUp.pdf)

> Photo by [Philipp Katzenberger](https://unsplash.com/@fantasyflip?utm_content=creditCopyText&utm_medium=referral&utm_source=unsplash) on [Unsplash](https://unsplash.com/photos/closeup-photo-of-turned-on-blue-and-white-laptop-computer-iIJrUoeRoCQ?utm_content=creditCopyText&utm_medium=referral&utm_source=unsplash)
