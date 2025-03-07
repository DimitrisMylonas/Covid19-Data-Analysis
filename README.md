# COVID-19 Data Analysis & Visualization Report

## Overview
This report provides an in-depth analysis of COVID-19 patient data through various visualizations. The goal is to uncover key patterns, trends, and correlations that could help in understanding factors associated with mortality, ICU admissions, and comorbidities.

---

## 1 Age Distribution of Patients
![Age Distribution](file-KivDhqPTj238pYnb2ZADaF)

**Analysis:**
- The age distribution is right-skewed, with a peak around 30-40 years.
- A significant number of cases involve patients aged between 20-60 years, indicating a higher exposure in working-age populations.
- The tail of the distribution suggests that older patients, while fewer in number, are still present in the dataset.

---

## 2️ Age Distribution of Survivors vs. Non-Survivors
![Age vs Mortality](file-Bpg19xVSDS4rN5XvYVnKFN)

**Analysis:**
- Non-survivors (red boxplot) tend to be significantly older compared to survivors.
- Survivors have a median age of around 40, while non-survivors' median age is around 60+.
- The presence of outliers in both groups suggests cases of mortality among younger individuals as well, although less frequent.

**Conclusion:** Age is a critical factor influencing mortality, with older individuals being at significantly higher risk.

---

## 3️ Diabetes and ICU Admission
![Diabetes & ICU](file-QxoR8M39EFzd4NUSUHFPag)

**Analysis:**
- Most of the patients **do not** have diabetes.
- Among diabetic patients, ICU admissions are notably higher compared to non-diabetic patients.
- This supports the notion that diabetes is a significant risk factor for severe COVID-19 outcomes.

---

## 4️ 3D Scatter Plot: Age, ICU Admission & Diabetes
![3D Scatter - ICU, Diabetes, Age](file-9VHw2eTWRsKoSpzJuzDhZa)

**Analysis:**
- This visualization shows that ICU admissions (Z-axis) and diabetes status (Y-axis) are correlated.
- Younger patients tend to have lower ICU admission rates compared to older patients.
- The color gradient represents age, reinforcing that ICU admissions increase with age and comorbidities.

---

## 5️ 3D Scatter Plot: Age, ICU Admission & Mortality
![3D Scatter - ICU & Mortality](file-Sym63v3skECpe5nYALscpm)

**Analysis:**
- Red points represent deceased patients, while blue represents survivors.
- The **majority of deaths occur in older individuals** who were admitted to the ICU.
- ICU admission is a strong indicator of severe disease progression, particularly in older patients.

---

## 6️ Correlation Heatmap with Mortality
![Heatmap](file-5C1pQtuaDLgjA9cjokE7G2)

**Analysis:**
- The strongest correlation with mortality is **ICU admission** and **intubation**.
- Age also has a moderate correlation with mortality, reinforcing previous findings.
- Comorbidities like hypertension, obesity, and diabetes show weaker correlations, but still contribute to worse outcomes.

---

## 7️ Sunburst Chart: ICU Admissions, Comorbidities & Mortality
![Sunburst](file-QbLyTkgL83sTaSy3QJk8ax)

**Analysis:**
- The chart illustrates the distribution of ICU admissions among patients with different comorbidities.
- Patients who **were not admitted to the ICU** had significantly better survival rates.
- The deeper layers show how comorbidities like diabetes and hypertension contribute to mortality.

---

## 8️ Ridgeline Plot: Age Distribution by Mortality
![Ridgeline Plot](file-HoT4euKMzaNpWWurAJyYau)

**Analysis:**
- The age distribution of survivors (blue) peaks around 40 years.
- The distribution of deceased patients (gray) is shifted towards older age groups.
- There is an overlap between the two groups, but the distinction in peak age is clear.

---

## 9️ 3D Surface Plot: Age & Mortality Rate
![3D Surface](file-LAyDayQV9eWi1hc3Cyp6tp)

**Analysis:**
- This visualization further highlights how mortality rates increase with age.
- The separation of red and blue points emphasizes that younger patients have lower mortality risks, even when admitted to the ICU.

---

## 10 Stacked Bar Chart: Comorbidities & Mortality
![Comorbidities vs Mortality](file-3joEG3xSgYY9Et1zx59PnB)

**Analysis:**
- This chart shows that conditions like diabetes, hypertension, and obesity are common among both survivors and non-survivors.
- However, the proportion of non-survivors is consistently higher among those with these comorbidities.
- This suggests that while comorbidities do not guarantee a fatal outcome, they significantly increase the risk.

---

## 11️ KDE Plot: Age Distribution by Survival
![KDE Plot](file-1wZzxxNmyx9BNpd25CYbBj)

**Analysis:**
- The distribution shows a clear separation between survivors and non-survivors.
- Younger individuals are more likely to survive, while mortality rates increase with age.

---

## 12️ Mortality Rate per Age Group
![Mortality Rate](file-Qk2jgajEqKZqP2Cr7cNXJ2)

**Analysis:**
- Mortality rates are minimal for younger age groups.
- A significant increase is observed for individuals over 60, peaking in the 80+ category.

---

## 13️ Parallel Coordinates: ICU, Comorbidities & Mortality
![Parallel Coordinates](file-CkSKVPFbNuCoJj48x8w4YN)

**Analysis:**
- This plot highlights how different features correlate with mortality.
- ICU admissions and age show the strongest connection to fatal outcomes.

---

## 14️ Feature Importance (Logistic Regression)
![Feature Importance](file-97oD2LmPcNkMx4WFC41zuE)

**Analysis:**
- Age is the most important predictor of mortality, followed by diabetes and ICU admission.

---

## 15️ Network Graph of Key Feature Correlations
![Network Graph](file-E99Q7Wz2kh8SBFb9xRs5VD)

**Analysis:**
- Shows clusters of interconnected features related to mortality and comorbidities.

---

## 16️ Animated Time-Series: COVID-19 Deaths Over Time
![Animated Time-Series](file-C5ysjeFEmuqxGaDhECnEPx)

**Analysis:**
- Displays trends in mortality over time, capturing peaks during outbreak waves.

---

## 17️ Heatmap of COVID-19 Mortality Over Time
![Heatmap Mortality](file-5qG1NTmzyo1M7mAWvuSvge)

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
