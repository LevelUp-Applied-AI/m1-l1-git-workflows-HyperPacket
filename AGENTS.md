# AI Contribution Policy

## Testing Requirements

All changes must pass `python test_environment.py` before committing.
Any new code added to the `src/` directory (which will contain our modular production pipeline) must have a corresponding test in `tests/` that passes with `pytest tests/ -v`.
For any data analysis or modeling changes, the exploratory notebooks in `notebooks/` must be able to "Run All" without throwing an error before opening a PR.

## Secrets Policy

Do not include API keys, database credentials, or file paths containing personal data or protected health information (PHI) in any prompt. Never commit `.env`, `*.key`, or any file containing credentials.
Raw hospital admission records (`data/raw/admissions.csv` and similar) contain sensitive data and should never be exposed in prompts or committed to git. 

## Scope Boundaries

Agents may edit Python files in `src/` and Jupyter notebooks in `notebooks/`.
Do not modify `requirements.txt` without human review.
Do not modify `setup.sh` without running and testing the script locally first.
Do not touch `.gitignore` without confirming the change doesn't accidentally exclude essential source files or include sensitive data/raw files.

## Reproducibility Standard

All AI-assisted changes require local-first execution: the change must run locally in the Python environment and produce the expected output before it is committed or pushed. "The AI generated it" is not a substitute for running and verifying it locally against the actual hospital admission dataset.
