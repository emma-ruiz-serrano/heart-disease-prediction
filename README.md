# Heart Disease Prediction

**Author:** Emma Ruiz Serrano  
**Date:** November 2024  

Predicting heart disease risk using machine learning algorithms, including **Neural Networks, Random Forest, KNN, XGBoost, and Logistic Regression**. The project includes data preprocessing, feature selection, model evaluation, and analysis of clinical and lifestyle factors.  

---

## Table of Contents

1. [Project Overview](#project-overview)  
2. [Dataset](#dataset)  
3. [Methodology](#methodology)  
4. [Machine Learning Models](#machine-learning-models)  
5. [Evaluation Metrics](#evaluation-metrics)  
6. [Results](#results)  
7. [How to Run the Code](#how-to-run-the-code)  
8. [References](#references)  

---

## Project Overview

Heart disease is one of the leading causes of death worldwide. Early prediction is critical for prevention and intervention. This project develops predictive models for heart disease by combining clinical, demographic, and lifestyle features, aiming to identify individuals at high risk and highlight the most relevant risk factors.  

---

## Dataset

The dataset comes from the **Behavioral Risk Factor Surveillance System (BRFSS), 2021**, provided by the World Health Organization (WHO).  

- **Number of samples:** 308,854  
- **Features:** 19, including health history, demographics, and lifestyle factors (e.g., smoking, diet, physical activity)  
- **Target variable:** Heart Disease (Yes/No)  

**Files included:**  
- `heart_disease_data.csv` – raw dataset  
- `heart_disease_prediction.py` – Python script with all preprocessing, model training, and evaluation  
- `paper_heart_disease_prediction.pdf` – detailed documentation of the project  

---

## Methodology

1. **Data preprocessing**  
   - Handling categorical and ordinal variables  
   - Dummy encoding for binary features  
   - Numerical encoding for age and other ordinal variables  
   - Balancing the dataset to address class imbalance  

2. **Feature selection**  
   - Correlation analysis  
   - Ridge and Lasso regression to select relevant variables  

3. **Cross-validation**  
   - 5-fold and 10-fold cross-validation depending on the model  
   - Ensures robustness and prevents overfitting  

4. **Hyperparameter tuning**  
   - Grid search to optimize model parameters  
   - Adjusted classification thresholds to prioritize sensitivity for heart disease detection  

---

## Machine Learning Models

- **Logistic Regression**  
- **Random Forest**  
- **K-Nearest Neighbors (KNN)**  
- **XGBoost**  
- **Support Vector Machines (SVM)**  
- **Neural Networks** (implemented with TensorFlow/Keras)  

---

## Evaluation Metrics

- **Accuracy** – overall correctness  
- **Sensitivity (Recall)** – correctly identifying heart disease cases  
- **Specificity (Precision)** – correctly identifying non-disease cases  
- **ROC Curve & AUC** – overall model performance  

---

## Results

- **Neural Network**: Sensitivity 82%, Specificity 71%, Accuracy 72%  
- Other models like Logistic Regression and Random Forest performed well in terms of specificity but had lower sensitivity.  

> The Neural Network was selected as the most suitable model for identifying heart disease risk, prioritizing early detection and minimizing false negatives.  

---

## How to Run the Code

1. Clone the repository:  
```bash
git clone https://github.com/emma-ruiz-serrano/heart-disease-prediction.git
