# Rice Variety Classification

The project focuses on classifying rice varieties using **two datasets**:

- **Part I (`part_i.csv`)** → Tabular dataset with 106 numerical features per sample.  
- **Part II (`part_ii`)** → Image dataset of rice grains, requiring feature extraction for classification.

The notebook: **`rice-classification.ipynb`**

---

## Project Overview
The goal is to understand and apply fundamental machine learning concepts using **scikit-learn**.  
We implement multiple algorithms and evaluate them on both tabular and image-based rice classification tasks.

- **Algorithms used:**  
  - k-Nearest Neighbor (kNN, weighted-kNN)  
  - Naive Bayes  
  - Random Forest  
  - Support Vector Machine (SVM)  

- **Evaluation metrics:**  
  - Accuracy  
  - Precision  
  - Recall  
  - F1-score  
  - Confusion Matrix  

- **Validation:**  
  - 80/20 Train-Test split  
  - k-Fold Cross Validation (k=5):contentReference[oaicite:0]{index=0}

---

## Part I: Textual Data Analysis
- Input: `part_i.csv` (106 features + class labels).  
- Tasks:  
  - Preprocessing (cleaning, scaling if necessary).  
  - Model training with kNN, Naive Bayes, Random Forest, SVM.  
  - Comparison of performance with different preprocessing choices (raw vs. scaled, etc.).

---

## Part II: Image Data Analysis
- Input: `part_ii/` (rice grain images).  
- Feature Extraction:  
  - RGB values.  
  - Thresholded binary representations.  
  - Additional methods (texture, shape features).  
- Models: Same as Part I (kNN, Naive Bayes, Random Forest, SVM).  
- Evaluation with both raw and extracted features:contentReference[oaicite:1]{index=1}.

---

## Installation
```bash
# Python 3.9+ recommended
python -m venv .venv
# Windows: .venv\Scripts\activate
source .venv/bin/activate
pip install -U pip
pip install -r requirements.txt
