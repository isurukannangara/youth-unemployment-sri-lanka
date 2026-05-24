# Youth Unemployment Patterns in Sri Lanka

### ST 3011 – Statistical Programming

A statistical analysis of youth unemployment patterns in Sri Lanka using data from the **Sri Lanka Labour Force Survey (LFS) 2023**, conducted by the Department of Census and Statistics.

---

## 📌 Project Overview

Youth unemployment is a significant socio-economic challenge in Sri Lanka. This study analyses patterns of youth unemployment (ages 15–29) across demographic, educational, and geographic dimensions using the LFS 2023 microdata.

### Objectives
1. Describe youth unemployment patterns using demographic characteristics (age, sex, sector, district)
2. Analyse the relationship between educational attainment and gender differences among unemployed youth
3. Examine gender differences in youth unemployment across sectors and geographic areas
4. Develop and evaluate a statistical model to identify factors associated with youth unemployment

---

## 📊 Dataset

- **Source:** Sri Lanka Labour Force Survey (LFS) 2023 — Department of Census and Statistics
- **Original size:** 18,937 observations, 128 variables
- **After preprocessing:** 1,428 economically active youth (ages 15–29)
  - 1,239 Employed
  - 189 Unemployed

> Dataset available at: [DCS Microdata Catalog](https://nada.statistics.gov.lk/index.php/catalog/489)

---

## 🔍 Key Findings

- Youth unemployment is **highest among ages 19–24**, declining steadily toward age 29
- **Female youth** experience higher unemployment (53.4%) than males (46.6%) across all sectors and regions
- **79.9% of unemployed youth** are from the rural sector, highlighting a significant rural–urban gap
- **Hambantota, Matara, and Badulla** record the highest district-level unemployment
- **Southern and Uva provinces** show the highest provincial unemployment rates
- The largest share of unemployed youth (50.8%) have completed **G.C.E. (A/L)**, indicating an education–labour market mismatch
- Chi-square analysis confirms a **statistically significant association** between education level and gender among unemployed youth
- Logistic regression identifies **female gender, younger age, estate sector residence, lower education, and Southern/Uva province** as key risk factors for unemployment

---

## 🧪 Methods Used

- **Exploratory Data Analysis (EDA)** — distributions, demographic breakdowns
- **Chi-square Tests of Independence** — gender vs education level, gender vs sector, gender vs province
- **Binary Logistic Regression** — baseline model and class-weighted model to handle class imbalance
- **Model Evaluation** — accuracy, precision, recall, F1-score, confusion matrices

---

## 📁 Repository Structure

```text
├── Group6_code.ipynb
├── LFS-2023-25-Percent-Data-Without-Computer.csv
├── README.md
```

---

## ▶️ How to Run

1. Clone this repository
2. Open `Group6_code.ipynb` in Jupyter Notebook or JupyterLab
3. Ensure the CSV file is in the same directory as the notebook
4. Install required libraries:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn statsmodels imbalanced-learn
```

5. Run all cells in order

---

## 👤 My Contribution
This was a group project. My specific contributions were:

- **Dataset Discovery** — identified and sourced the LFS 2023 microdata 
  from the Department of Census and Statistics
- **Data Preprocessing** — led the cleaning and recoding of raw survey 
  data by carefully studying the official survey documentation and 
  questionnaire
- **Statistical Modelling** — developed the binary logistic regression 
  models including addressing the class imbalance problem using 
  class weighting

---

## 📚 References

1. Department of Census and Statistics, Sri Lanka. (2023). *Labour Force Survey 2023* (Microdata).  
   https://nada.statistics.gov.lk/index.php/catalog/489
