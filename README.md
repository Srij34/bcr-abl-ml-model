# Chemoinformatic and Machine Learning Approach for BCR-ABL Kinase Inhibitor Discovery

This repository contains the research thesis titled **"Chemoinformatic Analysis and Machine Learning Model Development using BCR-ABL Kinase Structurally Diverse Inhibitors for Cancer Therapeutics"**. The study integrates ligand-based machine learning models with chemoinformatics and molecular docking to identify promising BCR-ABL kinase inhibitors—a key target in treating Chronic Myeloid Leukemia (CML).

---

## 🧬 Project Overview

BCR-ABL is a fusion gene resulting from a chromosomal abnormality that plays a major role in CML. This study:
- Extracts and preprocesses a dataset of 1649 compounds from the ChEMBL database.
- Uses 12 types of molecular fingerprints generated via **PaDEL-Descriptor**.
- Builds and evaluates ML-QSAR models using **Random Forest** and **Weka 3.8.5**.
- Identifies top lead compounds via **virtual screening** and **molecular docking**.
- Evaluates ADME/T properties using **Schrödinger's QikProp**.

---

## 📁 Repository Structure

```
bcr-abl-ml-model/
├── thesis/
│   └── Chemoinformatic_Analysis_BCR_ABL.pdf
├── models/
├── data/
├── figures/
├── LICENSE
└── README.md
```

---

## 📌 Key Highlights

- **Dataset:** 1649 BCR-ABL inhibitors with IC50 values
- **Feature Extraction:** 12 fingerprint types including Substructure, MACCS, E-state, PubChem, AtomPairs 2D
- **Best Model:** Substructure Count Fingerprint + Random Forest
  - Training Accuracy: **1.0**
  - Testing Accuracy: **97.14%**
  - AUC (ROC): **1.0**
- **Lead Compounds Identified:**
  - `F6548-0900` (Docking score: **-10.924 kcal/mol**)
  - `F3216-1016`
  - `F0882-0174`
- **Validation:** ADME analysis confirms drug-likeness properties

---

## 🔬 Tools & Technologies

- **Chemoinformatics:**
  - PaDEL-Descriptor
  - SMILES & molecular descriptors
- **Machine Learning:**
  - Random Forest (WEKA & Python/sklearn)
  - Feature Selection via PCA and Variance Threshold
- **Visualization:**
  - Seaborn & Matplotlib for EDA and ROC curves
- **Molecular Modeling:**
  - Schrödinger Suite: Glide (Docking), QikProp (ADME), LigPrep, Protein Prep Wizard
- **Data Source:**
  - [ChEMBL Database](https://www.ebi.ac.uk/chembl/)

---

## 📄 Full Thesis

📘 [`thesis/Chemoinformatic_Analysis_BCR_ABL.pdf`](./thesis/Chemoinformatic_Analysis_BCR_ABL.pdf)

---

## 🚀 Future Work

- Expand dataset to include more kinase targets
- Compare with deep learning models (e.g., Graph Neural Networks)
- In-vitro or in-vivo validation of top candidates

---


## 🙌 Acknowledgements

- **ChEMBL Database** for compound and activity data
- **Schrödinger Inc.** for computational tools
- **Open-source libraries** like scikit-learn, seaborn, matplotlib
- Faculty and peers who provided feedback and mentorship

---
