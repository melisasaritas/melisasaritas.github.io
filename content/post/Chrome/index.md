---
title: Chrome – TryHackMe
description: The solution for the "Chrome" challenge.
slug: chrome
date: 2025-04-20
categories:
    - Write-Up
tags:
    - Active Directory
    - Privilege Escalation
    - Kerberos Abuse
    - Write-Up
weight: 1
---

Chrome – TryHackMe

Google Chrome stores user credentials securely using the Windows Data Protection API (DPAPI), which relies on a master key tied to the user’s Windows credentials. This write-up focuses on solving the Chrome machine, which involves extracting and decrypting Chrome-stored credentials from a collection of provided files.

The approach includes analyzing captured network traffic, decompiling a .NET executable, decrypting AES-encrypted files, cracking the DPAPI password, and ultimately retrieving saved login credentials from Chrome’s database.

Each phase is executed using tools like Wireshark, ILSpy, CyberChef, and pypykatz, offering hands-on experience with credential recovery and browser forensics.

For a detailed step-by-step walkthrough of the solution, refer to the attached PDF file:

📄 [Solution: Attactive Directory.pdf](/writeups/files/Chrome.pdf)
