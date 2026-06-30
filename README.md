# MSAAI-501 — Foundations of Artificial Intelligence & Machine Learning

Coursework, experiments, and Jupyter notebooks for **MSAAI-501** (Semester 1).

## Project layout

```
.
├── notebooks/          # Jupyter notebooks (one per assignment / topic)
├── src/                # Reusable Python modules imported by the notebooks
├── data/
│   ├── raw/            # Original, immutable data (git-ignored)
│   ├── processed/      # Cleaned / transformed data (git-ignored)
│   └── external/       # Third-party data (git-ignored)
├── models/             # Saved model artifacts (git-ignored)
├── requirements.txt    # Python dependencies
└── README.md
```

## Getting started

1. **Create and activate a virtual environment** (Python 3.11+):

   ```bash
   python3 -m venv .venv
   source .venv/bin/activate        # Windows: .venv\Scripts\activate
   ```

2. **Install dependencies:**

   ```bash
   pip install -r requirements.txt
   ```

3. **Register the environment as a Jupyter kernel:**

   ```bash
   python -m ipykernel install --user --name msaai-501 --display-name "Python (MSAAI-501)"
   ```

4. **Launch JupyterLab:**

   ```bash
   jupyter lab
   ```

   Then open a notebook from `notebooks/` and select the **Python (MSAAI-501)** kernel.

## Notes

- Keep raw data out of version control — it lives in `data/raw/` which is git-ignored.
- Put shared helper code in `src/` and import it from notebooks (e.g. `from src.utils import ...`).
