---
title: Chrome – TryHackMe
description: The solution for the "Chrome" challenge.
slug: chrome
date: 2025-04-20
image: cover.jpg
categories:
    - Write-Up
tags:
    - Chrome
    - Privilege Escalation
    - Write-Up
weight: 1
---

Chrome – TryHackMe

Google Chrome stores user credentials securely using the Windows Data Protection API (DPAPI), which relies on a master key tied to the user’s Windows credentials. This write-up focuses on solving the Chrome machine, which involves extracting and decrypting Chrome-stored credentials from a collection of provided files.

The approach includes analyzing captured network traffic, decompiling a .NET executable, decrypting AES-encrypted files, cracking the DPAPI password, and ultimately retrieving saved login credentials from Chrome’s database.

Each phase is executed using tools like Wireshark, ILSpy, CyberChef, and pypykatz, offering hands-on experience with credential recovery and browser forensics.

For a detailed step-by-step walkthrough of the solution, refer to the attached PDF file:

📄 [Solution: Chrome.pdf](/writeups/files/Chrome_WriteUp.pdf)

> Photo by [Philipp Katzenberger](https://unsplash.com/@fantasyflip?utm_content=creditCopyText&utm_medium=referral&utm_source=unsplash) on [Unsplash](https://unsplash.com/photos/closeup-photo-of-turned-on-blue-and-white-laptop-computer-iIJrUoeRoCQ?utm_content=creditCopyText&utm_medium=referral&utm_source=unsplash)
