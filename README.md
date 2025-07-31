# Autism Spectrum Disorder Classification

### Project Overview

This project aims to classify **Autism Spectrum Disorder (ASD)** in toddlers based on responses to a set of screening questions (A1-A10) and demographic information. The goal is to develop a machine learning model that can accurately predict whether a toddler has ASD, potentially facilitating early diagnosis and intervention.

-----

### Technical Highlights

  * **Dataset**: [Kaggle - Autism Screening for Toddlers](https://www.kaggle.com/datasets/fabdelja/autism-screening-for-toddlers)
  * **Size**: 6075 entries, 15 columns
  * **Key Features**:
      * A1-A10 (screening questions), Age, Sex, Jaundice, Family\_ASD.
  * **Approach**:
      * Data Cleaning: Dropped duplicate rows (847 duplicates found). No missing values.
      * Exploratory Data Analysis: Histograms, Boxplots, and Heatmaps were used for visualization to understand data distributions and correlations.
      * Label Encoding: Applied to all columns, including numerical ones and the target 'Class'.
      * Binary Classification: The target variable 'Class' indicates ASD ('YES') or no ASD ('NO').
      * Models Used:
          * Logistic Regression, Ridge Classifier, SVC, Random Forest, XGBoost, AdaBoost, Gradient Boosting, Bagging, Decision Tree.
  * **Best Accuracy**:
      * 99.9% with Gradient Boosting Classifier.
      * 99.8% with AdaBoost Classifier.
      * 99.4% with XGBoost Classifier.
      * The very high accuracies suggest that the screening questions and demographic factors provide strong discriminative power for ASD classification in this dataset.

-----

### Purpose and Applications

  * Assist in the **early screening and potential diagnosis of Autism Spectrum Disorder** in toddlers.
  * Provide a preliminary assessment tool for parents and healthcare providers to identify children who may benefit from further evaluation.
  * Facilitate timely intervention and support for children with ASD.
  * Contribute to research on early markers and diagnostic methods for ASD.

-----

### Installation

Clone the repository:

```bash
git clone https://github.com/BhaveshBhakta/Autism-Spectrum-Disorder-Classification-Using-ML.git
cd Autism-Spectrum-Disorder-Classification-Using-ML
```

Install the necessary libraries:

```bash
pip install pandas numpy seaborn matplotlib scikit-learn xgboost
```

-----

### Collaboration

We welcome contributions to improve the project. You can help by:

  * Thoroughly investigating the very high accuracy to ensure no data leakage or overfitting is present, which is particularly important for sensitive medical diagnosis tasks.
  * Performing comprehensive hyperparameter tuning and cross-validation for all models to ensure robustness.
  * Exploring the impact of different feature selection or weighting strategies for the A1-A10 questions.
  * Adding explainability (e.g., SHAP or LIME) to understand which screening questions and demographic factors are most indicative of an ASD diagnosis.
