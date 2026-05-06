# 📖 Data Dictionary

This document describes the variables present in the `healthcare-dataset-stroke-data.csv` dataset used for the predicting stroke risk project. 

The original dataset contained 12 columns. During the preprocessing phase, the `id` column was dropped as it contained no predictive value, and rows with the `gender` labeled as "Other" were removed to maintain a strict binary classification.

### 🎯 Target Variable
| Variable Name | Data Type | Description |
| :--- | :--- | :--- |
| **`stroke`** | Integer (Binary) | The target variable for prediction. <br> `1` = The patient had a stroke <br> `0` = The patient did not have a stroke |

---

### 👤 Demographic Indicators
| Variable Name | Data Type | Description |
| :--- | :--- | :--- |
| **`gender`** | Categorical | The biological sex of the patient. <br> Values: `"Male"`, `"Female"` *(Note: "Other" was removed during preprocessing)*. |
| **`age`** | Numeric (Float) | The age of the patient in years. |
| **`ever_married`** | Categorical | Indicates whether the patient has ever been married. <br> Values: `"Yes"`, `"No"`. |
| **`work_type`** | Categorical | The employment or work status of the patient. <br> Examples of values: `"Private"`, `"Self-employed"`, `"children"`, `"Govt_job"`, `"Never_worked"`. |
| **`Residence_type`** | Categorical | The type of environment the patient resides in. <br> Values: `"Urban"`, `"Rural"`. |

---

### 🩺 Clinical & Health Indicators
| Variable Name | Data Type | Description |
| :--- | :--- | :--- |
| **`hypertension`** | Integer (Binary) | Indicates whether the patient suffers from hypertension (high blood pressure). <br> `1` = Has hypertension <br> `0` = Does not have hypertension |
| **`heart_disease`** | Integer (Binary) | Indicates whether the patient has a history of heart disease. <br> `1` = Has heart disease <br> `0` = Does not have heart disease |
| **`avg_glucose_level`** | Numeric (Float) | The patient's average blood glucose level (sugar level in the blood) measured in mg/dL. |
| **`bmi`** | Numeric (Float) | Body Mass Index, calculated as weight in kilograms divided by height in meters squared. <br> *(Note: The original dataset had 163 missing values in the training set, which were imputed using a KNN Imputer with `n_neighbors=5`)*. |

---

### 🚬 Lifestyle Factors
| Variable Name | Data Type | Description |
| :--- | :--- | :--- |
| **`smoking_status`** | Categorical | The smoking habit/history of the patient. <br> Values: `"smokes"`, `"formerly smoked"`, `"never smoked"`, `"Unknown"` *(Unknown implies the information is unavailable)*. |

---

### ⚙️ Feature Engineering Note
During the modeling process (in `analysis_notebook.ipynb`), all categorical variables (`gender`, `ever_married`, `work_type`, `Residence_type`, `smoking_status`) were converted into numerical formats using One-Hot Encoding (`pd.get_dummies` with `drop_first=True`). Continuous variables (`age`, `avg_glucose_level`, `bmi`) were standardized using `StandardScaler`.
