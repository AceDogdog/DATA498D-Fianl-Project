# DATA498D-Fianl-Project
# Predicting Stroke Risk: Machine Learning Approaches for Imbalanced Healthcare Data

## Project Overview
* **Problem Statement:** This project aims to predict the likelihood of a patient experiencing a stroke based on demographic and health indicators. Accurately identifying high-risk patients is critical for early medical intervention and healthcare management.
* **Methodology:** The analysis addresses extreme class imbalance (95.1% healthy vs. 4.9% stroke) through strategies like SMOTE and class-weighted Logistic Regression. Missing BMI values were estimated using a K-Nearest Neighbors (KNN) imputer. The predictive modeling compares Class-Weighted Logistic Regression, SMOTE Logistic Regression, and an Adjusted Random Forest model using threshold tuning.
* **Key Findings:** Feature importance analysis revealed that age, average glucose level, and BMI are the most critical factors for stroke prediction. Furthermore, clinical odds ratios indicate that age (Odds Ratio: 6.56) and hypertension (Odds Ratio: 1.88) significantly increase the probability of a stroke.

## Data Sources
* **Dataset:** The project utilizes the `healthcare-dataset-stroke-data.csv` dataset.
* **Size:** The dataset originally contains 5,110 patient records and 11 attributes before preprocessing.
* **Variables:** Key variables include age, hypertension, heart disease, average glucose level, and smoking status. For a complete description of each variable, please refer to the `data_dictionary.md` file in this repository.

## How to Run the Code
* **Dependencies:** Running this analysis requires Python and several libraries, including `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`, and `imblearn`.
* **Execution:** The complete analysis is contained within a single, fully reproducible Jupyter notebook. To reproduce our findings, open the notebook file and run all cells sequentially from start to finish.

## Repository Structure
* `README.md`: Provides the project overview, how to run the notebook, and data sources.
* `CONTRIBUTIONS.md`: Documents the specific roles and contributions of each team member.
* `data_dictionary.md`: Describes every variable present in the stroke dataset.
* `analysis_notebook.ipynb`: Contains the reproducible Python code for data cleaning, exploratory data analysis, and model building.
