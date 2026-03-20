# Hierarchical Multi-Label Learning for sEMG-Based Gesture Recognition

---

## Overview

This repository contains training code for hierarchical multi-label classification of sEMG signals across 3 open-source benchmarks. Each dataset involves jointly recognizing **hand gestures** alongside a **secondary motion label** — which differs per dataset (arm posture, orientation, or position).

---

## Repository Structure
```text
meta learner for AT-EMG.ipynb      # Training pipeline for AT-EMG dataset
meta learner for fors-emg.ipynb    # Training pipeline for FORS-EMG dataset
meta learner for unibo semg.ipynb  # Training pipeline for UniBo-INAIL dataset
```

---

## Datasets

No pretrained weights needed. Download datasets directly and follow the data processing steps in each notebook.

- **AT-EMG**: [GitHub](https://github.com/MoveR-Digital-Health-and-Care-Hub/posture_dataset_collection)
- **FORS-EMG**: [Kaggle](https://www.kaggle.com/datasets/ummerummanchaity/fors-emg-a-novel-semg-dataset)
- **UniBo-INAIL sEMG**: [GitHub](https://github.com/pulp-bio/unibo-inail-semg-dataset)

---

## Running the Notebooks

All notebooks are designed to run on **Kaggle** (free GPU).

1. Download the dataset and upload to Kaggle as a dataset.
2. Open the corresponding notebook on Kaggle.
3. Update dataset paths if necessary.
4. Run all cells.

---

## Results

Achieved **20–35% accuracy improvement** using the combined feature set (SNTDF + Extended Hudgins) over the Hudgins-5 baseline with SVM/LDA across all 3 benchmarks.

---

## Acknowledgements

- [AT-EMG Dataset](https://github.com/MoveR-Digital-Health-and-Care-Hub/posture_dataset_collection)
- [FORS-EMG Dataset](https://www.kaggle.com/datasets/ummerummanchaity/fors-emg-a-novel-semg-dataset)
- [UniBo-INAIL sEMG Dataset](https://github.com/pulp-bio/unibo-inail-semg-dataset)
