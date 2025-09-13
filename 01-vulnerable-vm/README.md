# Assignment 1 — Vulnerable VM Creation

## Scenario & Scope
The project focused on realistic “company mail server” (Ubuntu Server 20.04) with software up-to-date but **security misconfigurations** that enable local footholds and privilege escalation.

## What’s Inside
- **Report:** `VulnerableMachineDesign.pdf` — full report on the vulnerability crafted inside the VM.  

## Methods (High Level)
- **Local access:**  
  - Weak SSH credential on a leftover test account (`guest`).  
  - SMTP user enumeration + **Hydra** brute-force to recover a user password from SecLists.  
  - Email workflow abuse: base64-encoded attachment recovered via SFTP, ZIP cracked to retrieve credentials.  
- **Privilege escalation:**  
  - `sudo` misconfiguration allowing interactive shell (`fish`) to run with elevated rights.  
  - **Footprinting** the director’s public profile to derive a DOB-based password (demonstrates OSINT risk).  
  - SUID helper and **over-permissive SSH key files** enabling root access when combined with process/file-descriptor tricks.
 
  ## VM (OVA)
  **Download:** [Google Drive](https://drive.google.com/file/d/1avzkSMauvH16BbbR6_ifhJHaDNgqmDV1/view?usp=sharing) <br>
  **Run:** Import the OVA into **VirtualBox**, then start the VM.
