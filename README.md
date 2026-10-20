# -Networkwalks-Cybersecurity-Internship-Footprinting-Reconnaissance-Module-
# Networkwalks Cybersecurity Internship — Footprinting & Reconnaissance Module

**Batch:** B082 | **Mentor:** Waqas Karim (CCIE) | **Organization:** Networkwalks
**Scope:** networkwalks.com (per signed Letter of Authorization NW-LOA-B082-017)

## 📋 Overview
This module covered Phase 1 & 2 of the penetration testing lifecycle: passive and light active reconnaissance against an authorized target. I completed this writeup after catching up on the module, having paused mid-way due to overlapping school coursework and exams.

## 🛠️ Tools & Techniques Used

| Tool | Purpose |
|---|---|
| Google Hacking Database (GHDB) dorks | Found exposed webcams and open directories via search operators (`intitle`, `inurl`) |
| Maltego | Domain → email transform to map OSINT infrastructure |
| WAFW00F | Identified WAF protecting the target (ModSecurity / SpiderLabs) |
| DNSRecon | DNS enumeration (A records, SOA, SRV) |
| nslookup / whois | Basic domain resolution and registration lookups |
| curl -I | HTTP header inspection (server type, cookies, security headers) |

## 🔍 Key Findings (Authorized Scope Only)
- Target resolves to `192.232.216.135`, served by Apache
- Protected by ModSecurity (SpiderLabs) WAF
- No SRV records found; standard A record enumeration successful

## 📚 What I Learned
- How Google dorking surfaces exposed infrastructure through search engine indexing
- How OSINT tools like Maltego visually map an organization's public footprint
- The importance of WAF detection before deeper testing
- A practical DNS enumeration workflow
- Real-world VM/network troubleshooting (diagnosing a stale static IP overriding DHCP in NetworkManager)

## ⏳ Note on Timeline
This module was originally assigned mid-cycle but was completed later than scheduled — school exams and coursework (COS 202, INS 204) took priority during that period. This repo reflects the completed module.

## 📜 Authorization
All testing was conducted strictly within the scope and conditions of the signed Letter of Authorization (Ref: NW-LOA-B082-017), limited to the Client's own domain and the tester's own LAN. No exploitation, unauthorized access, or out-of-scope testing was performed.

---
*Networkwalks Cybersecurity Internship — Batch B082*