# FusPB-ESM2

Code and datasets for **FusPB-ESM2: Fusion model of ProtBERT and ESM-2 for cell-penetrating peptide prediction**.

## Paper

- Title: FusPB-ESM2: Fusion model of ProtBERT and ESM-2 for cell-penetrating peptide prediction
- Authors: Fan Zhang, Jinfeng Li, Zhenguo Wen, Chun Fang
- Journal: Computational Biology and Chemistry, 111, 108098, 2024
- DOI: https://doi.org/10.1016/j.compbiolchem.2024.108098
- PubMed: https://pubmed.ncbi.nlm.nih.gov/38820799/

## Overview

FusPB-ESM2 predicts cell-penetrating peptides (CPPs) by extracting sequence representations from protein language models, including ProtBERT and ESM-2, then fusing the learned features for classification.

## Repository Contents

- `data/trainCPP.csv`: training dataset.
- `data/testCPP.csv`: independent test dataset.
- `notebooks/Five_fold_esm.ipynb`: 5-fold validation for ESM-2 variants.
- `notebooks/Five_fold_protbert.ipynb`: 5-fold validation for ProtBERT variants.
- `notebooks/Five_fold_fusion.ipynb`: 5-fold validation for fused ProtBERT and ESM-2 features.
- `notebooks/Five_fold_d_mapping.ipynb`: 5-fold validation for dimensional mapping experiments.
- `notebooks/Independent_testing.ipynb`: independent test workflow.
- `environment.yml`: conda environment specification.

## Installation

Create the conda environment:

```bash
conda env create -f environment.yml
conda activate my_environment3
```

The notebooks use pretrained protein language models. Download or configure the corresponding ProtBERT and ESM-2 checkpoints before running the notebooks.

## Usage

Start Jupyter from the repository root:

```bash
jupyter notebook
```

Open the notebooks in `notebooks/` and run the cells. Dataset paths in the notebooks point to `../data/trainCPP.csv` and `../data/testCPP.csv`.

## Notes

Large pretrained model weights and runtime outputs are intentionally not committed to this repository.
