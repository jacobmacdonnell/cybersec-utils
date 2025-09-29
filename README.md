# offsec-utils

Personal collection of red-team scripts and lab writeups.  
Purpose: practice offensive security skills.  
**Lab use only. Do not run against systems you do not own or have permission to test.**

---

## Repository structure

    offsec-utils/
    ├─ scripts/        # one-off helpers (bash, python, etc.)
    ├─ writeups/       # HTB / THM / CTF notes and walkthroughs
    └─ README.md

---

## Quick start

```bash
git clone https://github.com/jacobmacdonnell/offsec-utils.git
cd offsec-utils

# run a Python script
python3 scripts/nmap_parse.py scans/scan.xml

# or a Bash script
bash scripts/quick_scan.sh target.example
