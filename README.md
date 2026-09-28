# CAS CS 506: Data Science Tools and Applications

**Group Members**
1. Sanyam Gupta
2. Talha Nadeem
3. Alejo Paullier
4. Shumail Inam

## Project Description

This project primarily aims to find how data science and machine learning techniques can be applied to the medical domain to better understand and predict thyroid disease risk. The first objective is to analyze thyroid disease risk datasets to identify which patient attributes are most strongly associated with a disease and to understand how these relationships in the dataset vary across different demographic groups. The second objective is to develop a machine learning model that can predict thyroid disease risk using relevant features from the datasets.

### Project Timeline

| Time Period | Planned Work |
|---|---|
| **Sept. 29 – Oct. 11** | Finalize the datasets and data sources. Explore dataset structures, common features, target distributions, missing values, and class imbalance. |
| **Oct. 12 – Oct. 25** | Clean and preprocess the datasets, standardize compatible features, perform initial feature engineering, and create preliminary exploratory visualizations. |
| **October Check-In** | Present preliminary visualizations, explain data collection/cleaning decisions, and show initial modeling experiments or baseline results. |
| **Oct. 26 – Nov. 8** | Finalize most data processing and feature selection. Perform demographic analysis across gender, ethnicity, and other relevant attributes. Train baseline classification models. |
| **Nov. 9 – Nov. 22** | Train and compare multiple models using 5-fold Stratified K-Fold validation. Evaluate Precision, Recall, F1-Score, ROC-AUC, and demographic-specific performance. Produce final-quality visualizations. |
| **November Check-In** | Present nearly finalized data processing, meaningful visualizations, at least 1–2 tested models, model performance results, and interpretations of the findings. |
| **Nov. 23 – Dec. 2** | Improve the strongest models, perform holdout testing and possible cross-dataset validation, analyze feature importance, demographic differences, limitations, and failure cases. |
| **Dec. 3 – Dec. 8** | Finalize the README/report, Makefile, reproducible pipeline, tests, GitHub workflow, figures, and results. Record the 10-minute final presentation. |
| **Dec. 9** | Submit the completed GitHub repository, final report, and presentation. |

## Project Goals

The first goal of our project is to predict the chance that an individual has a thyroid disease based on their biological data and external factors in their lives. This will be done by splitting our dataset into train and test sets, then seeing how close to the ground truth each model is. Using that to find which model generalizes best with unseen data.  
The second goal is to examine which attribute has the strongest association with a thyroid disease being present. This will be done by isolating patients with thyroid disease and finding commonalities, highlighting the feature with the largest correlation.

## Data collection and sources

We need to collect multiple datasets from different sources that contain features affecting thyroid disease risk. These different features will help us figure out how they affect thyroid disease risk. We plan on collecting data from Huggingface, Kaggle, and Github. We have found 3 different datasets totaling up to 38 different features and 242,000 rows approx. We are still trying to find more so the datasets are not exhaustive.

## Model testing strategies

We will reserve approximately 10% of the data as an unseen holdout test set.  
Because the target is imbalanced, we will use stratified sampling to preserve class proportions.  
For validation, we plan to use 5-fold Stratified K-Fold cross-validation.  
We will evaluate performance using Precision, Recall, F1-Score, and ROC-AUC.  
Accuracy will not be our primary metric because it can be misleading for imbalanced datasets.  
We will also compare model performance across demographic groups such as gender and ethnicity. If the datasets are sufficiently compatible, we will train on one dataset and test on the other to evaluate generalization.
