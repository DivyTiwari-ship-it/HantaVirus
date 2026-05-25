# 🦠 HantaVirus Prediction

![Python](https://img.shields.io/badge/Python-3.8+-blue)
![ML](https://img.shields.io/badge/ML-XGBoost-green)
![Accuracy](https://img.shields.io/badge/Accuracy-89.67%25-brightgreen)

## 📌 Overview
Predicted whether a patient is likely to have **HantaVirus syndrome**  
using Machine Learning on epidemiological outbreak data.  
The dataset included features such as confirmed cases, deaths, hospitalization records, and transmission-related information.

The model was trained to analyze outbreak patterns and disease severity.

---

## 📊 Results
| Model | Accuracy |
|-------|----------|
| Random Forest (baseline) | 81.42% |
| **XGBoost ✅** | **89.67%** |

---

## 🔧 Feature Engineering
| Feature | Description |
|---------|-------------|
| confirmed_cases | Total confirmed cases |
| deaths | Number of deaths |
| recovered | Total recovered patients |
| case_fatality_rate | Death percentage |
| hospitalized | Hospitalized patients |
| icu_admissions | ICU admissions |
| human_to_human_cases | Human transmission cases |
| latitude / longitude | Geographic outbreak location |

---

## 🛠️ Tech Stack
![Python](https://img.shields.io/badge/-Python-black?logo=python)
![Pandas](https://img.shields.io/badge/-Pandas-black?logo=pandas)
![NumPy](https://img.shields.io/badge/-NumPy-black?logo=numpy)
![XGBoost](https://img.shields.io/badge/-XGBoost-black)
![Seaborn](https://img.shields.io/badge/-Seaborn-black)

---

## 🚀 How to Run
```bash
git clone https://github.com/DivyTiwari-ship-it/HantaVirus.git

cd HantaVirus

pip install -r requirements.txt

jupyter notebook
```

---

## 💡 Key Learnings
- Preprocessing has a huge impact on epidemiological datasets
- XGBoost captured outbreak patterns better than RandomForest
- ICU admissions and fatality rate were strong predictive indicators
- Geographic features helped improve outbreak prediction
- Real-world healthcare datasets are noisy, making feature engineering very important- Epidemiological datasets me preprocessing ka huge impact hota hai
- XGBoost outbreak patterns ko better capture karta hai
- ICU admissions aur fatality rate strong indicators nikle
- Geographic features outbreak prediction me useful rahe
- Real-world healthcare data noisy hota hai, feature engineering matters a lot
