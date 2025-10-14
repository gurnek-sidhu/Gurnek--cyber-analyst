# Gurnek--cyber-analyst
# ITECH1502 — TryHackMe Project
**Author:** Gurnekpreet Kaur  
**FedUni email:** gurnekpreetk@students.federation.edu.au  
**Date:** 2025-10-19

## Project Overview
This repository documents three TryHackMe activities completed for ITECH1502:
1. Offensive Security (practical exploitation & reconnaissance)
2. Defensive Security Intro (defense fundamentals & monitoring)
3. Careers in Cyber (career guidance & next steps)

.

---


# Offensive Security
**TryHackMe Room:**
offensive security introduction  
  
**Evidence:** <img width="1470" height="956" alt="Image" src="https://github.com/user-attachments/assets/9637b10d-a400-463b-81a1-b3113c6d1958" />

](url)

## Summary
This activity focused on reconnaissance, scanning, enumeration, and basic exploitation in a lab environment. I used Nmap, Gobuster, and manual HTTP requests to find vulnerabilities and retrieve the room flag(s).

## Objectives
Look around the website (enumeration)
- “Next I explored the web app to find hidden pages and inputs — things like /admin, /uploads, or weird query parameters. I used directory checks and just looked at the site in a browser to see what files and pages existed. I kept a list of interesting URLs and screenshots to show what I found.”
## Tools Used

- Gobuster (directory enumeration)


## Methodology (step-by-step)

3. Ran Gobuster to find directories: gobuster -u http://fakebank.thm -w wordlist.txt dir  
4. Manually inspected discovered paths in a browser and discovered secret fakeBank website page for money transfer.
5. Retrieved the flag and saved a screenshot 

## Results
-  transfered $2000 from bank account 2276 to your account (account number 8881). 
- Hidden directories discovered via Gobuster (list saved in evidence).  
- Flag captured and screenshot saved.

## Reflection
This task reinforced the importance of careful enumeration — most successful attacks begin with finding small oversights like exposed directories or misconfigured files. Next steps: learn privilege escalation techniques and practice safe reporting.

# Defensive Security Intro
**TryHackMe Room(s):** Replace with exact room names (e.g., `Blue Team Basics`)  
 
**Evidence:** https://tryhackme.com/room/defensivesecurityintroQR?sharerId=68ee22ad92b9ec48c3b6cce9 
- <img width="1470" height="956" alt="Image" src="https://github.com/user-attachments/assets/355a3a24-e9b2-4a55-bcb0-9b43e1332ffb" /> 
## Summary
This activity introduced defensive concepts such as logging, host-based monitoring, basic firewall configuration, and how to interpret security logs for indicators of compromise.

## Objectives
- Understand the role of logs and monitoring in detection.  
- Learn basic host hardening / firewall settings.  
- Perform simple log analysis to identify suspicious events.

## Tools & Concepts
- Syslog / journalctl (log sources)
- UFW / iptables (basic host firewall)
- File integrity monitoring (conceptual)
- SIEM basics (Splunk/ELK concepts; screenshots of searches saved as evidence)

## Methodology (step-by-step)
1. Reviewed syslog entries from the lab VM and saved suspicious lines to `evidence/defensive_syslog.txt`.  
2. Checked firewall status and documented configuration: `sudo ufw status verbose > evidence/defensive_ufw_status.txt`.  
3. Performed basic log queries in the lab SIEM (or used Splunk/ELK playground) and saved screenshots to `evidence/defensive_monitoring.png`.  
4. Wrote brief remediation suggestions for observed issues (e.g., disable unused services, enforce strong SSH configs).

## Results
- Identified suspicious login attempts in syslog (example saved).  
- Documented the host firewall state and suggested hardening steps.  
- Saved SIEM query screenshot showing a sample alert.

## Reflection
Understanding the defender's view clarified how detection and timely response stop attackers. Next steps: practice writing SIEM queries, learn alert tuning, and explore host-based monitoring (OSSEC, Wazuh).

# Careers in Cyber
**TryHackMe Room(s):** Replace with exact room name(s) (e.g., `Careers in Cyber`)  
  
**Evidence:** `https://tryhackme.com/room/careersincyber?sharerId=68ee22ad92b9ec48c3b6cce9
<img width="1470" height="956" alt="Image" src="https://github.com/user-attachments/assets/8f1aca8f-b72d-42b4-9449-5a00bf8f9b64" />

## Summary
This activity covered career pathways, required skills, learning resources, certifications, and practical next steps to build a career in cybersecurity.

## Key Takeaways
- Common entry roles: SOC Analyst, Junior Penetration Tester, Incident Responder, Security Operations.  
- Recommended certifications/learning: CompTIA Security+ (intro), eJPT/OSCP (offensive), CSX/Splunk/Certified SOC Analyst (defensive).  
- Skills to develop: Linux CLI, networking fundamentals, scripting (Python/Bash), log analysis, threat-hunting basics.

## Action Plan / Next Steps
1. Build a GitHub portfolio with documented labs (this repo).  
2. Complete a certification roadmap (Security+ → eJPT → OSCP or equivalent).  
3. Join local/online CTFs and community groups; network via LinkedIn and local meetups.  
4. Prepare an interview-focused project: explain methodology, evidence, and mitigation.


## Reflection
This module helped crystallize a clear path forward: concentrate on foundational skills, build demonstrable artifacts (GitHub + TryHackMe), and target entry-level roles with project-based evidence.

