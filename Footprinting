# Footprinting & Network Scanning Phases

**W2-PM-FINAL | CYBERSECURITY | NETWORKWALKS**

## Project Information

| Field | Details |
|---|---|
| **Pentester Name** | Nethmi Bhayogya |
| **Program / Batch** | B084 - Networkwalks |
| **Date** | 17 November 2026 |
| **Modules Completed** | W2-PM1 – Multiple Kali Tools<br>W2-PM5 – Zenmap Scanning |
| **Client / Target** | 1. Networkwalks (Written permission secured)<br>2. Own Local LAN Network |
| **Permission Secured** | Yes |
| **Phases Covered** | Phase 1: Reconnaissance & Footprinting<br>Phase 2: Scanning & Network Discovery<br>Phases 3–5: In Progress |

---

## 1. Liability Disclaimer

I have performed these activities only on systems and devices for which I had secured written permission or on devices and systems that I own.

All materials are intended for educational and research purposes only. Do not use any information or techniques presented here to violate the law.

The instructor, authors, and Networkwalks are not responsible for any misuse of this knowledge. Every action taken is the user's own responsibility.

Unauthorized access is a crime in many countries, even when no damage is caused. Misuse may result in criminal charges, heavy fines, loss of employment, and a permanent criminal record.

## 2. Introduction

This report documents two cybersecurity activities completed as part of Week 2 of my ongoing internship program at Networkwalks.

The activities cover two important stages of the penetration testing process:

- **Footprinting and Reconnaissance (W2-PM1):** Gathering publicly available information about the `networkwalks.com` domain using multiple Kali Linux tools.
- **Scanning and Network Discovery (W2-PM5):** Scanning my own local area network using Zenmap to identify active hosts and network information.

Together, these activities demonstrate how penetration testers move from collecting publicly available information to discovering live hosts within a network.

All footprinting commands were executed in Kali Linux, while network scanning was performed using Zenmap on a Windows PC.

Each activity includes the commands used, observed results, screenshots as evidence, and a brief explanation of the security relevance of the findings.

## 3. Tools Used

The following tools were used during the footprinting and network scanning activities.

| Tool | Purpose |
|---|---|
| Kali Linux | Operating system used for reconnaissance activities |
| Windows | Operating system used for network scanning |
| WHOIS | Retrieves publicly available domain registration information, including registration dates and name servers |
| WhatWeb | Identifies website technologies, CMS platforms, plugins, and server information |
| Nslookup | Resolves domain names into IP addresses using DNS |
| Curl (`-I`) | Retrieves HTTP response headers from a website |
| Wafw00f | Detects whether a Web Application Firewall (WAF) protects a website |
| DNSRecon | Enumerates DNS records, including NS, MX, SPF, TXT, and SRV records |
| Zenmap (Nmap GUI) | Scans a local subnet to discover active hosts, IP addresses, and MAC addresses |
| Windows CMD | Identifies local IP and MAC address information |

## 4. Activities Performed

### 4.1 Footprinting & Reconnaissance

I performed reconnaissance against the `networkwalks.com` domain using six Kali Linux tools:

1. WHOIS
2. WhatWeb
3. Nslookup
4. Curl
5. Wafw00f
6. DNSRecon

Each tool was used to gather a different category of publicly accessible information about the target domain and its web infrastructure.

#### 4.1.1 WHOIS – Domain Registration Information

WHOIS was used to retrieve publicly available domain registration information and identify the domain's name servers.

**Purpose:**
- Identify domain registration details.
- Examine domain registration dates.
- Identify registered name servers.
- Gather publicly available information about the domain.

**Security Relevance:**

This information can help penetration testers understand the domain's registration and hosting infrastructure during the reconnaissance phase.

#### 4.1.2 WhatWeb – Website Technology Fingerprinting

WhatWeb was used to identify the technologies and software components used by the target website.

**Key Findings:**
- CMS: WordPress 7.0.4
- Plugin: WP Download Manager 3.3.58
- Additional website technology information was identified.

**Security Relevance:**

Identifying the CMS, plugins, and software versions helps security professionals understand the target's technology stack and investigate potential security vulnerabilities.

#### 4.1.3 Nslookup – DNS Resolution

Nslookup was used to resolve the target domain name into its corresponding IP address.

**Command Purpose:**
- Retrieve the IP address associated with the domain.
- Examine DNS resolution information.

**Key Finding:**

| Domain | Resolved IP Address |
|---|---|
| networkwalks.com | 192.232.216.135 |

**Security Relevance:**

Identifying the IP address helps establish the network endpoint associated with a domain for authorized security assessment.

#### 4.1.4 Curl – HTTP Response Header Analysis

Curl was executed with the `-I` option to retrieve and inspect the HTTP response headers of the target website.

**Command Purpose:**
- Examine HTTP response headers.
- Identify server-related information.
- Observe information exposed by the web application.

**Key Finding:**

The response exposed the WordPress REST API endpoint:

`/wp-json/`

**Security Relevance:**

HTTP response headers and exposed API endpoints can provide useful information about the web application and its underlying technologies.

#### 4.1.5 Wafw00f – Web Application Firewall Detection

Wafw00f was used to identify whether a Web Application Firewall (WAF) was protecting the target website.

**Key Finding:**

- Detected WAF: ModSecurity (SpiderLabs)

**Security Relevance:**

Identifying a WAF helps security professionals understand the protective mechanisms implemented by a website and evaluate its security architecture.

#### 4.1.6 DNSRecon – DNS Enumeration

DNSRecon was used to enumerate DNS records associated with the target domain.

**Information Examined:**
- NS Records – Name servers
- MX Records – Mail exchange servers
- SPF Records – Sender Policy Framework information
- TXT Records – Additional DNS text information
- SRV Records – Service-related records
- DNS software information

**Security Relevance:**

DNS enumeration provides insights into domain infrastructure, mail services, and publicly exposed DNS information. These findings can help identify potential areas for further authorized security assessment.

---

## 5. Evidence and Screenshots

Screenshots of the commands executed and their corresponding results are included in the relevant activity sections to document the practical work performed.

## 6. Conclusion

Through these activities, I gained practical experience in two important stages of penetration testing: footprinting and network scanning.

Using Kali Linux tools, I explored how publicly available information about a domain can be collected and analyzed. I also used Zenmap to discover active devices and identify network information within my own local LAN.

These exercises improved my understanding of reconnaissance techniques, DNS enumeration, website technology fingerprinting, WAF detection, and network discovery.

**Status:** Phase 1 and Phase 2 completed. Phases 3–5 are in progress.
