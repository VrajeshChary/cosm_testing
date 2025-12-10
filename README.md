# Computer-Oriented Statistical Methods - Hypothesis Testing on Payments Dataset

![Status: Experimenting](https://img.shields.io/badge/status-experimental-yellow)
![Dataset](https://img.shields.io/badge/dataset-88MB-red)

Welcome to **cosm_testing** — a sleek, data-driven notebook project that explores payroll statistics, hypothesis testing, and multiple linear regression using a real-world dataset. This repo contains a polished Jupyter notebook (`ml.py.ipynb`) with exploratory analysis, inferential statistics, and visualization recipes, plus the raw `data.csv` used for all analyses.

Why you'll love this repo
- **Beautifully documented notebook**: step-by-step statistical workflows (Z-test, T-tests, Chi-square, ANOVA, Regression) with reproducible plotting code.
- **Ready-to-run**: open the notebook in Jupyter or VS Code and run cells — everything is self-contained.
- **Practical insights**: great for learning statistics applied to payroll data, or as a starting point for ML feature experiments.

Contents
- `ml.py.ipynb` — The main Jupyter notebook. Readme-friendly walkthrough, visualizations, and regression modeling.
- `data.csv` — The payroll dataset (large; ~88 MB). Used by the notebook for all analyses and plots.

Quick Start
1. Clone the repo (if you haven't already):

```powershell
git clone https://github.com/VrajeshChary/cosm_testing.git
cd cosm_testing
```

2. (Optional) Create a Python virtual environment and activate it:

```powershell
python -m venv .venv ; .\.venv\Scripts\Activate.ps1
```

3. Install the core dependencies:

```powershell
pip install pandas numpy scipy statsmodels matplotlib seaborn jupyter
```

4. Start Jupyter and open the notebook:

```powershell
jupyter notebook ml.py.ipynb
```

Notebook Highlights
- Data cleaning and currency parsing utilities for messy payroll fields.
- Z-test and one-/two-sample T-tests to check mean differences.
- Chi-square tests for categorical association checks.
- ANOVA across departments and post-hoc-ready visuals.
- Multiple Linear Regression using `statsmodels` with detailed diagnostic plots (residuals, QQ, predicted vs actual).

Notes & Recommendations
- Large dataset: `data.csv` is ~88 MB — above GitHub's recommended limit. Consider using Git LFS for the CSV to keep the repo lightweight.

  To migrate to Git LFS locally (suggested):

```powershell
git lfs install
git lfs track "data.csv"
git add .gitattributes
git rm --cached data.csv
git add data.csv
git commit -m "Move data.csv to Git LFS"
git push
```

- If you prefer a smaller demo, extract a sample subset and save it (e.g., `data_sample.csv`) to try the notebook quickly.

Customization & Extensions
- Swap the regression formula in the notebook to include department dummies or job-class features.
- Add a `requirements.txt` by running:

```powershell
pip freeze > requirements.txt
```

Contributing
- Bug fixes, notebook improvements, or nicer visual themes are welcome. Open an issue or a PR on GitHub.

License
- This repository is provided as-is for educational use. Add a LICENSE file if you want formal terms.

Contact
- Repo owner: `VrajeshChary` — open an issue or reach out via GitHub.

Enjoy exploring the numbers — and if you want, I can:
- migrate `data.csv` to Git LFS for you, or
- add a focused `requirements.txt`, `.gitignore`, or a compact sample dataset.
