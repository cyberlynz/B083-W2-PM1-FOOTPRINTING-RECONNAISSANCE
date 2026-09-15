# Lessons Learned

## Footprinting & Reconnaissance

1. **WHOIS** can expose domain registration and administrative information such as registrar, dates, name servers and abuse contacts.
2. **WhatWeb** can fingerprint technologies such as the web server, CMS and plugins.
3. **NSLookup** maps a domain name to an IP address through DNS resolution.
4. **cURL headers** can expose server banners, response information, cookies, redirects and application endpoints.
5. **Wafw00f** can identify whether a Web Application Firewall is present.
6. **DNSRecon** can enumerate DNS information including name servers, mail servers, SPF/TXT data and service records.

## Security Takeaway

The assignment demonstrates that information exposed publicly can help build a profile of an organization before later security-testing stages. Defenders can perform the same reconnaissance against their own assets to identify unnecessary information exposure.
