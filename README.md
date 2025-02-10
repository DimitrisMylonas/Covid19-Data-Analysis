# COVID-19 Data Analysis & Visualization Report

## Overview
This report provides an in-depth analysis of COVID-19 patient data through various visualizations. The goal is to uncover key patterns, trends, and correlations that could help in understanding factors associated with mortality, ICU admissions, and comorbidities.

---

## 1 Age Distribution of Patients

**Analysis:**
- The age distribution is right-skewed, with a peak around 30-40 years.
- A significant number of cases involve patients aged between 20-60 years, indicating a higher exposure in working-age populations.
- The tail of the distribution suggests that older patients, while fewer in number, are still present in the dataset.

---

## 2 Age Distribution of Survivors vs. Non-Survivors

**Analysis:**
- Non-survivors (red boxplot) tend to be significantly older compared to survivors.
- Survivors have a median age of around 40, while non-survivors' median age is around 60+.
- The presence of outliers in both groups suggests cases of mortality among younger individuals as well, although less frequent.

**Conclusion:** Age is a critical factor influencing mortality, with older individuals being at significantly higher risk.

---

## 3 Diabetes and ICU Admission

**Analysis:**
- Most of the patients **do not** have diabetes.
- Among diabetic patients, ICU admissions are notably higher compared to non-diabetic patients.
- This supports the notion that diabetes is a significant risk factor for severe COVID-19 outcomes.

---

## 4 3D Scatter Plot: Age, ICU Admission & Diabetes

**Analysis:**
- This visualization shows that ICU admissions (Z-axis) and diabetes status (Y-axis) are correlated.
- Younger patients tend to have lower ICU admission rates compared to older patients.
- The color gradient represents age, reinforcing that ICU admissions increase with age and comorbidities.

---

## 5 3D Scatter Plot: Age, ICU Admission & Mortality

**Analysis:**
- Red points represent deceased patients, while blue represents survivors.
- The **majority of deaths occur in older individuals** who were admitted to the ICU.
- ICU admission is a strong indicator of severe disease progression, particularly in older patients.

---

## 6 Correlation Heatmap with Mortality

**Analysis:**
- The strongest correlation with mortality is **ICU admission** and **intubation**.
- Age also has a moderate correlation with mortality, reinforcing previous findings.
- Comorbidities like hypertension, obesity, and diabetes show weaker correlations, but still contribute to worse outcomes.

---

## 7 Sunburst Chart: ICU Admissions, Comorbidities & Mortality

**Analysis:**
- The chart illustrates the distribution of ICU admissions among patients with different comorbidities.
- Patients who **were not admitted to the ICU** had significantly better survival rates.
- The deeper layers show how comorbidities like diabetes and hypertension contribute to mortality.

---

## 8 Ridgeline Plot: Age Distribution by Mortality

**Analysis:**
- The age distribution of survivors (blue) peaks around 40 years.
- The distribution of deceased patients (gray) is shifted towards older age groups.
- There is an overlap between the two groups, but the distinction in peak age is clear.

---

## 9 3D Surface Plot: Age & Mortality Rate

**Analysis:**
- This visualization further highlights how mortality rates increase with age.
- The separation of red and blue points emphasizes that younger patients have lower mortality risks, even when admitted to the ICU.

---

## 10 Stacked Bar Chart: Comorbidities & Mortality

**Analysis:**
- This chart shows that conditions like diabetes, hypertension, and obesity are common among both survivors and non-survivors.
- However, the proportion of non-survivors is consistently higher among those with these comorbidities.
- This suggests that while comorbidities do not guarantee a fatal outcome, they significantly increase the risk.

---

## 11 KDE Plot: Age Distribution by Survival

**Analysis:**
- The distribution shows a clear separation between survivors and non-survivors.
- Younger individuals are more likely to survive, while mortality rates increase with age.

---

## 12 Mortality Rate per Age Group

**Analysis:**
- Mortality rates are minimal for younger age groups.
- A significant increase is observed for individuals over 60, peaking in the 80+ category.

---

## 13 Parallel Coordinates: ICU, Comorbidities & Mortality

**Analysis:**
- This plot highlights how different features correlate with mortality.
- ICU admissions and age show the strongest connection to fatal outcomes.

---

## 14 Feature Importance (Logistic Regression)

**Analysis:**
- Age is the most important predictor of mortality, followed by diabetes and ICU admission.

---

## 15 Network Graph of Key Feature Correlations

**Analysis:**
- Shows clusters of interconnected features related to mortality and comorbidities.

---

## 16 Animated Time-Series: COVID-19 Deaths Over Time

**Analysis:**
- Displays trends in mortality over time, capturing peaks during outbreak waves.

---

## 17 Heatmap of COVID-19 Mortality Over Time

**Analysis:**
- Highlights mortality peaks and their temporal distribution.



## Conclusion & Future Work

### Key Findings:
- **Age and ICU admissions are the strongest predictors of mortality.**
- **Diabetes, hypertension, and obesity increase risk but are secondary factors.**
- **Comorbidities alone do not determine mortality, but their combination with age significantly raises the risk.**

### Future Work & Machine Learning Applications:
- **Predictive Modeling:** Logistic regression, random forests, and gradient boosting (e.g., XGBoost) could be used to predict patient mortality.
- **Risk Stratification:** Clustering techniques (e.g., K-Means, DBSCAN) could group patients based on risk factors.
- **Time-Series Analysis:** Recurrent neural networks (RNNs) or ARIMA models could analyze trends in COVID-19 mortality over time.
- **Feature Engineering:** Further exploration of interactions between comorbidities and ICU admissions to improve model performance.
- **Bias Consideration:** Addressing potential dataset imbalances to ensure models generalize well across different patient demographics.

By leveraging machine learning techniques, this analysis could be extended to develop models that assist in early risk prediction, resource allocation, and improved patient care strategies.
