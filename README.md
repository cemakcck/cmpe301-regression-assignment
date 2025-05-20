# 🧠 Regression Model for Missing Value Imputation – CMPE301 Project

This project showcases a regression-based approach to clean missing data in a `.parquet` dataset using a machine learning model. It was originally developed as part of the CMPE301 course at Istanbul Bilgi University.

---

## 📝 Project Overview

The dataset contains missing values marked as `-100` in **column G**. The objective is to:

- Detect and isolate missing values
- Train a regression model on valid data
- Predict the missing entries
- Replace `-100` values with predicted results
- Save the cleaned dataset as a new `.parquet` file

---

## 💾 Files

| File | Description |
|------|-------------|
| `Cem_Akcicek_122200044_Assignment.ipynb` | The full notebook with code, model, and logic |
| `122200044.parquet` | Output file with all `-100`s in column G replaced |
| `modified.parquet` | *(Not included)* – This is the instructor-provided input file and must be placed manually for the notebook to run

---

## ⚙️ Model Details

- Model: `RandomForestRegressor`
- Handling: One-hot encoding for categorical features
- Evaluation: Mean Squared Error logged during training

```python
Mean Squared Error: ~0.34
