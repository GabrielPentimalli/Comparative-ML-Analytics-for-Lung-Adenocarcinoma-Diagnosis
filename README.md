# 🧬 Comparative Machine Learning Analytics for Lung Adenocarcinoma Diagnosis

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/downloads/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

## 📖 Project Overview

This project applies advanced machine learning algorithms to metabolomic data analysis for lung adenocarcinoma identification. The main objective is to develop accurate predictive models that can distinguish between patients with lung adenocarcinoma and healthy subjects through serum and plasma metabolic profile analysis.

### 🎯 Main Objectives

- **Binary Classification**: Distinguish lung adenocarcinoma patients from healthy subjects
- **Biomarker Identification**: Identify significant metabolites for diagnosis
- **Algorithm Comparison**: Evaluate performance of different ML algorithms
- **Predictive Optimization**: Maximize diagnostic accuracy and sensitivity

## 📊 Dataset

**Source**: Metabolomics Workbench (Dataset ID: ST000339)  
**Type**: GC-MS data from serum and plasma  
**Dimensions**: 181 metabolites × 181 samples  
**Classes**: 
- 🔴 Adenocarcinoma: 100 samples
- 🟢 Healthy: 81 samples

**Key Identified Metabolites**:
- **Aspartic Acid** (serum)
- **Pyrophosphate** (plasma)

## 🤖 Implemented Algorithms

| Algorithm | Category |
|-----------|-----------|
| **Logistic Regression** | Linear |
| **Partial Least Squares** | Linear |
| **XGBoost** | Ensemble | 
| **AdaBoost** | Ensemble |
| **Gradient Boosting** | Ensemble |
| **Random Forest** | Ensemble | 
| **Support Vector Machine** | Kernel | 
| **Naïve Bayes** | Probabilistic |

## 🛠️ Technologies and Libraries

### Languages
- ![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)

### Main Libraries
```python
# Machine Learning
scikit-learn >= 1.0
xgboost >= 1.5

# Data Processing
pandas >= 1.3
numpy >= 1.21

# Visualization
matplotlib >= 3.5
seaborn >= 0.11

# Jupyter Environment
jupyter >= 1.0
```

## 📈 Analysis Pipeline

### 1. **Data Preprocessing**
- Data cleaning and typo correction
- Missing value handling with KNN Imputation
- Feature normalization and scaling

### 2. **Feature Selection**
- Chi-square test for most significant feature selection
- Relevant biomarker identification

### 3. **Model Training & Optimization**
- Dataset split (80% training, 20% test)
- Grid Search for hyperparameter optimization
- Cross-validation with KFold (k=5)

### 4. **Evaluation**
- Metrics: Accuracy, Precision, Recall, F1-Score, AUC-ROC
- Confusion matrices
- Comparative ROC curves

## 📊 Main Results

### Performance by Metric
| Metric | Best Algorithm | Value |
|--------|----------------|-------|
| **Accuracy** | Logistic Regression | 83% |
| **Precision** | Partial Least Squares | 87% |
| **Recall** | XGBoost | 90% |
| **F1-Score** | XGBoost | 86% |
| **AUC-ROC** | Logistic Regression | 82% |

### Identified Biomarkers
✅ **Aspartic Acid**: Present in all models  
✅ **Pyrophosphate**: Confirmed by feature selection  

## 🔬 Scientific Insights

### Metabolomics and Cancer
Metabolomics studies the complete set of metabolites present in an organism. In the context of lung cancer, metabolic profile analysis can reveal:

- **Metabolic Alterations**: Changes in cellular energy pathways
- **Diagnostic Biomarkers**: Specific molecules associated with tumor presence
- **Pathological Mechanisms**: Understanding of altered biological processes

### Clinical Relevance
- **Early Diagnosis**: Identification before symptomatic manifestation
- **LDCT Complement**: Reduction of false positives in screening
- **Personalized Medicine**: Individual metabolic profiles

## 📈 Limitations and Future Developments

### Current Limitations
- **Dataset Size**: Limited number of samples (181)
- **Validation**: Independent dataset validation required
- **Interpretability**: Biological validation of biomarkers needed

### Future Developments
- 🧠 **Deep Learning**: Implementation of artificial neural networks
- 📈 **Data Augmentation**: Techniques to increase dataset size
- 🔬 **Clinical Validation**: Studies on larger cohorts

## 📄 License

This project is distributed under the MIT License. See `LICENSE` for more information.

## 👨‍💻 Author

**Gabriel Pentimalli**
- 📧 Email: gab.pentimalli@stud.uniroma3.it
- 🎓 LinkedIn: [Gabriel Pentimalli](https://www.linkedin.com/in/gabriel-pentimalli-54180625a/)
- 🐙 GitHub: [@GabrielPentimalli](https://github.com/GabrielPentimalli)

---
