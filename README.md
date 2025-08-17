# University Admission Predictor

**Author:** Aki Harsha

---

## Project Overview
This project predicts whether a student will be **admitted or rejected** to a university in the USA based on academic and personal credentials. The model uses **Logistic Regression**, a classical machine learning algorithm suitable for binary classification problems.

The goal of this project is to provide a simple predictive tool for admissions based on historical data.

---

## Dataset
The dataset used for this project is `Admission_Predict.csv`, which contains the following features:

- **GRE Score:** Graduate Record Exam score  
- **TOEFL Score:** Test of English as a Foreign Language score  
- **University Rating:** Ranking of the target university  
- **SOP:** Statement of Purpose strength  
- **LOR:** Letter of Recommendation strength  
- **CGPA:** Undergraduate GPA  
- **Research:** Research experience (0 = No, 1 = Yes)  
- **Chance of Admit:** Original probability of admission (converted to binary for this project)  

---

## Files
- `Admission_Predict.csv` — Dataset for the project  
- `unipredict.ipynb` — Jupyter Notebook containing data preprocessing, model training, evaluation, and prediction  
- `README.md` — Project documentation  

---

## Data Preprocessing
- Checked for missing values and handled them appropriately  
- Converted the continuous **Chance of Admit** into a binary **Admit/Reject** variable using a threshold of 0.75  
- Encoded categorical variables  
- Standardized numeric features using **StandardScaler** to improve model performance  

---

## Model
- **Algorithm:** Logistic Regression  
- **Purpose:** Predict binary admission outcome (Admit = 1, Reject = 0)  

---

## Performance Metrics
| Metric    | Value |
|-----------|-------|
| Accuracy  | 0.91  |
| Precision | 0.86  |
| Recall    | 0.93  |
| F1-Score  | 0.89  |

These metrics indicate that the model performs well in correctly predicting admitted students while minimizing false negatives.

---

## How to Use
1. Clone the repository:  
   ```bash
   git clone https://github.com/<your-username>/university-admission-predictor.git
