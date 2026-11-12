# Contributing to Macro-Modelling

Thank you for sharing your work. These guidelines keep the library consistent, reproducible and easy to use for everyone.

---

## Who can contribute

Anyone with a GitHub account: academics, PhD students, central-bank and policy economists, and practitioners. You do not need to be invited.

---

## What we accept

- Implementations of macroeconomic models (structural, empirical, climate–macro, macro-finance)
- Replication packages for published papers or working papers
- Teaching versions of standard models, with clear documentation
- Improvements, bug fixes or extensions of models already in the repository

We do **not** accept:
- Code you do not have the right to share
- Confidential, proprietary or personally identifiable data
- Very large files (over 50 MB). Please host large data elsewhere (Zenodo, OSF, a data provider) and link to it, or add a download script.

---

## Step-by-step: submitting a model

### Option A: in the browser (no Git knowledge needed)

1. Click **Fork** (top right) to create your own copy of this repository.
2. In your fork, go to the right category under `models/` (e.g. `models/climate/`).
3. Click **Add file → Create new file** and type the folder name followed by `/README.md`, e.g.
   `models/climate/transition-risk-dsge_rossi/README.md`
   (typing the `/` creates the folder).
4. Use **Add file → Upload files** to add your code and data into that folder.
5. Go back to your fork's main page and click **Contribute → Open pull request**.
6. Fill in the pull-request description and submit.

### Option B: with Git

```bash
git clone https://github.com/<your-username>/Macro-Modelling.git
cd Macro-Modelling
git checkout -b add-model-name
# add your folder under models/<category>/
git add .
git commit -m "Add <model name> (<author>)"
git push origin add-model-name
```
Then open a pull request from your fork on GitHub.

---

## Folder naming and structure

Name your folder `model-name_author-surname`, in lowercase with hyphens, e.g. `hank-climate_bianchi`.

```
model-name_author-surname/
├── README.md          required
├── code/              required
├── data/              data files, or a download script / link
├── output/            optional: example figures or tables
└── requirements.txt   required (or environment.yml / Project.toml / renv.lock)
```

---

## The model README: required information

Every model folder must contain a `README.md` with at least the following. Copy this template:

```markdown
# Model name

**Author(s):** Name Surname (Affiliation), ...
**Contact:** email or GitHub handle
**Reference paper:** Author (Year), "Title", Journal / Working Paper series. DOI or link
**Category:** DSGE / Empirical / Climate / Finance
**Language and version:** e.g. MATLAB R2023b + Dynare 6.1; Python 3.11
**License:** MIT (or specify)

## Description
Two or three paragraphs: what the model does, key mechanisms, main results.

## Data
Sources, vintage/date accessed, licence or terms of use, and how to obtain them.

## How to run
1. Install dependencies: ...
2. Run: `main.m` / `python main.py` / ...
3. Expected runtime and hardware: ...

## Output
What the code produces (figures, tables) and where it is saved.

## Notes
Known limitations, calibration choices, differences from the published version.
```

---

## Code quality checklist

Before opening a pull request, please make sure that:

- [ ] The code **runs from start to finish** in a clean environment
- [ ] There is **one main entry-point script** (e.g. `main.m`, `main.py`, `run.R`)
- [ ] File paths are **relative**, not absolute (no `C:\Users\...`)
- [ ] Dependencies and versions are listed
- [ ] The code is commented where the logic is not obvious
- [ ] No passwords, API keys or personal data are included
- [ ] Large data files are linked rather than uploaded
- [ ] You have the right to share the code and data under the stated licence

---

## Review process

1. A member of the E-axes Forum team reviews your pull request, usually within two weeks.
2. We check structure, documentation and, where feasible, that the code runs.
3. We may ask for changes in the pull-request conversation.
4. Once approved, your model is merged and listed in the repository.

The review checks completeness and reproducibility. It is not a scientific peer review of the model.

---

## Updating your model

To fix bugs or update your model, open a new pull request that changes only your model folder. Please describe what changed and why.

---

## Reporting problems or proposing models

- **Bug in a model?** Open an [Issue](https://github.com/eaxesforum/Macro-Modelling/issues) and tag the model folder name.
- **Idea for a model or feature?** Open an Issue labelled `proposal`.

---

## Licensing of contributions

By submitting a pull request, you confirm that you have the right to share the code and that it is released under the MIT License (or the licence stated in your model folder). You keep the copyright to your work.

---

## Code of conduct

Please be respectful and constructive in all interactions. Harassment or discriminatory behaviour will not be tolerated.

---

Questions? Contact **info@e-axes.org**.
