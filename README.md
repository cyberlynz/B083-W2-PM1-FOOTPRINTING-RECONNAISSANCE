<div align="center">

# 🔎 Footprinting & Reconnaissance with Kali Linux

**NetworkWalks Cybersecurity & Ethical Hacking — Batch B083**  
**Week 02 | Project Module 1 (W2-PM1)**

![Cybersecurity](https://img.shields.io/badge/Cybersecurity-Reconnaissance-blue)
![Kali Linux](https://img.shields.io/badge/Kali%20Linux-Reconnaissance-557C94)
![NetworkWalks](https://img.shields.io/badge/NetworkWalks-B083-green)

</div>

---

## 📌 Project Overview

This project documents practical **footprinting and reconnaissance** activities completed as part of the NetworkWalks Week 02 Project Module 1.

The exercise focuses on collecting publicly available information about **networkwalks.com** using six Kali Linux reconnaissance tools. The assignment describes reconnaissance as the first stage of an ethical hacking or security assessment, where information about a target is gathered before later testing activities.

The six tools required by the project are:

- `whois` — domain registration details
- `whatweb` — web technology fingerprinting
- `nslookup` — DNS-to-IP resolution
- `curl -I` — HTTP response headers
- `wafw00f` — Web Application Firewall detection
- `dnsrecon` — DNS record enumeration

> **Important:** This repository is a record of an educational lab. Testing should only be performed against systems where permission has been granted or within an authorised training environment.

## 🎯 Objectives

- Query the public domain registration record using `whois`.
- Fingerprint the website using `whatweb`.
- Resolve the domain to its IP address using `nslookup`.
- Inspect HTTP response headers using `curl -I`.
- Detect a Web Application Firewall using `wafw00f`.
- Enumerate DNS records using `dnsrecon`.
- Save the command output for each task.
- Capture and document a screenshot for each task.

## 🧪 Target

| Item | Details |
|---|---|
| Target domain | `networkwalks.com` |
| Platform | Kali Linux |
| Exercise | Footprinting & Reconnaissance Attacks with Multiple Kali Tools |
| Week | 02 |
| Project Module | 01 |
| Batch | B083 |

## 🗂️ Project Structure

```text
B083-W2-PM1-FOOTPRINTING-RECONNAISSANCE/
│
├── README.md
├── task-01-whois/
│   ├── README.md
│   ├── command.txt
│   ├── output.txt
│   └── screenshot/
│       └── README.md
│
├── task-02-whatweb/
│   ├── README.md
│   ├── command.txt
│   ├── output.txt
│   └── screenshot/
│       └── README.md
│
├── task-03-nslookup/
│   ├── README.md
│   ├── command.txt
│   ├── output.txt
│   └── screenshot/
│       └── README.md
│
├── task-04-curl/
│   ├── README.md
│   ├── command.txt
│   ├── output.txt
│   └── screenshot/
│       └── README.md
│
├── task-05-wafw00f/
│   ├── README.md
│   ├── command.txt
│   ├── output.txt
│   └── screenshot/
│       └── README.md
│
└── task-06-dnsrecon/
    ├── README.md
    ├── command.txt
    ├── output.txt
    └── screenshot/
        └── README.md
```

## 📚 Tasks

### Task 1 — WHOIS

**Requirement:** Query the public domain registration record to find who owns the domain, when it was registered, and its name servers.

**Command:**

```bash
whois networkwalks.com
```

![View Task 1](whois-screenshot.png)

**📸 Screenshot:** Add your Kali terminal screenshot to `task-01-whois/screenshot/`.

---

### Task 2 — WhatWeb

**Requirement:** Fingerprint the technologies running on the website, including the web server, CMS, plugins, frameworks and IP address.

**Command:**

```bash
whatweb networkwalks.com
```

[View Task 2](whatweb-screenshot.png)

**📸 Screenshot:** Add your Kali terminal screenshot to `task-02-whatweb/screenshot/`.

---

### Task 3 — NSLookup

**Requirement:** Resolve the domain name to its IP address using DNS.

**Command:**

```bash
nslookup networkwalks.com
```

[View Task 3](nslookup-screenshot.png)

**📸 Screenshot:** Add your Kali terminal screenshot to `task-03-nslookup/screenshot/`.

---

### Task 4 — cURL

**Requirement:** Read the HTTP response headers to see the server banner, status, cookies and redirects.

**Command:**

```bash
curl -I https://networkwalks.com
```

[View Task 4](curl-screenshot.png)

**📸 Screenshot:** Add your Kali terminal screenshot to `task-04-curl/screenshot/`.

---

### Task 5 — Wafw00f

**Requirement:** Detect whether a Web Application Firewall (WAF) is protecting the target site.

**Command:**

```bash
wafw00f networkwalks.com
```

[View Task 5](wafw00f-screenshot.png)

**📸 Screenshot:** Add your Kali terminal screenshot to `task-05-wafw00f/screenshot/`.

---

### Task 6 — DNSRecon

**Requirement:** Enumerate DNS records including name servers, mail servers, SPF, TXT and service (SRV) records.

**Command:**

```bash
dnsrecon -d networkwalks.com
```

[View Task 6](dnsrecon-screenshot.png)

**📸 Screenshot:** Add your Kali terminal screenshot to `task-06-dnsrecon/screenshot/`.

## 📸 Evidence Checklist

The NetworkWalks task instructions require a screenshot and saved output for every task.

| Task | Tool | Command saved | Output saved | Screenshot |
|---|---|---|---|---|
| 01 | WHOIS | ✅ | ⏳ Add output | ⏳ Add screenshot |
| 02 | WhatWeb | ✅ | ⏳ Add output | ⏳ Add screenshot |
| 03 | NSLookup | ✅ | ⏳ Add output | ⏳ Add screenshot |
| 04 | cURL | ✅ | ⏳ Add output | ⏳ Add screenshot |
| 05 | Wafw00f | ✅ | ⏳ Add output | ⏳ Add screenshot |
| 06 | DNSRecon | ✅ | ⏳ Add output | ⏳ Add screenshot |

## 🧠 Why Footprinting Matters

Reconnaissance helps build a profile of a target before later security testing. The assignment explains that `whois` and DNS tools can reveal domain ownership, IP addresses, hosting information and mail infrastructure, while `whatweb` and `curl` can help identify technologies and HTTP details. `wafw00f` can indicate whether a Web Application Firewall is present.

The project also emphasizes that footprinting relies on information that is publicly available and that defenders can perform the same checks against their own infrastructure to understand what an outside observer can discover.

## 📝 Evidence Submission Format

For each task:

1. Run the exact command provided in the assignment.
2. Capture a clear screenshot showing the Kali terminal and command result.
3. Save the complete terminal output in `output.txt`.
4. Place the screenshot inside that task's `screenshot/` directory.
5. Replace the screenshot placeholder documentation with the actual screenshot filename.

## 🔒 Security & Ethical Use

This project is for educational and authorised security testing purposes only. Do not use the techniques documented here against systems without permission. The NetworkWalks assignment itself states that hacking is legal only when testing a network or device you own, working in a lab environment, or operating under documented permission and an agreed scope.

## 👤 Author

**Collins**  
NetworkWalks Cybersecurity Internship — Batch B083

## 📋 Project Information

| Item | Details |
|---|---|
| Training Program | NetworkWalks Cybersecurity & Ethical Hacking |
| Batch | B083 |
| Week | 02 |
| Project | W2-PM1 |
| Project Title | Footprinting & Reconnaissance Attacks with Multiple Kali Tools |
| Target | `networkwalks.com` |
| Author | Collins |

---

> **Note:** This repository structure follows the documentation style of the Week 01 lab repository while keeping the Week 02 task requirements from the supplied NetworkWalks assignment as the source of truth.
