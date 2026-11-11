# Breast Cancer Detection — Machine Learning Project

A complete machine learning workflow for predicting breast cancer malignancy from cell characteristics, implemented in Python with the standard data science stack.

![Python](https://img.shields.io/badge/Python-3.x-3776AB?logo=python&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-ML-F7931E?logo=scikitlearn&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?logo=jupyter&logoColor=white)

---

## 📋 Table of Contents

- [Project Overview](#-project-overview)
- [Dataset Description](#-dataset-description)
- [Project Workflow](#️-project-workflow)
- [Repository Structure](#-repository-structure)
- [Getting Started \& Installation](#-getting-started--installation)
- [Model Performance](#-model-performance)
- [License](#-license)

---

## 🔍 Project Overview

Early and accurate detection of breast cancer is crucial for effective treatment and improving patient survival rates. This project applies machine learning to classify cell samples as **Benign** or **Malignant** based on cytological features extracted from breast mass fine needle aspirations (FNA).

---

## 📊 Dataset Description

The project uses `breast_cancer.csv`, containing **683 samples** and **11 attributes** after cleaning missing values.

| # | Attribute | Description | Range |
| --- | --- | --- | --- |
| 1 | Sample Code Number | Patient identifier code | — |
| 2 | Clump Thickness | Consistency of cell clump formations | 1–10 |
| 3 | Uniformity of Cell Size | Evaluation of cell size uniformity | 1–10 |
| 4 | Uniformity of Cell Shape | Evaluation of cell shape uniformity | 1–10 |
| 5 | Marginal Adhesion | Measure of cell adhesion properties | 1–10 |
| 6 | Single Epithelial Cell Size | Size of epithelial cells | 1–10 |
| 7 | Bare Nuclei | Assessment of nuclei lacking cytoplasm | 1–10 |
| 8 | Bland Chromatin | Texture and uniformity of nuclear chromatin | 1–10 |
| 9 | Normal Nucleoli | Presence and size of nucleoli | 1–10 |
| 10 | Mitoses | Frequency of cell division | 1–10 |
| 11 | **Class** | Target variable — diagnosis | `2` / `4` |

### Target variable

| Class | Label | Instances |
| --- | --- | --- |
| `2` | Benign (non-cancerous) | 444 |
| `4` | Malignant (cancerous) | 239 |

---

## ⚙️ Project Workflow

**1. Data Preprocessing & Loading**

- Loaded the dataset with `pandas`.
- Checked for missing values, data types and class balance.
- Separated features (`X`) from the target variable (`y`).

**2. Train–Test Split**

- Split the dataset into training and testing subsets to evaluate performance on unseen data reliably.

**3. Feature Scaling**

- Applied feature scaling to normalize input dimensions for optimal model convergence.

**4. Model Training & Evaluation**

- Trained a classification model on the scaled training data.
- Evaluated performance using key classification metrics such as accuracy score and the confusion matrix.

---

## 📁 Repository Structure

```text
Machine-Learning-Projects/
│
├── Breast_Cancer_Detection.ipynb   # Jupyter Notebook with the complete code and analysis
├── breast_cancer.csv               # Dataset used for training and testing
└── README.md                       # Project documentation

🚀 Getting Started & Installation
Prerequisites
Make sure Python is installed, then install the required data science libraries:
Copy
pip install numpy pandas scikit-learn matplotlib seaborn jupyter

Running the Notebook
Clone the repository or download the files.

Launch Jupyter Notebook:
Copy
jupyter notebook
Open Breast_Cancer_Detection.ipynb and run all cells sequentially to reproduce the results.
