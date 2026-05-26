# 🦠 Hantavirus Death Prediction

![Python](https://img.shields.io/badge/Python-3.8+-blue)
![ML](https://img.shields.io/badge/ML-XGBoost-green)
![R2 Score](https://img.shields.io/badge/R2%20Score-96.57%25-brightgreen)
![MAE](https://img.shields.io/badge/MAE-3.89-yellow)

## 📌 Overview
Predicted the **number of deaths** caused by Hantavirus (Andes Virus) across different countries and years  
using Machine Learning on global epidemiological data spanning **1993–2026**.

Dataset source: [Kaggle — Hantavirus Andes Virus Global Epidemiology](https://www.kaggle.com/datasets/zkskhurram/hantavirus-andes-virus-global-epidemiology)

---

## 📊 Results

| Model | MAE | R2 Score |
|-------|-----|----------|
| Random Forest (baseline) | 7.17 | 0.9224 |
| **XGBoost ✅** | **3.89** | **0.9657** |

---

## 🔧 Feature Engineering

| Feature | Description |
|---------|-------------|
| icu_to_hospital_ratio | ICU admissions / hospitalized |
| hospitalization_rate | Hospitalized / confirmed cases |
| distance_from_equator | Absolute latitude value |
| is_northern_hemisphere | 1 if latitude > 0, else 0 |
| region_avg_fatality | Mean fatality rate per WHO region |
| syndrome_region | Syndrome + WHO region combined |
| h2h_intensity | Confirmed cases × human-to-human cases |

---

## 🛠️ Tech Stack

![Python](https://img.shields.io/badge/-Python-black?logo=python)
![Pandas](https://img.shields.io/badge/-Pandas-black?logo=pandas)
![XGBoost](https://img.shields.io/badge/-XGBoost-black)
![Scikit-Learn](https://img.shields.io/badge/-ScikitLearn-black?logo=scikit-learn)
![Seaborn](https://img.shields.io/badge/-Seaborn-black)
![Matplotlib](https://img.shields.io/badge/-Matplotlib-black)

---

## 🚀 How to Run

```bash
git clone https://github.com/DivyTiwari-ship-it/HantaVirus
pip install -r requirements.txt
jupyter notebook hantavirus.ipynb
```

---

## 💡 Key Learnings
- Feature engineering (region fatality, ICU ratio) significantly improved model performance
- XGBoost outperformed RandomForest — MAE almost halved (7.17 → 3.89)
- Epidemiological data requires Regression, not Classification — deaths is a continuous variable
- WHO region-based grouping was one of the most impactful features
