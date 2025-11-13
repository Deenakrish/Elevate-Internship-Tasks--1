                                                  Cyber Security Internship: Task 1 — Network Scanning

Project: Basic network reconnaissance (Nmap)
Date: 13-11-2025
Environment: Linux (Nmap pre‑installed)

Objective

Discover live hosts and open ports on my local /24 network, identify running services and versions, run vulnerability checks with Nmap NSE, capture example traffic with Wireshark, and produce actionable remediation recommendations.

Short summary (one line)

I used Nmap to discover live hosts, open TCP/UDP ports, service/version information, and OS fingerprints; then ran vulnerability-oriented NSE scripts.

Key findings

Hosts up (2):

HOST 1-10.178.XX.XX

Open: 53/tcp — dnsmasq 2.51

Device: Android phone (Android 9–10 / Linux 4.x)

Vulnerabilities found: multiple high-severity CVEs for dnsmasq 2.51 (see scans/10.178.XX.XX_vuln.txt for full list).

HOST 2-10.178.XX.XX

Open: 443/tcp — HTTPS (service not fully fingerprinted)

Device: General-purpose Linux (Linux 5.x/6.x)

Vulnerabilities found: likely vulnerable to Slowloris DoS; HTTP verb tampering possible (authentication bypass on specific URIs).

Note: Some findings reference public exploits. The vulnerability I found can be exploited using Metasploit — do not attempt exploitation on networks/devices you do not own; validate exploits only in a controlled lab with written permission.
