# 👥 Team Contributions

This document outlines the specific roles and responsibilities of each team member in the **Predicting Stroke Risk** project. The project was divided into five key phases, with team members taking ownership of specific code implementations and analyses.

### 📊 Responsibility Breakdown

| Phase | Task / Step | Primary Contributor | Description of Contribution |
| :---: | :--- | :--- | :--- |
| **Step 1** | **Data Loading and Splitting** | `[Yiqi Hu]` | Responsible for importing the raw stroke dataset, performing initial data cleaning (e.g., dropping the 'id' column, removing invalid 'Other' gender records), and establishing a rigorous 80/20 stratified train/test split to prevent data leakage. |
| **Step 2** | **Exploratory Data Analysis (EDA)** | `[Zhiyao Liu]` | Conducted comprehensive EDA on the training set. Generated statistical summaries and visualizations (boxplots for outliers, KDE plots for distributions, and correlation heatmaps) to uncover underlying patterns and highlight the severe class imbalance. |
| **Step 3** | **Data Preprocessing and Preparation** | `[Zhuoyan Li]` | Handled missing data by implementing a K-Nearest Neighbors (KNN) imputer for the BMI feature. Applied One-Hot Encoding to categorical variables and used `StandardScaler` to normalize continuous features, ensuring the dataset was fully optimized for machine learning algorithms. |
| **Step 4** | **Modeling and Handling Imbalance** | `[Xinrui Li]` | Addressed the extreme class imbalance by implementing SMOTE (Synthetic Minority Over-sampling Technique). Trained and tuned multiple predictive models, including Class-Weighted Logistic Regression, SMOTE Logistic Regression, and Random Forest Classifier. |
| **Step 5** | **Model Evaluation and Clinical Insights** | **Zongbo Li** | Evaluated model performance using advanced metrics suitable for imbalanced data, focusing on Precision-Recall AUC (PR-AUC) and custom threshold tuning. Extracted feature importances and translated statistical odds ratios into actionable clinical insights. |

---
*Note: While primary responsibilities were divided as shown above, all team members actively participated in code reviews, bug fixing, and finalizing the project report and documentation.*
