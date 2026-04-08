# Neuroblastoma Machine Learning Analysis

This repository contains coursework completed as part of my MSc Bioinformatics programme, focusing on applying machine learning to RNA-seq data for clinical outcome prediction.

The project integrates transcriptomic and clinical data from a neuroblastoma cohort to predict high-risk disease status. Machine learning was used to model clinical outcomes from RNA-seq data, with a focus on robust validation and biological interpretation of predictive genes.
---

## Repository Structure

neuroblastoma-ml-analysis/
├── DataSet/ (input data; large files excluded)  
├── plots/ (PCA, ROC, feature importance, etc.)  
├── results/ (model predictions)  
└── neuroblastoma_analysis.ipynb  

---

## Methods

- Integration of RNA-seq expression and clinical metadata  
- Exploratory PCA (unsupervised, for visualisation only)  
- Variance-based feature selection applied on training data only  
- Supervised models: Logistic Regression, SVM, Random Forest (tuned)  
- Model evaluation using stratified 5-fold cross-validation and a held-out test set (ROC-AUC)  
- Feature importance analysis and prediction of high-risk status in unlabelled samples  

---

## Reproducibility

1. Clone the repository  
2. Open `neuroblastoma_analysis.ipynb`  
3. Install required Python packages  
4. Run all cells sequentially  

---

## Data

The dataset (GSE49711) is publicly available at:  
https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE49711  

This dataset contains RNA-seq expression profiles from 498 primary neuroblastoma tumours with associated clinical annotations.

---

## Notes

- PCA was used for exploratory analysis only and was not included in the modelling pipeline  
- Feature selection and preprocessing were performed using training data only to avoid data leakage  
- High test performance should be interpreted cautiously due to the relatively small test set size  
- Feature importance reflects association rather than causation  

---

## Tools and Packages

Python · pandas · NumPy · scikit-learn · matplotlib · seaborn  

---

## Author

Ammarah Kathawala  
MSc Bioinformatics
