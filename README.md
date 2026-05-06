# 🏥 DATA498D-Final-Project
# 🧠 Predicting Stroke Risk: Machine Learning Approaches for Imbalanced Healthcare Data

## 📊 Project Overview
* **🎯 Problem Statement:** This project aims to predict the likelihood of a patient experiencing a stroke based on demographic and health indicators. Accurately identifying high-risk patients is critical for early medical intervention and healthcare management.
* **🛠️ Methodology:** The analysis addresses extreme class imbalance through strategies like SMOTE and class-weighted Logistic Regression. Missing BMI values were estimated using a K-Nearest Neighbors (KNN) imputer (with `n_neighbors=5`). The predictive modeling compares Class-Weighted Logistic Regression, SMOTE Logistic Regression, and a Random Forest model using threshold tuning (evaluated at a 0.1 threshold for the Random Forest).
* **📈 Key Findings:** Feature importance analysis and clinical odds ratios indicate that age (Odds Ratio: 6.58), child work type (`work_type_children` Odds Ratio: 2.44), and hypertension (Odds Ratio: 1.88) significantly increase the probability of a stroke. 

## 📁 Data Sources
* **📄 Dataset:** The project utilizes the `healthcare-dataset-stroke-data.csv` dataset.
* **📏 Size:** The dataset originally contains 5,110 patient records and 11 attributes before preprocessing.
* **📌 Variables:** Key variables include age, hypertension, heart disease, average glucose level, and smoking status. For a complete description of each variable, please refer to the `data_dictionary.md` file in this repository.

## 🚀 How to Run the Code
* **💻 Dependencies:** Running this analysis requires Python and several libraries, including `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`, and `imblearn`.
* **▶️ Execution:** The complete analysis is contained within a single, fully reproducible Jupyter notebook. To reproduce our findings, open the notebook file and run all cells sequentially from start to finish.

## 🗂️ Repository Structure
* `README.md`: Provides the project overview, how to run the notebook, and data sources.
* `CONTRIBUTIONS.md`: Documents the specific roles and contributions of each team member.
* `data_dictionary.md`: Describes every variable present in the stroke dataset.
* `analysis_notebook.ipynb`: Contains the reproducible Python code for data cleaning, exploratory data analysis, and model building.
