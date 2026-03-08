[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/FdVrU54p)
# Lab 1 — Git Workflows and Environment Setup

> **Lab 1 starter repo** — Replace the heading above with your project title. Team member names are not part of the lab — they go in Section 2 of your completed README in the integration task.

---
## Team Members

- Diala Abdullqader
- Nasser Obaid
- Alex Chen 
## Project Overview

This repository establishes a reproducible Python development environment for the AI.SPIRE Foundations project. The goal is to ensure that any contributor or reviewer can clone the repository, set up the environment, and verify that it works in a consistent way across machines.

The repository includes dependency management using requirements.txt, a Python virtual environment setup, and a verification script (test_environment.py) to confirm the environment is configured correctly.
---
## Data Sources
This project will analyze hospital admission data for a regional health authority.

Data files are not tracked in this repository. Before running any analysis, place the dataset in the following directory:
```bash
data/raw/admissions.csv
```

This ensures that large or sensitive data files are not committed to version control.

## Setup Instructions

TODO: Complete these setup steps after creating your `requirements.txt`:

```bash
python -m venv .venv

# Activate — choose the command for your OS:
# Mac / Linux:      source .venv/bin/activate
# Windows Git Bash: source .venv/Scripts/activate
# Windows CMD:      .venv\Scripts\activate.bat
# Windows PowerShell: .venv\Scripts\Activate.ps1

pip install -r requirements.txt
python test_environment.py    # should print "Environment OK"
```

---
## Project Structure
m1-l1-git-workflows-MsDiala/
├── README.md                — Project overview and setup instructions
├── README-template.md       — Starter template provided for the lab
├── AGENTS.md.template       — Template for AI contribution policy
├── setup.sh.template        — Template for automated environment setup
├── requirements.txt         — Python dependencies (pandas, matplotlib)
├── test_environment.py      — Script that verifies the environment setup
├── tests/                   — Automated tests used by the autograder
│   ├── test_environment_runs.py
│   ├── test_gitignore_has_venv.py
│   ├── test_integration_structure.py
│   ├── test_lab_structure.py
│   └── test_requirements_txt.py
└── __pycache__/             — Python cache files generated automatically

## Contributing

- Branch naming: `setup/`, `feature/`, `fix/`
- Open a PR to `main` for all changes
- Commit messages: imperative mood, ≤ 50 characters

---

*Starter file for Lab 1 — lab-1-git-workflows | aispire-14005*