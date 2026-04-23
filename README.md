# Nmap Practice

This repository documents my hands-on experience using Nmap for network scanning and enumeration in controlled lab environments.

## Tool

- Nmap (network scanning and enumeration)

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

Target: scanme.nmap.org

Command:

```
nmap -sS -A scanme.nmap.org -oN scan1.txt
```

## Findings

* Open ports discovered (e.g., 22, 80, 443)
* Service enumeration performed:

  * 22 → SSH
  * 80 → HTTP
  * 443 → HTTPS
* Basic OS detection completed

## Output

Scan results are saved in:

* `or3ali.txt`

## Notes

* All scans are performed on authorized targets (e.g., scanme.nmap.org)
* This repository is for educational and ethical cybersecurity practice only
