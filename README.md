# Breast Cancer Classification using Machine Learning

## Quick Overview

- Built an end-to-end machine learning system for breast cancer classification  
- Dataset: Wisconsin Breast Cancer Diagnostic (UCI / Kaggle)  
- Models: Logistic Regression, Random Forest, SVM, XGBoost  
- Best Model: Random Forest Classifier  
- Performance: 97.4% accuracy, 93.0% recall, ROC-AUC > 0.99  
- Focus Areas: Model interpretability (SHAP), clinical relevance, responsible AI  

## Project Summary

This project presents a comprehensive end-to-end machine learning system for classifying breast tumors as benign or malignant using clinical features extracted from Fine Needle Aspiration (FNA) images.

The work focuses on achieving high predictive performance while maintaining model transparency, clinical relevance, and responsible use of artificial intelligence. The system is designed as a medical decision-support tool rather than a replacement for professional diagnosis.

## Project Objective

The main objectives of this project are:

- To develop an accurate binary classification model for breast cancer detection  
- To prioritize high recall (sensitivity) in order to minimize missed malignant cases  
- To provide interpretable predictions that can support clinical decision-making  

## Dataset Information

- Dataset: Wisconsin Breast Cancer Diagnostic Dataset  
- Source: UCI Machine Learning Repository / Kaggle  
- Dataset Link: https://www.kaggle.com/datasets/uciml/breast-cancer-wisconsin-data  
- Total Samples: 569  
- Number of Features: 30 real-valued cell nucleus measurements  

### Target Variable

- 0 – Benign  
- 1 – Malignant  

The dataset is clean, well-structured, and widely used in academic and medical machine learning research.

## Methodology Overview

### Exploratory Data Analysis

- Analysis of class distribution  
- Statistical summary of features  
- Correlation analysis to identify multicollinearity  
- Outlier detection using the IQR method  
- Statistical significance testing using independent t-tests  

### Data Preprocessing

- Encoding of the target variable  
- Feature scaling using StandardScaler  
- Stratified 80/20 train–test split  
- Reproducibility ensured using fixed random states  

### Feature Engineering and Selection

- Feature importance analysis using Random Forest  
- Recursive Feature Elimination (RFE)  
- Principal Component Analysis (PCA) to study variance retention  
- Final feature selection prioritizing interpretability for medical use  

### Model Development

The following machine learning models were trained and evaluated:

- Logistic Regression  
- Random Forest Classifier  
- Support Vector Machine (SVM)  
- XGBoost Classifier  

All models were evaluated using cross-validation and medical-relevant performance metrics.

## Model Performance

The final selected model achieved the following results:

- Accuracy: 97.4%  
- Recall (Sensitivity): 93.0%  
- Precision: 97.6%  
- F1-Score: 95.2%  
- ROC-AUC: Greater than 0.99  

The Random Forest Classifier was selected as the final model due to its strong balance of performance, robustness, interpretability, and compatibility with explainable AI techniques.

## Model Explainability

To ensure transparency and trust, SHAP (SHapley Additive exPlanations) was used to interpret model predictions.

- Global explanations identify the most influential features across the dataset  
- Local explanations provide insight into individual patient predictions  
- Key features related to nuclear size and irregularity were identified as strong indicators of malignancy  

This approach allows clinicians to understand why a prediction was made, not just the predicted outcome.

## Clinical Relevance

- High recall reduces the risk of missing malignant cases  
- Low false-positive rates help minimize unnecessary biopsies  
- Model behavior aligns with established pathological knowledge  
- Suitable for use as a screening or diagnostic support system  

This system is intended to assist healthcare professionals and should not replace clinical examination or biopsy confirmation.

## Tools and Technologies

- Programming Language: Python  
- Libraries: Pandas, NumPy, Scikit-learn, XGBoost, SHAP  
- Visualization: Matplotlib, Seaborn  
- Development Environment: Jupyter Notebook  

## Key Learning Outcomes

- Developed a complete machine learning pipeline from data exploration to model interpretation  
- Applied evaluation strategies appropriate for medical datasets  
- Implemented explainable AI techniques for transparency and trust  
- Gained practical experience in responsible machine learning for healthcare  

## Author

Noorul Hasiba  
Computer Science and Data Science Student  
Albukhary International University  

