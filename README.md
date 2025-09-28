# offsec-utils
A personal collection of red-team utilities, scripts, and lab writeups.  
Purpose: practice offensive security skills and build repeatable workflows.  
**For lab use only. Not intended for unauthorized activity.**

---

## Repository structure

offsec-utils/
├─ scripts/ # Python + Bash scripts
├─ tools/ # Small custom utilities
├─ labs/ # Local lab configs and notes
├─ writeups/ # HTB, THM, CTF writeups
└─ docs/ # Cheatsheets and workflows

---

## Quick start

```bash
git clone https://github.com/jacobmacdonnell/offsec-utils.git
cd offsec-utils

# optional: create and activate venv
python -m venv .venv
source .venv/bin/activate

# run example
python3 scripts/python/nmap_parse.py scans/scan.xml
