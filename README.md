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
  
**Evidence:** 

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


