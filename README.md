# Ethical Hacking Labs 2024 🧩🛡️

## Overview
Two team-based penetration-testing assignments from the Ethical Hacking course:
1) an intentionally vulnerable VM we designed to simulate real-world misconfigurations;  
2) a separate vulnerable VM assigned to our team, which we enumerated and exploited.

Each assignment followed the same structure: **3 local-access vulnerabilities** and **3 privilege-escalation paths**, with full documentation.

## ⚠️ Safety Notice
For educational/academic use only. All work was performed against **isolated lab VMs** we were explicitly authorized to test. Do **not** reuse techniques against systems you do not own or operate without *written* permission. The authors assume no responsibility for misuse.

## Contents
| Path | Description |
| --- | --- |
| `/01-vulnerable-vm/` | Designed and documented an intentionally vulnerable Ubuntu Server 20.04 VM. Includes scenario, threat model, and exploitation summary. |
| `/02-assigned-vm-exploit/` | Detailed report for vulnerable VM exploitation. |

## Main tools & Environment
**Environment:** VirtualBox; Parrot OS attack VM; target Ubuntu Server 20.04.  
**Discovery & Enumeration:** nmap, gobuster, smtp-enum modules, manual recon.  
**Exploitation & Post-Ex:** Metasploit, netcat, reverse shells, GTFOBins.  
**Credential Attacks:** Hydra, hashcat, SecLists wordlists.  
**Network:** Wireshark (PCAP), tcpdump.  
**Write-ups:** PDF reports with reproduction steps, analysis, and remediation.

