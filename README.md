# German Credit Risk Analysis Project

This project was completed as part of the **BLM4800 - Introduction to Data Mining** course at Yıldız Technical University, Department of Computer Engineering. It involves a comprehensive **credit risk analysis** using the **German Credit Dataset**, applying **classification and clustering techniques** from machine learning to evaluate customer creditworthiness.


## Project Summary

The main goal of this project is to analyze and model **credit risk** in the financial sector by leveraging machine learning algorithms. The dataset contains 1000 credit applications with 20 features (7 numerical, 13 categorical) and a binary target variable indicating whether the applicant is a **good (0)** or **bad (1)** credit risk.

Key tasks performed:
- Exploratory Data Analysis (EDA)
- Feature preprocessing and encoding
- Classification modeling using cost-sensitive evaluation
- Clustering for customer segmentation
- Evaluation and comparison of models/clusters


##  Contents

| File | Description |
|------|-------------|
| `german_credit_analysis.ipynb` | Main Jupyter notebook containing all data analysis, modeling, and visualization steps |
| `README.md` | This file – project overview and instructions |
| `requirements.txt` | List of Python packages required to run the notebook |


## Requirements & Setup

### Install Dependencies

Make sure you have Python installed. Then install the necessary packages via:

pip install -r requirements.txt

## Dataset
The original dataset (german.data) is not included in this repository but can be found in the link here: https://archive.ics.uci.edu/dataset/144/statlog+german+credit+data .

Place it in the root directory under the name german.data.

## Key Features of the Project
**Classification Models:**
- Logistic Regression
- Decision Tree
- Random Forest

**Evaluation Metrics:**
- Accuracy
- Precision
- Recall (Sensitivity)
- F1-Score
- ROC AUC
- Custom Cost Function (where FP=1, FN=5)

**Clustering Algorithms:**
- K-Means Clustering
- Agglomerative Hierarchical Clustering
- DBSCAN
  
## Highlights
**K-Means Clustering (k=4)** successfully identified distinct customer segments, including:
   - Low-risk customers (older, low loan amounts, stable employment)
   - High-risk customers (long-term loans, high credit amounts)
     
**Random Forest** achieved the best overall performance in classification metrics, while Logistic Regression yielded the lowest custom cost.

**DBSCAN** struggled with parameter tuning and produced many noise points, suggesting the need for further optimization.
