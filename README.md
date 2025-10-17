# Wine Quality Classification — From-Scratch LR & SVM (with Kernels)

This repository contains a reproducible project to classify wine quality (binary) using **logistic regression** and **support vector machines**, including **kernel** variants. Models are implemented **from scratch** (no scikit-learn estimators for training), with a leakage-safe workflow (train-only transforms, stratified splits, and cross-validation for model selection).

## Contents
- `Wine_Classification.ipynb` — End-to-end notebook (EDA → preprocessing → training → evaluation).
- `Wine_Classification.pdf` — Report export of the notebook (optional).
- `data/` — Raw data and/or extracted files from the provided archive.
- `.gitignore` — Standard ignores for Python + notebooks.

## Quickstart
1. Create and activate a Python environment (e.g., `python -m venv .venv && source .venv/bin/activate` on macOS).
2. Install dependencies you used for the notebook (e.g., `numpy`, `pandas`, `matplotlib`, etc.).
3. Open the notebook: `jupyter lab` or `code Wine_Classification.ipynb` (VS Code).
4. Run all cells. Ensure any file paths in the notebook point to `data/`.

## Reproducibility Notes
- All preprocessing should be **fit on training data only** (and within each CV fold).
- Use **stratified train/test split**.
- Tune hyperparameters via **cross-validation** and hold out the test set for a single final evaluation.

---

Extracted dataset archive into data/.
