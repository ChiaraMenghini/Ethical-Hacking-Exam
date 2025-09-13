# Ethical Hacking Labs 2024 🧩🛡️

## Overview
Two team-based penetration-testing assignments from the Ethical Hacking course:
1) an intentionally vulnerable VM we designed to simulate real-world misconfigurations;  
2) a separate vulnerable VM assigned to our team, which we enumerated and exploited.

Each assignment followed the same rubric: **3 local-access vulnerabilities** and **3 privilege-escalation paths**, with full documentation and reproducibility notes.

## ⚠️ Safety Notice
For educational/academic use only. All work was performed against **isolated lab VMs** we owned or were explicitly authorized to test. Do **not** reuse techniques against systems you do not own or operate without *written* permission. The authors assume no responsibility for misuse.

## Contents
| Path | Description |
| --- | --- |
| `/01-vulnerable-vm/` | We designed and documented an intentionally vulnerable Ubuntu Server 20.04 VM (mail/SSH stack). Includes scenario, threat model, and exploitation summary. |
| `/02-assigned-vm-exploit/` | Engagement report for a provided vulnerable VM: enumeration, exploitation, post-ex, and remediation. |

## Tools & Environment
**Environment:** VirtualBox/VMware; Kali/Parrot attack VM; target Ubuntu Server 20.04.  
**Discovery & Enumeration:** nmap, gobuster/feroxbuster, smtp-enum modules, manual recon.  
**Exploitation & Post-Ex:** Metasploit (select modules), netcat, reverse shells, GTFOBins, `sudo -l`.  
**Credential Attacks:** Hydra, hashcat, SecLists wordlists.  
**Network:** Wireshark (PCAP), tcpdump.  
**Write-ups:** PDF reports with reproduction steps, analysis, and remediation.

> Sensitive artifacts (e.g., VM images, key material, cracked hashes) are **excluded** or placed in password-protected archives with clear labeling. See each assignment’s `artifacts/` notes.
