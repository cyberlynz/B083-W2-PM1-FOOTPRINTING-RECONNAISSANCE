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

This project documents practical **footprinting and reconnaissance** activities completed during NetworkWalks Week 02.

The assessment uses Kali Linux to gather publicly available information about **networkwalks.com** with six reconnaissance tools.

## 🎯 Objectives

- Collect domain registration information with `whois`.
- Identify web technologies with `whatweb`.
- Resolve DNS information with `nslookup`.
- Inspect HTTP headers with `curl -I`.
- Detect WAF protection with `wafw00f`.
- Enumerate DNS records with `dnsrecon`.
- Preserve terminal output and screenshot evidence for each task.

## 🧪 Target & Environment

| Item | Details |
|---|---|
| Target | `networkwalks.com` |
| Platform | Kali Linux |
| Week | 02 |
| Project | W2-PM1 |
| Batch | B083 |

## 🗂️ Repository Structure

```text
B083-W2-PM1-FOOTPRINTING-RECONNAISSANCE/
│
├── README.md
├── whois-screenshot.png
├── whatweb-screenshot.png
├── nslookup-screenshot.png
├── curl-screenshot.png
├── wafw00f-screenshot.png
├── dnsrecon-screenshot.png
│
├── task-01-whois/
│   ├── README.md
│   └── output.txt
│
├── task-02-whatweb/
│   ├── README.md
│   └── output.txt
│
├── task-03-nslookup/
│   ├── README.md
│   └── output.txt
│
├── task-04-curl/
│   ├── README.md
│   └── output.txt
│
├── task-05-wafw00f/
│   ├── README.md
│   └── output.txt
│
└── task-06-dnsrecon/
    ├── README.md
    └── output.txt
```

## 📚 Tasks & Evidence

### 01 — WHOIS

```bash
whois networkwalks.com
```

![WHOIS](whois-screenshot.png)

[Task documentation](task-01-whois/README.md) · [Command output](task-01-whois/output.txt)

---

### 02 — WhatWeb

```bash
whatweb networkwalks.com
```

![WhatWeb](whatweb-screenshot.png)

[Task documentation](task-02-whatweb/README.md) · [Command output](task-02-whatweb/output.txt)

---

### 03 — NSLookup

```bash
nslookup networkwalks.com
```

![NSLookup](nslookup-screenshot.png)

[Task documentation](task-03-nslookup/README.md) · [Command output](task-03-nslookup/output.txt)

---

### 04 — cURL

```bash
curl -I https://networkwalks.com
```

![cURL](curl-screenshot.png)

[Task documentation](task-04-curl/README.md) · [Command output](task-04-curl/output.txt)

---

### 05 — Wafw00f

```bash
wafw00f networkwalks.com
```

![Wafw00f](wafw00f-screenshot.png)

[Task documentation](task-05-wafw00f/README.md) · [Command output](task-05-wafw00f/output.txt)

---

### 06 — DNSRecon

```bash
dnsrecon -d networkwalks.com
```

![DNSRecon](dnsrecon-screenshot.png)

[Task documentation](task-06-dnsrecon/README.md) · [Command output](task-06-dnsrecon/output.txt)

## ✅ Evidence Checklist

| Task | Tool | Screenshot | Output |
|---|---|---|---|
| 01 | WHOIS | ✅ | ✅ |
| 02 | WhatWeb | ✅ | ✅ |
| 03 | NSLookup | ✅ | ✅ |
| 04 | cURL | ✅ | ✅ |
| 05 | Wafw00f | ✅ | ✅ |
| 06 | DNSRecon | ✅ | ✅ |

## 🔒 Security & Ethical Use

This project is for educational and authorised security testing only. Reconnaissance activities should be performed only against systems that are owned, provided for training, or explicitly authorised for testing.

## 👤 Author

**Collins**  
NetworkWalks Cybersecurity & Ethical Hacking — Batch B083

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
