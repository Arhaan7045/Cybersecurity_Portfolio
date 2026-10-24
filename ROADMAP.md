# Complete Cybersecurity Roadmap
Updated: 24 October 2026

## Mission
Build practical cybersecurity skills across systems, networks, Windows, security fundamentals, web/API security, authorised testing, SOC/detection, cloud, automation, risk, communication and career readiness. SOC and web security are connected perspectives, not separate learning worlds.

## Learning rules
- Start every episode with a realistic scenario (for example, fictional Falcon Technologies).
- Explain concepts in simple English and explain every new command/tool and the output.
- Aim for ~80% hands-on and 20% theory when appropriate; never skip essential foundations.
- Connect how a system can fail, how evidence reveals it, how to detect/fix it, and how to explain it.
- Require genuine proof: command output, lab evidence, mini challenge, or explanation in own words. Screenshots alone are insufficient.
- Each episode: short learning log, relevant command-reference additions, concise screenshot checklist, mini challenge, interview prompt, technical and non-technical explanation, Git commit when complete.
- One main repository: Cybersecurity_Portfolio. Preserve current files and the existing Learning-Log (singular) folder.
- Only test owned, deliberately vulnerable, or explicitly authorised systems. Never fabricate evidence.

## Phase structure and exit proofs
1. Linux and command-line foundations (EP-001–018). Exit: Bash log analyser flags failed-login bursts in supplied sample logs; limitations explained.
2. Networking and Internet fundamentals (EP-019–030). Exit: explain a packet capture and write an evidence-based investigation.
3. Windows, identity and endpoint security (EP-031–042). Exit: investigate Windows event logs and recommend next steps.
4. Security fundamentals and vulnerability management (EP-043–054). Exit: prioritised vulnerability register with remediation and verification.
5. Web and API security (EP-055–072). Exit: mini assessment report for a vulnerable lab app, with evidence, impact and fixes.
6. Ethical testing and reconnaissance (EP-073–084). Exit: scoped test plan, validated lab findings, report and retest.
7. SOC, detection and incident response (EP-085–100). Exit: three tested detection rules mapped to ATT&CK with false-positive notes.
8. Cloud and cloud identity security (EP-101–112). Exit: investigate, fix and verify a simulated cloud misconfiguration.
9. Python, automation and AI security (EP-113–124). Exit: explainable automation/triage pipeline with tests and failure-case notes.
10. Integrated projects, risk and career readiness (EP-125 onward). Exit: reproducible capstone connecting scenario, evidence, detection, remediation and non-technical briefing.

## Detailed episode catalogue

### Phase 1 — Linux and command-line foundations (EP-001–018)
- EP-001: Terminal basics: pwd, ls, ls -l (covered)
- EP-002: Navigation: cd, paths, . and .. (covered)
- EP-003: Files and directories: mkdir, touch, cp, mv, rm, rmdir (covered)
- EP-004: Viewing/searching contents: cat, less, head, tail, grep (covered)
- EP-005: Linux permission model and ls -l (covered)
- EP-006: chmod, chown, chgrp and least privilege (covered; ownership lab to revisit)
- EP-007: Users, groups, identity and sudo (covered)
- EP-008: Processes, PIDs, CPU/memory and safe investigation (covered)
- EP-009: Services and systemctl (covered)
- EP-010: Logs, journalctl and authentication log variations (covered; recap pending)
- EP-011: Linux networking commands: ip, ping, ss, curl and DNS lookup (next after recap)
- EP-012: Package management and software updates
- EP-013: Finding files and filtering results: find and grep practice
- EP-014: Compression, archives and safe file handling
- EP-015: SSH and secure remote access
- EP-016: Bash fundamentals: variables, conditions, loops and exit codes
- EP-017: Bash scripting for security tasks
- EP-018: Linux security investigation checkpoint

### Phase 2 — Networking and Internet fundamentals (EP-019–030)
- EP-019: Internet basics and client-server communication
- EP-020: IPv4, private/public addresses, ports and socket basics
- EP-021: TCP vs UDP and TCP handshake
- EP-022: DNS, DHCP and ARP
- EP-023: Routing, gateways, NAT and subnetting
- EP-024: OSI and TCP/IP models
- EP-025: HTTP requests, responses, methods and status codes
- EP-026: HTTPS, TLS and certificates
- EP-027: Common protocols and their security implications
- EP-028: Firewalls and network security controls
- EP-029: Wireshark packet analysis
- EP-030: Network investigation challenge

### Phase 3 — Windows, identity and endpoint security (EP-031–042)
- EP-031: Windows architecture and filesystem
- EP-032: Windows users, groups and privileges
- EP-033: Services, scheduled tasks and processes
- EP-034: PowerShell fundamentals
- EP-035: Event Viewer and Windows event logs
- EP-036: Windows authentication and logon events
- EP-037: Active Directory fundamentals
- EP-038: Entra ID and cloud identity concepts
- EP-039: Endpoint security and hardening
- EP-040: Persistence and suspicious activity basics
- EP-041: Windows investigation lab
- EP-042: Endpoint security checkpoint

### Phase 4 — Security fundamentals and vulnerability management (EP-043–054)
- EP-043: Confidentiality, integrity and availability
- EP-044: Threats, vulnerabilities, exploits and risk
- EP-045: Authentication, authorisation and MFA
- EP-046: Cryptography, hashes and certificates basics
- EP-047: Least privilege and secure configuration
- EP-048: Patch management and attack surface
- EP-049: Vulnerability scanners and manual validation
- EP-050: CVSS, severity and business impact
- EP-051: Firewalls, EDR and security control types
- EP-052: MITRE ATT&CK and attack lifecycle concepts
- EP-053: Risk registers and ISO 27001/NIST overview
- EP-054: Prioritisation and remediation lab

### Phase 5 — Web and API security (EP-055–072)
- EP-055: How web applications work
- EP-056: HTML, JavaScript, forms and browser DevTools
- EP-057: Burp Suite Proxy, Repeater and safe setup
- EP-058: Cookies, sessions and authentication
- EP-059: SQL injection (SQLi)
- EP-060: Cross-site scripting (XSS)
- EP-061: Access control and IDOR
- EP-062: Authentication and session flaws
- EP-063: CSRF and SameSite cookies
- EP-064: Path traversal and file handling
- EP-065: File-upload vulnerabilities
- EP-066: OS command injection
- EP-067: SSRF and XXE
- EP-068: CORS, clickjacking and security headers
- EP-069: REST APIs and API security
- EP-070: JWT and token security
- EP-071: Testing methodology, validation and remediation
- EP-072: Web application assessment report

### Phase 6 — Ethical testing and reconnaissance (EP-073–084)
- EP-073: Rules of engagement, legal boundaries and scope
- EP-074: Reconnaissance and asset inventory
- EP-075: DNS and subdomain enumeration in authorised labs
- EP-076: Nmap ports and service detection
- EP-077: Content discovery in a lab
- EP-078: Manual validation versus scanner output
- EP-079: Reproducing findings and collecting evidence
- EP-080: CVSS, prioritisation and report quality
- EP-081: CTF methodology and hint-driven problem solving
- EP-082: PortSwigger or TryHackMe practical challenge
- EP-083: Retesting fixes and writing remediation advice
- EP-084: Mini penetration-testing engagement simulation

### Phase 7 — SOC, detection and incident response (EP-085–100)
- EP-085: SOC workflows, alert lifecycle and triage
- EP-086: Log sources, normalisation and timelines
- EP-087: IOC enrichment and threat intelligence
- EP-088: MITRE ATT&CK mapping in investigations
- EP-089: Incident response lifecycle
- EP-090: SIEM fundamentals and data ingestion
- EP-091: Microsoft Sentinel and KQL fundamentals
- EP-092: Splunk and SPL fundamentals
- EP-093: Detection logic and Sigma-style rules
- EP-094: False positives, tuning and validation
- EP-095: Windows security event investigations
- EP-096: Linux authentication and process investigations
- EP-097: Web attack signals in logs
- EP-098: Threat hunting and hypothesis testing
- EP-099: Incident report and response recommendations
- EP-100: Integrated SOC investigation

### Phase 8 — Cloud and cloud identity security (EP-101–112)
- EP-101: Cloud shared responsibility and core concepts
- EP-102: Select one cloud provider based on target jobs
- EP-103: IAM, roles and least privilege
- EP-104: Cloud audit logs and activity trails
- EP-105: Storage exposure and secrets management
- EP-106: Cloud networking and security groups
- EP-107: Cloud identity and suspicious sign-ins
- EP-108: Cloud misconfiguration assessment
- EP-109: Basic container and image security
- EP-110: Cloud alerting and SIEM integration
- EP-111: Investigate and remediate a cloud security incident
- EP-112: Cloud security checkpoint

### Phase 9 — Python, automation and AI security (EP-113–124)
- EP-113: Python refresher for security work
- EP-114: Files, JSON, CSV and regular expressions
- EP-115: Parse and summarise security logs
- EP-116: IOC extraction and enrichment
- EP-117: APIs, HTTP clients and safe error handling
- EP-118: Automate repeatable security checks
- EP-119: Git, testing and reproducible scripts
- EP-120: AI-assisted analysis and verification
- EP-121: LLM application risks and prompt injection
- EP-122: OWASP LLM risks in a safe lab
- EP-123: Human validation of AI triage results
- EP-124: Security automation capstone

### Phase 10 — Integrated projects, risk and career readiness (EP-125 onward)
- EP-125: Integrated attack-to-detection case study
- EP-126: Risk assessment and security controls
- EP-127: Privacy and data-protection overview
- EP-128: Portfolio review and project hardening
- EP-129: Resume and LinkedIn evidence review
- EP-130: Technical interview practice
- EP-131: Explain a technical finding to a non-technical audience
- EP-132: Mock incident briefing and Q&A
- EP-133: Job-description analysis and applications
- EP-134: Career review and next specialist plan

## Portfolio projects (build progressively)
1. Linux log investigation + Bash/Python analyser.
2. Network traffic investigation with Wireshark.
3. SIEM detection lab with ATT&CK-mapped rules.
4. Web/API assessment report with remediation and retest.
5. Cloud misconfiguration investigation.
6. IOC extraction and AI-assisted triage with validation.
7. Integrated case study: scenario, logs, detection, response, fix and plain-English briefing.

Every project README should include scope/permission, scenario, steps, evidence, interpretation, impact, fix/verification, limitations, and next steps.
