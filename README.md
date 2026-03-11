# Hospital Admission Records Analysis

## Team Members

- Zaid
- Diala

## Project Overview

This project analyzes hospital admission records to identify trends in patient intake and resource utilization. The insights are intended for hospital administrators to optimize staffing and reduce wait times.

## Data Sources

Data is not tracked in this repository. See the setup instructions below
for how to obtain and place the data files before running any analysis.

_Data should be placed in `data/raw/admissions.csv`._

## Setup Instructions

```bash
git clone <repo-url>
cd <repo-name>
python -m venv .venv
```

Activate the virtual environment — choose the command for your OS:

```bash
# Mac / Linux
source .venv/bin/activate

# Windows Git Bash
source .venv/Scripts/activate

# Windows CMD
.venv\Scripts\activate.bat

# Windows PowerShell
.venv\Scripts\Activate.ps1
```

Once activated, install dependencies and verify the environment:

```bash
pip install -r requirements.txt
python test_environment.py
```

`test_environment.py` should print "Environment OK" when the setup is correct.

## Project Structure

```text
aispire-foundations/
├── README.md             — Project overview and setup instructions
├── CHANGELOG.md          — Record of notable changes
├── AGENTS.md             — AI contribution policy
├── requirements.txt      — Python dependencies
├── setup.sh              — Automated environment setup script
├── test_environment.py   — Environment validation
├── .gitignore            — Files excluded from version control
├── src/                  — Production source code (importable modules)
├── notebooks/            — Exploratory analysis notebooks
├── data/                 — Data directory (contents not committed to Git)
│   └── raw/              — Original unmodified data files
└── tests/                — Automated tests
```

## Contributing

- Branch naming convention: e.g., `feature/`, `setup/`, `fix/`
- Open a PR to `main` for all changes
- Commit messages: imperative mood, ≤ 50 characters
