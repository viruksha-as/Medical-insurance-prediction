# 🏥 Medical Insurance Charge Prediction

> Predicts individual medical insurance costs using **Linear Regression** 
> based on age, BMI, smoking status, and region.

## 📌 Problem Statement
Insurance pricing is complex and opaque. This model estimates charges 
using key personal health indicators, making cost prediction accessible.

## 🛠️ Tech Stack
| Tool | Purpose |
|------|---------|
| Python | Core language |
| Scikit-learn | Linear Regression model |
| Pandas / NumPy | Data preprocessing |
| Matplotlib / Seaborn | Data visualization |
| Jupyter Notebook | Development environment |

## 📊 Dataset Features
| Feature | Type | Description |
|---------|------|-------------|
| age | int | Policyholder age |
| bmi | float | Body mass index |
| smoker | bool | Smoking status |
| region | categorical | US region |
| charges | float | **Target variable** |

## 📈 Model Performance (Best Model: Multi All Features)

| Metric | Training | Test |
|--------|----------|------|
| R² Score | 0.7417 | 0.7833 |
| Adj R² | 0.7403 | 0.7784 |
| MAE | 4,208 | 4,186 |
| RMSE | 6,105 | 5,799 |

> 7 model variants tested — from single-feature to multi-feature regression.  
> Smoking status + BMI combination gave the biggest performance jump.

## 🚀 How to Run
Open in Jupyter or Google Colab:
```bash
git clone https://github.com/viruksha-as/Medical-insurance-prediction.git
```
Then open `Medical_insurance.ipynb`

## 🔍 Key Findings
- Smoking status alone achieved R² of 0.74 — strongest single predictor
- Age and BMI alone performed poorly (R² ~0.08–0.12)
- Combining all features achieved best test R² of 0.78
- Model generalizes well — test performance slightly better than training
