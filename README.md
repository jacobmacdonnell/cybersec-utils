# offsec-utils

A personal collection of red-team utilities, scripts, and lab writeups.  
Purpose: practice offensive security skills and build repeatable workflows.  
**For lab use only. Not intended for unauthorized activity.**

---

## Repository structure

    offsec-utils/
    ├─ scripts/        # Python + Bash scripts
    ├─ tools/          # Small custom utilities
    ├─ labs/           # Local lab configs and notes
    ├─ writeups/       # HTB, THM, CTF writeups
    ├─ docs/           # Cheatsheets and workflows
    ├─ ci/             # CI config (optional)
    ├─ .pre-commit-config.yaml
    ├─ requirements-dev.txt
    └─ LICENSE

---

## Quick start

```bash
git clone https://github.com/jacobmacdonnell/offsec-utils.git
cd offsec-utils

# create and activate venv (recommended)
python -m venv .venv
source .venv/bin/activate

# install dev deps (for linters / pre-commit)
pip install -r requirements-dev.txt

# install pre-commit hooks
pre-commit install

# run hooks once on all files
pre-commit run --all-files

# generate detect-secrets baseline (one-time)
detect-secrets scan > .secrets.baseline
git add .secrets.baseline

# run example (requires a sample Nmap XML file)
python3 scripts/python/nmap_parse.py scans/scan.xml
