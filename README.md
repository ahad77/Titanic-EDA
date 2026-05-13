# Titanic Disaster: Exploratory Data Analysis (EDA)

## 📌 Project Overview
This repository contains a comprehensive Exploratory Data Analysis (EDA) of the Titanic dataset. The goal is to identify high-signal predictors for survival and assess data integrity for machine learning readiness[cite: 1, 2].

## 📊 Technical Insights
*   **Survival Distribution:** The global survival rate is 38.38%.
*   **Feature Dominance:** 'Sex' and 'Pclass' provide the highest information gain. Females had a survival rate of ~74% compared to ~18% for males[cite: 1, 2].
*   **Socio-Economic Correlation:** 1st-class passengers had a >60% survival probability, validating 'Pclass' as a primary proxy for evacuation priority[cite: 1, 2].
*   **Non-Linearity:** Age distribution shows a survival spike in the [0-10] pediatric cohort[cite: 1, 2].

## 🛠 Engineering Strategy
*   **Imputation:** Handle 19.8% missingness in 'Age' using grouped medians to preserve variance[cite: 1, 2].
*   **Sparsity Management:** Drop 'Cabin' (77% null) to reduce model noise[cite: 1, 2].
*   **Normalization:** Log-transform 'Fare' to address distribution skewness[cite: 2].

## 🚀 Usage
1. Clone the repo.
2. Install dependencies: `pip install -r requirements.txt`
3. Run the Jupyter notebook in the `/notebooks` folder.
