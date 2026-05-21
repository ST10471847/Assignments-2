# PDAN8411 – Programming for Data Analytics 2
## Part 2: Classification and Model Improvement  

### Student Information
- **Name:** Simphiwe Busakwe  
- **Student Number:** ST10471847  
- **Module:** PDAN8411  
- **Assessment:** POE Part 2  

---

## Project Overview

This project focuses on building and evaluating a **machine learning classification model** to predict whether a tumour is **malignant (cancerous)** or **benign (non-cancerous)**.

The analysis follows a full data science workflow, including:
- Exploratory Data Analysis (EDA)
- Feature selection
- Model training
- Model evaluation

The goal is to develop a reliable model that can assist in **early detection of breast cancer**, which is critical in improving patient outcomes.

---

## Dataset

The dataset used is the **Breast Cancer Wisconsin (Diagnostic)** dataset, obtained from:

- Kaggle  
- UCI Machine Learning Repository  

### Dataset Characteristics:
- **569 observations**
- **30 numerical features**
- **Binary target variable (diagnosis)**
  - `0 = Benign`
  - `1 = Malignant`

The dataset is clean, well-structured, and widely used for classification problems.

---

## Approach

The following steps were followed in this analysis:

### 1. Exploratory Data Analysis (EDA)
- Checked dataset structure, missing values, and summary statistics
- Visualised:
  - Class distribution
  - Feature distributions (histograms)
  - Correlation heatmap
  - Boxplots (outliers and class-based comparison)

### 2. Feature Selection
- Used correlation analysis to identify important features
- Applied a threshold (> 0.5) to select relevant predictors
- Removed redundant features to improve model performance

### 3. Model Training
- Split data into training and testing sets (80/20 split)
- Trained a **Random Forest classifier**
- Ensured reproducibility using a fixed random state

### 4. Model Evaluation
The model was evaluated using multiple metrics:
- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix

---

## Results

- **Accuracy:** 95.6%
- The model successfully classified the majority of cases
- Strong performance in detecting malignant cases
- Only a small number of misclassifications were observed

---

## Key Findings

- Tumour size-related features (e.g. `area_mean`, `radius_mean`) are strong predictors
- Malignant tumours tend to have higher values and greater variability
- The model demonstrates high reliability for classification tasks

---

## 🔧 Model Improvement

Although the model performs well, further improvements could include:
- Hyperparameter tuning (e.g. GridSearchCV)
- Cross-validation
- Comparing additional algorithms (e.g. Logistic Regression, SVM)

---

## Files Included

- `PDAN8411 Assignment 2.ipynb` → Jupyter Notebook (code + analysis)  
- `Simphiwe Busakwe PDA8411 part 2.pdf` → Final report  

---

## How to Run

1. Open the `.ipynb` file in **Jupyter Notebook or Google Colab**
2. Use your Kaggle.json file and
3. Run all cells sequentially
4. All visualisations and results will be displayed

---

## References

- UCI Machine Learning Repository (1995) – Breast Cancer Dataset  
- Scikit-learn Documentation (2024)  
- Han et al. (2011) – Data Mining: Concepts and Techniques  

---

## Conclusion

The Random Forest model achieved strong predictive performance and demonstrated the ability to effectively distinguish between benign and malignant tumours. The results highlight the importance of machine learning in supporting medical diagnosis and decision-making.

---

**Status:** Completed and submitted  
