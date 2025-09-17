# Rice-Variety-Classification

Jupyter notebook: **`rice-classification.ipynb`**  
Goal: Classify rice varieties using tabular and/or image-derived features. Baselines: KNN, SVM, Random Forest, Decision Tree.

## Overview
- **Part I (Tabular):** Train ML models on features from `data/part_i.csv`.
- **Part II (Images):** Extract texture/shape features from images (e.g., Haralick with `mahotas`, `skimage.feature`) and train classic ML models.
- **Metrics:** accuracy, precision, recall, F1, confusion matrix (optionally ROC/AUC).

## Data
- **Tabular:** `data/part_i.csv` (columns = handcrafted features).  
- **Images:** `data/images/<ClassName>/*.png|jpg` (e.g., `Arborio/`, `Basmati/`, `Jasmine/`).  

## Setup
```bash
# Python 3.9+ recommended
python -m venv .venv
# Windows: .venv\Scripts\activate
source .venv/bin/activate
pip install -U pip
pip install numpy pandas scikit-learn scikit-image mahotas opencv-python matplotlib seaborn scipy jupyterlab
