# Nmap Practice

This repository documents my hands-on experience using Nmap for network scanning and enumeration in controlled lab environments.

## Tool

* Nmap (network scanning and enumeration)

## Objectives

* Identify open ports on target systems
* Detect running services and versions
* Perform basic OS fingerprinting
* Understand network exposure and attack surface

## Commands Used

* `nmap -sS` — TCP SYN scan (stealth scan)
* `nmap -A` — Aggressive scan (OS detection, version detection, scripts)
* `nmap -p-` — Scan all ports
* `nmap -sV` — Service version detection

## Sample Scan

**Target:** scanme.nmap.org

**Command:**

```
nmap -sS -A scanme.nmap.org -oN or3ali.txt
```

## Findings

* Discovered open ports: 22, 80, 9929, 1337
* Filtered ports detected: 25 (SMTP), 5060 (SIP)

### Service Enumeration

* 22 → SSH (tcpwrapped)
* 80 → HTTP (Apache 2.4.7 - Ubuntu)
* 9929 → Nping Echo
* 1337 → tcpwrapped

### Additional Observations

* Target is running Linux (kernel 4.x – 5.x)
* HTTP service identified with Apache server
* Network distance: ~22 hops

## Output

Scan results are saved in:

* `or3ali.txt`

## Notes

* All scans are performed on authorized targets (e.g., scanme.nmap.org)
* This repository is for educational and ethical cybersecurity practice only

## Skills Demonstrated

* Network scanning
* Port enumeration
* Service detection
* Basic reconnaissance methodology
