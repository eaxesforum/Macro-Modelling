# Macro-Modelling

**An open library of macroeconomic models, curated by the [E-axes Forum](https://e-axes.org).**

This repository brings together replication code and model implementations from researchers working in macroeconomics, with a particular focus on climate economics, sustainable finance and monetary-financial interactions. The goal is to make models easy to find, run, compare and build on.

---

## What you will find here

- **Structural models**: DSGE, E-DSGE (environmental DSGE), HANK, OLG
- **Empirical models**: VAR, SVAR, local projections, panel models
- **Climate–macro models**: integrated assessment models (IAMs), transition-risk and physical-risk models, climate stress-testing frameworks
- **Financial models**: macro-finance, banking and non-bank sector models
- **Replication packages** for published and working papers

Supported languages include **MATLAB / Dynare, Python, R and Julia**. Other languages are welcome if documented clearly.

---

## Repository structure

```
Macro-Modelling/
├── README.md               ← you are here
├── CONTRIBUTING.md         ← how to submit a model
├── CITATION.cff            ← how to cite this repository
├── LICENSE
└── models/
    ├── dsge/
    │   └── model-name_author-surname/
    ├── empirical/
    ├── climate/
    └── finance/
```

Each model lives in its own folder, which always contains:

```
model-name_author-surname/
├── README.md          description, reference paper, how to run
├── code/              source code
├── data/              input data (or a link / download script)
├── output/            optional: example figures or results
└── requirements.txt   or environment.yml / Project.toml / renv.lock
```

---

## How to use a model

1. Browse the `models/` folder and open the model's own `README.md`.
2. Download the repository (green **Code** button → **Download ZIP**) or clone it:
   ```bash
   git clone https://github.com/eaxesforum/Macro-Modelling.git
   ```
3. Install the dependencies listed in the model folder.
4. Follow the run instructions in the model's `README.md`.

---

## How to contribute

We welcome contributions from researchers, PhD students, central-bank and policy economists, and practitioners.

In short: **fork the repository → add your model in its own folder → open a pull request.** A member of the E-axes Forum team will review it before it is merged.

Please read **[CONTRIBUTING.md](CONTRIBUTING.md)** for the full guidelines and the checklist.

Questions or ideas for new models? Open an [Issue](https://github.com/eaxesforum/Macro-Modelling/issues).

---

## Citing

If you use code from this repository, please cite **both** the original paper of the model you use **and** this repository. Click **"Cite this repository"** in the right-hand sidebar, or see [CITATION.cff](CITATION.cff).

---

## License

Unless stated otherwise in a model folder, code in this repository is released under the [MIT License](LICENSE). Individual contributors keep the copyright to their work. Data files may be subject to their original providers' terms; see each model's `README.md`.

---

## Disclaimer

Models are shared for research and educational purposes. Each contributor is responsible for the content of their model. Inclusion in this repository does not imply endorsement of the results by the E-axes Forum.

---

## Contact

**E-axes Forum** · [e-axes.org](https://e-axes.org) · info@e-axes.org
