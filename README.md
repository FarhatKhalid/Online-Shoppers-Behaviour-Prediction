# Predicting Online Shopper Behavior with Machine Learning
Implementation and enhancement of machine learning models for predicting online shoppers behaviour

## Overview

This project focuses on predicting online shoppers' purchasing intentions using machine learning techniques. The work is based on the research paper **"Comparative Analysis of Different Machine Learning Algorithms to Predict Online Shoppers' Behaviour"** and includes the implementation, evaluation, and comparison of multiple classification models on the Online Shoppers Purchasing Intention dataset.

In addition to reproducing the original study, an enhanced predictive framework was developed using the **CatBoost classifier** with hyperparameter optimization to improve model performance and provide deeper insights into customer purchasing behavior.

---
## Objectives

* Analyze online shopper behavior using real-world e-commerce data.
* Implement and compare multiple machine learning classification algorithms.
* Identify the most effective model for predicting purchase intention.
* Improve prediction performance using an advanced boosting algorithm.
* Discover the most influential factors affecting customer purchasing decisions.

---
## Dataset

**Dataset:** Online Shoppers Purchasing Intention Dataset

**Source:** UCI Machine Learning Repository

### Dataset Characteristics

* 12,330 user sessions
* 18 numerical and categorical attributes
* One year of website visitor activity
* Imbalanced dataset:

  * Approximately 85% non-purchasing sessions
  * Approximately 15% purchasing sessions

---

## Methodology

The project follows a structured machine learning workflow:

1. Data Collection
2. Data Preprocessing
3. Exploratory Data Analysis (EDA)
4. Feature Analysis
5. Model Training
6. Performance Evaluation
7. Hyperparameter Optimization
8. Comparative Analysis

---

## Machine Learning Models Implemented

The following algorithms were implemented and evaluated:

* Logistic Regression
* Support Vector Machine (SVM)
* Random Forest
* AdaBoost
* Gradient Boosting
* CatBoost (Proposed Enhancement)

---

## Performance Comparison

| Model               | Accuracy | Precision | Recall | F1-Score | ROC-AUC |
| ------------------- | -------- | --------- | ------ | -------- | ------- |
| Gradient Boosting   | 0.901    | 0.723     | 0.589  | 0.649    | 0.929   |
| Random Forest       | 0.901    | 0.751     | 0.537  | 0.626    | 0.923   |
| SVM                 | 0.888    | 0.690     | 0.500  | 0.580    | 0.859   |
| Logistic Regression | 0.881    | 0.743     | 0.356  | 0.481    | 0.887   |
| AdaBoost            | 0.880    | 0.604     | 0.647  | 0.625    | 0.898   |

---

## Proposed Enhancement: CatBoost

To further improve prediction quality, CatBoost was introduced and optimized using hyperparameter tuning.

### Optimal Parameters

* Learning Rate: 0.03
* Depth: 6
* L2 Leaf Regularization: 9
* Bagging Temperature: 0.5

### CatBoost Performance

| Metric    | Score |
| --------- | ----- |
| Accuracy  | 0.863 |
| Precision | 0.536 |
| Recall    | 0.832 |
| F1-Score  | 0.652 |
| ROC-AUC   | 0.931 |

The CatBoost model achieved the highest ROC-AUC score, demonstrating excellent capability in distinguishing purchasing and non-purchasing sessions, particularly for imbalanced datasets.

---

## Key Insights

The most influential features identified by CatBoost were:

| Feature             | Importance |
| ------------------- | ---------- |
| Month               | 25.85%     |
| Page Values         | 24.39%     |
| Page Value Product  | 11.85%     |
| Exit Rates          | 4.38%      |
| Total Page Duration | 3.63%      |
| Product Pages Ratio | 3.30%      |

### Major Findings

* Seasonal trends significantly influence online purchases.
* Product page engagement strongly affects buying decisions.
* Higher page values are associated with increased purchase probability.
* Exit rates can indicate potential loss of customers before conversion.

---

## Technologies Used

* Python
* Pandas
* NumPy
* Scikit-learn
* CatBoost
* Matplotlib
* Seaborn
* Jupyter Notebook

---

## Repository Structure

Predicting-Online-Shopper-Behavior/
│
├── Base Paper Implementation/
├── Dataset/
├── Enhance Algorithm Implementaion/
├── Presentation/
├── README.md/

---

## Future Work

* Deep learning-based purchase prediction models
* Real-time recommendation systems
* Feature selection and dimensionality reduction
* Ensemble learning approaches
* Customer segmentation and personalization

---

## Author

**Farhat Khalid**

Project: Predicting Online Shopper Behavior with Machine Learning

Research Focus: Machine Learning, Data Analytics, Predictive Modeling, and E-commerce Intelligence.


