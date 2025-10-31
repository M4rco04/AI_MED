# 🩺 Medical Data Analysis and ML Model Classification

This project performs data analysis and classification of medical data based on geometric heart features (e.g., heart perimeter, inscribed circle radius, CTR ratio).

---

## 📋 Overview

The script performs the following steps:

1. **Data import** from `task_data.csv`.  
2. **Data preprocessing**:  
   - Converts comma-separated numbers to dots,  
   - Removes unnecessary spaces from column names,  
   - Standardizes feature values.  
3. **Data analysis**:  
   - Correlation matrix (`seaborn.heatmap`),  
   - Pair plot (`sns.pairplot`).  
4. **Model training** using three classifiers:  
   - Support Vector Machine (SVM)  
   - Logistic Regression  
   - Random Forest  
5. **Model evaluation** using accuracy (`accuracy_score`) and cross-validation (`cross_val_score`).  
6. **Model comparison** on the test set.

---

## ⚙️ Requirements

To run this script, install the following dependencies:

```bash
pip install -r requirements.txt
```

---

## 🚀 How to Run

1. Place the file `task_data.csv` in the same directory as the script.  
2. Run the script:
   ```bash
   python Cardiomyopathy.py
   ```
3. The results (best parameters and accuracy scores) will be printed in the console.

---

## 📊 Example Results

| Model                  | Best Accuracy| Cross-Validation Accuracy | Test Accuracy |
|------------------------|--------------|---------------------------|---------------|
| Support Vector Machine | 0.85         | 0.54                      | 0.875         |
| Logistic Regression    | 0.795        | 0.628                      | 0.75         |
| Random Forest          | 0.745        | 0.696                      | 0.875         |

---
