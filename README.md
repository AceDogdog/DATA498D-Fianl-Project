# DATA498D-Fianl-Project
# Predicting Stroke Risk: Machine Learning Approaches for Imbalanced Healthcare Data

## Project Overview
* **Problem Statement:** This project aims to predict the likelihood of a patient experiencing a stroke based on demographic and health indicators[cite: 2]. Accurately identifying high-risk patients is critical for early medical intervention and healthcare management.
* **Methodology:** The analysis addresses extreme class imbalance (95.1% healthy vs. 4.9% stroke)[cite: 2] through strategies like SMOTE and class-weighted Logistic Regression[cite: 2]. Missing BMI values were estimated using a K-Nearest Neighbors (KNN) imputer[cite: 2]. The predictive modeling compares Class-Weighted Logistic Regression, SMOTE Logistic Regression, and an Adjusted Random Forest model using threshold tuning[cite: 2].
* **Key Findings:** Feature importance analysis revealed that age, average glucose level, and BMI are the most critical factors for stroke prediction[cite: 2]. Furthermore, clinical odds ratios indicate that age (Odds Ratio: 6.56) and hypertension (Odds Ratio: 1.88) significantly increase the probability of a stroke[cite: 2].

## Data Sources
* **Dataset:** The project utilizes the `healthcare-dataset-stroke-data.csv` dataset[cite: 2].
* **Size:** The dataset originally contains 5,110 patient records and 11 attributes before preprocessing[cite: 2].
* **Variables:** Key variables include age, hypertension, heart disease, average glucose level, and smoking status[cite: 2]. For a complete description of each variable, please refer to the `data_dictionary.md` file in this repository[cite: 1].

## How to Run the Code
* **Dependencies:** Running this analysis requires Python and several libraries, including `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`, and `imblearn`[cite: 2].
* **Execution:** The complete analysis is contained within a single, fully reproducible Jupyter notebook[cite: 1]. To reproduce our findings, open the notebook file and run all cells sequentially from start to finish[cite: 1].

## Repository Structure
* `README.md`: Provides the project overview, how to run the notebook, and data sources[cite: 1].
* `CONTRIBUTIONS.md`: Documents the specific roles and contributions of each team member[cite: 1].
* `data_dictionary.md`: Describes every variable present in the stroke dataset[cite: 1].
* `analysis_notebook.ipynb`: Contains the reproducible Python code for data cleaning, exploratory data analysis, and model building[cite: 1].
