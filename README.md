# Pan-STARRS Quasar Clustering Analysis

This repository contains the computational analysis pipeline developed for studying the clustering properties of high-redshift quasars using Pan-STARRS1 (PS1) survey data.

The project focuses on measuring the redshift-space two-point correlation function (2PCF) of sparse quasar populations at high redshift and constraining their clustering strength through statistical modelling and MCMC fitting.

---

# Scientific Motivation

Quasar clustering provides insight into:

- Large-scale structure formation
- Dark matter halo occupation
- Growth of supermassive black holes
- Evolution of massive structures in the early Universe

At high redshift, quasar populations become sparse, making clustering measurements statistically challenging. This project investigates these effects using observational survey data and simulated random catalogues.

---

# Main Features

This repository includes workflows for:

- Two-point correlation function estimation
- Random catalogue generation
- Survey footprint analysis
- Redshift-space clustering measurements
- Incompleteness analysis
- Halo mass and duty cycle studies
- MCMC fitting of clustering parameters
- Lightcone-based analysis

---

# Datasets Used

The analysis involves data from:

- Pan-STARRS1 (PS1)
- SDSS DR5 quasar sample
- Simulated cosmological lightcones

---

# Methodology

The clustering analysis follows the standard redshift-space two-point correlation framework.

Key steps include:

1. Construction of survey footprints using HEALPix
2. Generation of random catalogues within observational masks
3. Assignment of redshifts from smoothed observational distributions
4. Pair counting using Corrfunc
5. Estimation of ξ(s) using correlation estimators
6. MCMC fitting of power-law clustering models

The clustering model used is:

\[
\xi(s) = \left( \frac{s}{s_0} \right)^{-\delta}
\]

where:
- \( s_0 \) is the correlation length
- \( \delta \) is the clustering slope

---

# Validation

The pipeline was validated by reproducing the clustering results from:

- Shen et al. (2007)

using SDSS DR5 quasar samples.

The reproduced clustering measurements showed good agreement with published results. :contentReference[oaicite:0]{index=0}

---

# Repository Structure

```text
Codes/                      Core clustering and analysis scripts
Plots/                      Figures and visualization outputs
Notes/                      Analysis notes and references
PhdProjects/Complicor/      Additional clustering and incompleteness workflows

*.ipynb                     Interactive Jupyter notebooks
*.py                        Python analysis scripts
```

---

# Tools and Libraries

This project primarily uses:

- Python
- NumPy
- SciPy
- Matplotlib
- Astropy
- emcee
- Corrfunc
- HEALPix
- Jupyter Notebook

---

# Selected Results

Key results include:

- Measurement of PS1 quasar redshift-space clustering
- Constraints on clustering correlation length \( s_0 \)
- MCMC posterior estimation of clustering parameters
- Comparison with lower-redshift quasar clustering studies
- Analysis of incompleteness effects in sparse quasar samples

The analysis demonstrates the challenges of clustering measurements in small high-redshift quasar samples while remaining broadly consistent with increasing clustering trends at earlier cosmic epochs. :contentReference[oaicite:1]{index=1}

---

# Current Status

This repository is an active computational astrophysics research workspace containing analysis tools, notebooks, and supporting materials related to high-redshift quasar clustering studies.

---

# Author

Vibin Ram Narayanan

Research interests:
- Computational astrophysics
- Large-scale structure
- Quasar clustering
- Scientific computing
- Cosmological simulations
- Data-intensive astronomy
