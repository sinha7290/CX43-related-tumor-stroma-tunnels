# CX43

**Companion code for our JCI 2024 paper on how breast cancers that disseminate to bone marrow acquire aggressive phenotypes through CX43-related tumor-stroma tunnels.**

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Publication](https://img.shields.io/badge/Published-JCI%202024-blue)](https://doi.org/10.1172/JCI170953)
[![PMID](https://img.shields.io/badge/PMID-39480488-lightgrey)](https://pubmed.ncbi.nlm.nih.gov/39480488/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter)](https://jupyter.org/)

## Overview

This repository contains the code and derived analyses underlying our study of how **estrogen receptor positive (ER+) breast cancer** cells that disseminate to bone marrow acquire aggressive phenotypes through direct contact with **mesenchymal stromal cells (MSCs)**, mediated by **Connexin 43 (CX43, encoded by *GJA1*) tumor-stroma tunnels**.

We modeled these interactions using tumor MSC co-cultures and applied an **integrated transcriptome, proteome, and network analyses workflow** to build a comprehensive catalog of contact-induced changes. Key findings include:

* Conditioned media from MSCs failed to recapitulate the genes and proteins induced in cancer cells by direct contact, implicating physical intercellular connections rather than soluble factors
* Contact-induced changes fell into two functionally distinct classes: **"borrowed"** components acquired from MSCs and **"intrinsic"** components upregulated in the tumor cells themselves
* Protein protein interaction networks revealed a rich connectome linking borrowed and intrinsic programs
* CX43-related tumor-stroma tunnels emerged as the mechanistic anchor for phenotype acquisition
* The composite CX43 associated signature stratifies patient outcomes and tracks disease aggressiveness in independent ER+ breast cancer cohorts

## Repository contents

| File | Purpose |
| :--- | :--- |
| `composite_ROC_AUC.ipynb` | Composite ROC and AUC analyses evaluating the CX43 signature as a classifier of disease state and outcome |
| `heatmaps.ipynb` | Publication heatmaps of borrowed vs intrinsic transcriptomic and proteomic programs |
| `km plots.ipynb` | Kaplan Meier survival analyses stratified by CX43 signature scores in independent patient cohorts |

## Reproducing the analysis

1. Clone the repository and install dependencies (Python 3.9+, standard scientific stack, plus `lifelines` for survival analyses and `scikit-learn` for ROC/AUC).
2. Download the primary datasets from the accessions listed below.
3. Run the notebooks in the following order:
   1. `heatmaps.ipynb` to reproduce the transcriptomic and proteomic figure panels.
   2. `composite_ROC_AUC.ipynb` to compute composite signature performance metrics.
   3. `km plots.ipynb` to reproduce the survival analyses in external patient cohorts.

## Data availability

Primary datasets generated in the study are deposited in public repositories:

* **Transcriptomics:** NCBI Gene Expression Omnibus, accession **GSE224322**
* **Proteomics:** ProteomeXchange, identifier **PXD039860**

Full data availability details and supporting data values are provided in the manuscript and supplementary materials.

## Publication

> Sinha S, Callow BW, Farfel AP, Roy S, Chen S, Masotti M, Rajendran S, Buschhaus JM, Espinoza CR, Luker KE, Ghosh P, Luker GD.
> **Breast cancers that disseminate to bone marrow acquire aggressive phenotypes through CX43-related tumor-stroma tunnels.**
> *Journal of Clinical Investigation*, 2024 Oct 31; 134(24): e170953.
> doi: [10.1172/JCI170953](https://doi.org/10.1172/JCI170953)
> PMID: 39480488 · PMCID: PMC11645149

If you use this code, the CX43 signature, or derived analyses in your own work, please cite the manuscript.

## Contact

**Saptarshi Sinha, Ph.D.**
Assistant Project Scientist, Department of Cellular and Molecular Medicine
Director, PreCSN Center
University of California San Diego
Email: sasinha@health.ucsd.edu

## License

Released under the MIT License. See `LICENSE`.
