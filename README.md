# Linear-Regression-Analysis-for-Graduate-Admissions
📌 Project Overview
   Jamboree Education recently launched a feature where students can check their probability of graduate admission into top universities.
This project uses Linear Regression to analyze admission factors and predict the Chance of Admit based on student profiles (GRE, TOEFL, GPA, SOP, LOR, Research, etc.).

The analysis not only builds a predictive model but also provides actionable insights for students and Jamboree.


📊 Dataset
  File: jamboree_admission.csv

Columns:

Serial No. – Unique row ID (dropped during analysis)
GRE Score – Graduate Record Exam score (out of 340)
TOEFL Score – English language test score (out of 120)
University Rating – Rating of the university (out of 5)
SOP – Statement of Purpose strength (out of 5)
LOR – Letter of Recommendation strength (out of 5)
CGPA – Undergraduate GPA (out of 10)
Research – Research experience (0 = No, 1 = Yes)
Chance of Admit – Target variable (0–1)

🛠️ Methodology
1. Exploratory Data Analysis (EDA)
Checked data types, shape, missing values, and duplicates.
Descriptive statistics for all features.
Univariate analysis (distribution plots).
Bivariate analysis (correlation & scatterplots with Chance of Admit).
2. Data Preprocessing
Dropped Serial No..
Outlier detection and treatment.
Prepared dataset for regression modeling.
3. Model Building
Linear Regression (Statsmodels & Scikit-learn).
Ridge and Lasso regression for comparison.
Coefficient analysis to identify key predictors.
4. Model Assumption Testing
✅ Multicollinearity check (VIF < 5).
✅ Residuals mean ≈ 0.
✅ Linearity check (residuals vs fitted values).
✅ Homoscedasticity (constant variance of residuals).
✅ Normality of residuals (QQ Plot & Histogram).
5. Model Evaluation
Metrics:
R² = 0.82
Adjusted R² = 0.81
MAE = 0.04
RMSE = 0.06
Ridge & Lasso confirmed importance of GRE, TOEFL, GPA, and Research.
💡 Insights & Recommendations
Strongest predictors: GPA, GRE, TOEFL, and Research.
Moderate predictors: SOP & LOR have low but positive effect.
Key takeaway: Students should prioritize strong academic performance (CGPA), GRE, and TOEFL preparation. Research experience significantly boosts admission chances.
For Jamboree:
Focus guidance on GRE/TOEFL prep & academic improvement.
Encourage students to take up research projects.
Deploy this model on the Jamboree website for real-time predictions.
📂 Project Files
Jamboree - Colab.pdf → Detailed report with code, EDA, regression analysis, and insights.
jamboree_admission.csv → Dataset.
notebook.ipynb → Colab notebook (if included).
README.md → Project documentation.
🚀 Future Scope
Incorporate additional variables like extracurriculars, internships, publications.
Try advanced models (Random Forest, Gradient Boosting) for improved accuracy.
Deploy as a Flask/Django web app for student use.
🧑‍💻 Technologies Used
Python (Pandas, NumPy, Matplotlib, Seaborn)
Statsmodels
Scikit-learn
Jupyter/Google Colab
