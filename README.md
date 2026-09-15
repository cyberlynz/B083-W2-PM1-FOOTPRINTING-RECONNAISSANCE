# B083-W2-PM1-FOOTPRINTING-RECONNAISSANCE

## Week 2 | Project Module 1

**Project:** Footprinting & Reconnaissance Attacks with Multiple Kali Tools  
**Training:** NetworkWalks Cybersecurity & Ethical Hacking  
**Target:** `networkwalks.com`  
**Environment:** Kali Linux

## Overview

This project documents a footprinting and reconnaissance exercise against the public website `networkwalks.com`. The assignment uses six built-in Kali Linux tools to collect publicly available information about the target.

The exercise demonstrates how different reconnaissance tools contribute to a broader target profile without attempting exploitation.

## Tasks

| Task | Tool | Objective |
|---|---|---|
| 01 | `whois` | Find domain registration details |
| 02 | `whatweb` | Fingerprint web technologies |
| 03 | `nslookup` | Resolve the domain to its IP address |
| 04 | `curl -I` | Inspect HTTP response headers |
| 05 | `wafw00f` | Detect a Web Application Firewall |
| 06 | `dnsrecon` | Enumerate DNS records |

## Commands

```bash
whois networkwalks.com
whatweb networkwalks.com
nslookup networkwalks.com
curl -I https://networkwalks.com
wafw00f networkwalks.com
dnsrecon -d networkwalks.com
```

## Key Findings Shown in the Assignment

- **WHOIS:** The assignment notes that the domain's name servers point to **HostGator**.
- **WhatWeb:** The example identifies **Apache**, **WordPress 7.0.4**, and **WP Download Manager 3.3.58**, and exposes the server IP and an email address.
- **NSLookup:** The example resolves `networkwalks.com` to **192.232.216.135**.
- **Curl:** The example shows HTTP response headers and references the WordPress REST API endpoint `/wp-json/`.
- **Wafw00f:** The example detects **ModSecurity (SpiderLabs)** as the WAF.
- **DNSRecon:** The example identifies DNS, mail, SPF/TXT and cPanel-related service records and reports **BIND 9.16.23**.

> These findings are reproduced from the provided NetworkWalks assignment PDF. They are reference findings from the training material, not claims that the same values were independently re-scanned for this repository.

## Repository Structure

```text
B083-W2-PM1-FOOTPRINTING-RECONNAISSANCE/
├── README.md
├── task-01-whois/
│   ├── README.md
│   ├── command.txt
│   └── findings.txt
├── task-02-whatweb/
│   ├── README.md
│   ├── command.txt
│   └── findings.txt
├── task-03-nslookup/
│   ├── README.md
│   ├── command.txt
│   └── findings.txt
├── task-04-curl/
│   ├── README.md
│   ├── command.txt
│   └── findings.txt
├── task-05-wafw00f/
│   ├── README.md
│   ├── command.txt
│   └── findings.txt
└── task-06-dnsrecon/
    ├── README.md
    ├── command.txt
    └── findings.txt
```

## Why Footprinting Matters

Reconnaissance is the first phase of an ethical hacking or security assessment. Public information can reveal domain ownership details, IP addresses, hosting information, technologies, DNS records, mail infrastructure and defensive controls. The assignment emphasizes that defenders can use the same techniques against their own infrastructure to understand what an external observer can discover.

## Evidence

The assignment requires a screenshot and saved command output for every task. The repository currently contains the task structure and reference findings from the supplied PDF. Add your own terminal screenshots and captured output files after running each command in Kali Linux.

## Educational Use

This repository is for cybersecurity training and authorized lab work. Reconnaissance should only be performed against systems you are permitted to assess.

## Source

Based on the provided **NetworkWalks W2-PM1 — Week 2, Project Module 1: Footprinting & Reconnaissance Attacks with Multiple Kali Tools** assignment PDF.
