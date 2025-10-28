# CMSE 492 Project — Breast Cancer Classification

**Author:** Ishan Baweja  
**Course:** CMSE 492 — Machine Learning Project  

This project explores supervised learning approaches for classifying breast tumors as benign or malignant using the Breast Cancer Wisconsin (Diagnostic) dataset. The goal is to compare three model families — Logistic Regression (linear), Random Forest (ensemble), and Support Vector Machine (polynomial kernel) — to evaluate trade-offs between interpretability, accuracy, and robustness. The project includes exploratory data analysis (EDA), baseline modeling, and a final comparative evaluation.

## Repository Structure
cmse492_project/
├── README.md  
├── .gitignore  
├── requirements.txt  
├── data/  
│   ├── raw/  
│   └── processed/  
├── notebooks/  
│   └── exploratory/  
├── src/  
│   ├── preprocessing/  
│   ├── models/  
│   └── evaluation/  
├── figures/  
├── docs/  
└── reports/

## Setup Instructions
1. Clone this repository: git clone https://github.com/<your-username>/cmse492_project.git  
2. Navigate into the folder: cd cmse492_project  
3. Create and activate a Python environment (Python ≥ 3.10)  
   - Mac/Linux: python -m venv venv && source venv/bin/activate  
   - Windows: python -m venv venv && venv\Scripts\activate  
4. Install dependencies: pip install -r requirements.txt  
5. Launch Jupyter Notebook: jupyter notebook  
   - Open notebooks in notebooks/exploratory/ to begin exploratory data analysis (EDA) and baseline modeling.

## Project Description
Breast cancer remains one of the most prevalent and life-threatening cancers worldwide, and early detection is crucial for improving patient outcomes. This project applies supervised machine learning methods to automate tumor classification using numerical features derived from digitized images of fine-needle aspirates. Each model family represents a different learning paradigm: Logistic Regression provides interpretability through feature coefficients, Random Forest captures nonlinear feature interactions, and SVM (Polynomial Kernel) models complex, high-dimensional boundaries. The evaluation focuses on ROC–AUC, F1-score, and accuracy to determine which approach offers the best balance between performance and interpretability. Results will be documented in Jupyter notebooks and a formal LaTeX report.
