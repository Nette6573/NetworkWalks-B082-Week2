# NetworkWalks-B082-Week2

## Author

**Name:** Antoinette Thompson  
**GitHub:** [Nette6573](https://github.com/Nette6573)  
**Program:** NetworkWalks Cybersecurity Internship  
**Batch:** B082  
**Project:** Project 2 – Footprinting, Reconnaissance & Network Scanning

## Overview

This repository documents my Week 2 practical cybersecurity work for the NetworkWalks Cybersecurity Internship.

The project covers:

- **W2-PM1:** Footprinting & Reconnaissance with Multiple Kali Linux Tools
- **W2-PM2:** Footprinting & Reconnaissance with the Google Hacking Database (GHDB)
- **W2-PM5:** Network Scanning with Zenmap/Nmap
- **W2-PM-FINAL:** Detailed penetration-testing report

The exercises demonstrate a progression from reconnaissance and information gathering to search-engine-assisted discovery and authorized local-network host discovery.

## Security & Privacy Notice

This repository contains **sanitized evidence for portfolio and assessment sharing**.

Sensitive information has been intentionally removed or blurred, including:

- Public IP addresses discovered during reconnaissance
- Private local-network IP addresses
- MAC addresses
- Live third-party camera URLs
- Contact information
- Verification tokens and other potentially sensitive values

The original unredacted evidence should be retained privately and supplied only through an authorized submission channel when required by the internship.

**Important:** The PM2 camera findings are summarized without reproducing live third-party access URLs. The PM5 local-network mappings are summarized without publishing individual IP/MAC pairs.

## Project Structure

```text
NetworkWalks_B082_Week2/
│
├── PM1-Footprinting/
│   ├── README.md
│   └── screenshots/
│       ├── PM1-Task1-WHOIS-REDACTED.png
│       ├── PM1-Task2-WhatWeb-REDACTED.png
│       ├── PM1-Task3-Nslookup-REDACTED.png
│       ├── PM1-Task4-cURL-REDACTED.png
│       ├── PM1-Task5-Wafw00f-REDACTED.png
│       └── PM1-Task6-DNSRecon-REDACTED.png
│
├── PM2-GHDB/
│   ├── README.md
│   ├── results/
│   └── screenshots/
│
├── PM5-Zenmap/
│   ├── README.md
│   ├── results/
│   └── screenshots/
│       └── PM5-Zenmap-Topology-REDACTED.png
│
├── W2-PM-FINAL/
│   ├── Antoinette_Thompson_NetworkWalks_B082_Week2_Penetration_Testing_Report.pdf
│   └── Antoinette_Thompson_NetworkWalks_B082_Week2_Penetration_Testing_Report.docx
│
└── README.md
```

## PM1 – Footprinting & Reconnaissance

Six Kali Linux reconnaissance tools were used:

| Tool | Purpose | Key observation |
|---|---|---|
| WHOIS | Domain registration reconnaissance | Registrar, registration dates and nameserver information |
| WhatWeb | Web technology fingerprinting | Apache, WordPress and supporting web technologies |
| Nslookup | DNS resolution | Domain-to-IP resolution |
| cURL | HTTP response inspection | HTTP/2 response and implementation metadata |
| Wafw00f | WAF fingerprinting | ModSecurity (SpiderLabs) identified |
| DNSRecon | DNS enumeration | SOA, NS, MX, A, TXT and SRV records |

### Key PM1 lesson

Using multiple tools provides a more complete picture than relying on one source. Information from WHOIS, DNS, HTTP responses and technology fingerprinting can be correlated to understand the external attack surface.

## PM2 – GHDB Footprinting

The GHDB exercise demonstrated how search-engine indexing can reveal resources without direct exploitation.

### Task 1 – Camera Interfaces

The completed worksheet recorded **11 camera-related findings**, exceeding the required 10.

The findings included searches related to several webcam and network-camera technologies. Exact live URLs are intentionally excluded from this public repository.

**Security lesson:** Organizations should review externally indexed camera and management interfaces and ensure that any interface intended to remain private is protected by appropriate access controls.

### Task 2 – Mathematics PDF Listings

The completed worksheet recorded **11 mathematics-related PDF directory/listing findings**, exceeding the required 10.

**Security lesson:** Directory indexing can expose document collections more broadly than intended. Organizations should review directory-listing configuration and search-engine indexing of public files.

## PM5 – Zenmap Network Scanning

The authorized local-network scan identified:

- **11 live hosts**, including the assessment workstation
- Corresponding IP and MAC information in the original evidence
- A Zenmap topology visualization

Individual IP/MAC mappings are intentionally excluded from this public repository.

**Security lesson:** Asset discovery is fundamental to network security. Organizations should maintain an accurate inventory of authorized devices and investigate unknown or unmanaged hosts.

## Key Findings

1. External web technologies can be fingerprinted.
2. DNS and hosting relationships can be enumerated.
3. HTTP responses can expose implementation metadata.
4. WAF technology can be identified.
5. Search engines can expose publicly indexed camera interfaces.
6. Search engines can expose directory-indexed document repositories.
7. Multiple live devices can be identified on an authorized local network.

These observations are **not automatically confirmed vulnerabilities**. Additional authorized testing would be required to establish exploitability.

## Recommendations

- Maintain an accurate inventory of externally exposed services and internal assets.
- Review DNS records periodically.
- Keep WordPress, plugins, themes and supporting libraries patched.
- Minimize unnecessary technology/version disclosure.
- Review HTTP headers and cookie security.
- Maintain and monitor WAF protections.
- Review search-engine indexing for cameras, management interfaces and file repositories.
- Require authentication for non-public camera/management interfaces.
- Disable unnecessary directory listing.
- Perform periodic internal asset discovery.
- Use network segmentation and appropriate access controls.
- Keep unredacted evidence private and use sanitized screenshots for public documentation.

## Final Report

The detailed Week 2 penetration-testing report is available in the `W2-PM-FINAL` folder.

**[View the PDF Report](./W2-PM-FINAL/Antoinette_Thompson_NetworkWalks_B082_Week2_Penetration_Testing_Report.pdf)**

The editable Word version is also included for reference:

**[View the Word Report](./W2-PM-FINAL/Antoinette_Thompson_NetworkWalks_B082_Week2_Penetration_Testing_Report.docx)**

## Evidence

All screenshots included in this repository have been sanitized for safe sharing.

The evidence demonstrates the practical work without unnecessarily publishing sensitive addresses, identifiers, tokens or third-party access paths.

## LinkedIn Project Update

My Week 2 Project 2 update is available on LinkedIn:

**Project 2: Footprinting, Reconnaissance & Network Scanning | NetworkWalks B082**

[View the LinkedIn Project 2 Post](https://lnkd.in/p/ehRvcSnG)

## Disclaimer

This repository documents practical cybersecurity exercises completed as part of the **NetworkWalks Cybersecurity Internship – Batch B082**.

All activities documented in this repository were performed for **educational and authorized training purposes** within the scope of the internship exercises.

The information presented is intended for cybersecurity learning, assessment documentation and professional portfolio purposes. The repository does not claim unauthorized access, exploitation or compromise of any system.

Sensitive information has been sanitized before publication. Live third-party camera URLs, IP addresses, MAC addresses, credentials, tokens and other potentially sensitive information have intentionally been excluded or redacted.

Any findings documented in this repository should not be interpreted as confirmed vulnerabilities without appropriate validation and authorization.

**Original unredacted evidence should be retained privately and shared only through an authorized NetworkWalks submission channel when required.**

## Acknowledgement

Thank you to **NETWORKWALKS** and **Waqas Karim (CCIE)** for the guidance, instruction and opportunity to develop practical cybersecurity skills through the internship.
