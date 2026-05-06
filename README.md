# DATA498D-Fianl-Project
# Predicting Stroke Risk: Machine Learning Approaches for Imbalanced Healthcare Data

## Project Overview
* [cite_start]**Problem Statement:** This project aims to predict the likelihood of a patient experiencing a stroke based on demographic and health indicators[cite: 91]. Accurately identifying high-risk patients is critical for early medical intervention and healthcare management.
* [cite_start]**Methodology:** The analysis addresses extreme class imbalance (95.1% healthy vs. 4.9% stroke) [cite: 138] [cite_start]through strategies like SMOTE [cite: 258] [cite_start]and class-weighted Logistic Regression[cite: 261]. [cite_start]Missing BMI values were estimated using a K-Nearest Neighbors (KNN) imputer[cite: 105]. [cite_start]The predictive modeling compares Class-Weighted Logistic Regression, SMOTE Logistic Regression [cite: 280][cite_start], and an Adjusted Random Forest model using threshold tuning[cite: 285, 287].
* [cite_start]**Key Findings:** Feature importance analysis revealed that age, average glucose level, and BMI are the most critical factors for stroke prediction[cite: 324, 325, 326]. [cite_start]Furthermore, clinical odds ratios indicate that age (Odds Ratio: 6.56) and hypertension (Odds Ratio: 1.88) significantly increase the probability of a stroke[cite: 351].

## Data Sources
* [cite_start]**Dataset:** The project utilizes the `healthcare-dataset-stroke-data.csv` dataset[cite: 89].
* [cite_start]**Size:** The dataset originally contains 5,110 patient records and 11 attributes before preprocessing[cite: 94].
* [cite_start]**Variables:** Key variables include age, hypertension, heart disease, average glucose level, and smoking status[cite: 95, 96]. [cite_start]For a complete description of each variable, please refer to the `data_dictionary.md` file in this repository[cite: 35].

## How to Run the Code
* [cite_start]**Dependencies:** Running this analysis requires Python and several libraries, including `pandas` [cite: 77][cite_start], `numpy` [cite: 78][cite_start], `matplotlib` [cite: 79][cite_start], `seaborn` [cite: 80][cite_start], `scikit-learn` [cite: 82, 226][cite_start], and `imblearn`[cite: 255].
* [cite_start]**Execution:** The complete analysis is contained within a single, fully reproducible Jupyter notebook[cite: 34]. To reproduce our findings, open the notebook file and run all cells sequentially from start to finish.

## Repository Structure
* [cite_start]`README.md`: Provides the project overview, how to run the notebook, and data sources[cite: 34].
* [cite_start]`CONTRIBUTIONS.md`: Documents the specific roles and contributions of each team member[cite: 36].
* [cite_start]`data_dictionary.md`: Describes every variable present in the stroke dataset[cite: 35].
* [cite_start]`analysis_notebook.ipynb`: Contains the reproducible Python code for data cleaning, exploratory data analysis, and model building[cite: 34].
