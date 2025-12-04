# CMSE 492 Project — Breast Cancer Subtype Classification

**Author:** Ishan Baweja  
**Course:** CMSE 492 — Machine Learning Project

This project builds an end-to-end machine learning workflow for classifying breast cancer tumors into PAM50 and Claudin-low subtypes using the METABRIC dataset. The workflow includes preprocessing, exploratory data analysis (EDA), PCA-based dimensionality reduction, model development, hyperparameter tuning, evaluation, and interpretation using Random Forest importance and SHAP values.

## Repository Structure
cmse492_project/  
│── README.md  
│── requirements.txt  
│── .gitignore  
│  
├── data/  
│   ├── raw/  
│   └── processed/  
│  
├── notebooks/  
│   └── exploratory/  
│  
├── src/  
│   ├── preprocessing/  
│   ├── models/  
│   └── evaluation/  
│  
├── figures/  
├── docs/  
└── reports/  

## Setup Instructions
1. Clone the repository:  
   `git clone https://github.com/Ishan-Baweja/cmse492_project.git`
2. Navigate into the folder:  
   `cd cmse492_project`
3. Create and activate a Python environment (Python ≥ 3.10):  
   - Mac/Linux:  
     `python -m venv venv && source venv/bin/activate`  
   - Windows:  
     `python -m venv venv && venv\Scripts\activate`
4. Install dependencies:  
   `pip install -r requirements.txt`
5. Launch Jupyter Notebook:  
   `jupyter notebook`  
   (Open notebooks in `notebooks/exploratory/` for EDA and baseline modeling.)

## Project Description
Breast cancer includes several clinically meaningful subtypes. This project uses supervised machine learning to classify tumors using genomic and clinical features from the METABRIC dataset. Preprocessing includes missing-value handling, encoding, variance filtering, scaling, and PCA (50 components).

Three models were evaluated:
- Logistic Regression  
- Random Forest  
- Support Vector Machine  

Logistic Regression performed best overall, achieving an accuracy of 0.729 and an AUC of 0.917. Random Forest captured nonlinear relationships, while SVM performance was more sensitive to class imbalance. Evaluation metrics included accuracy, weighted precision, weighted recall, weighted F1-score, and weighted AUC.

Interpretability methods such as PCA loadings, Random Forest feature importance, and SHAP summary plots were used to understand how features contributed to subtype prediction.

The final written report is compiled in LaTeX and included in the `reports/` directory.
