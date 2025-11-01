# 🧮 Statistics Analysis and Regression Project

## 🎯 Objective
This project investigates whether there is a **statistically significant difference** in the average house sale price (`SalePrice`) across different categories of `GarageFinish`.

Additionally, it builds a **multiple linear regression model** to predict `SalePrice` using the best set of predictors, while ensuring model assumptions are not violated.

---

## 📊 Dataset
The dataset contains information about house characteristics and sale prices.

Key variables:
- `GarageFinish`: Category of garage finishing (e.g., Fin, RFn, Unf, None)
- `SalePrice`: Final sale price of the house (target variable)

---

## 🧠 Hypotheses
**Null Hypothesis (H₀):**  
There is **no statistically significant difference** in the mean `SalePrice` among the different `GarageFinish` categories.

**Alternative Hypothesis (H₁):**  
At least one category of `GarageFinish` has a **significantly different** mean `SalePrice`.

Significance level: **α = 0.05**

---

## ⚙️ Steps & Methodology
1. **Data Preparation**
   - Handle missing values (`GarageFinish` → filled with “None”)
   - Keep relevant columns (`GarageFinish`, `SalePrice`)
   - Ensure data cleanliness and proper typing

2. **Exploratory Data Analysis (EDA)**
   - Visualize `SalePrice` distribution by `GarageFinish`
   - Check variance and spread across groups

3. **Statistical Testing**
   - Check normality and homogeneity of variance assumptions  
   - Choose appropriate test:
     - **Parametric:** One-way ANOVA (if assumptions met)
     - **Non-parametric:** Kruskal-Wallis test (if assumptions violated)
   - Perform **Post-hoc (pairwise)** tests to compute adjusted p-values

4. **Regression Modeling**
   - Build a **Multiple Linear Regression Model** to predict `SalePrice`
   - Select best predictors (based on correlation, significance, and VIF)
   - Validate model assumptions:
     - Linearity  
     - Homoscedasticity  
     - Normality of residuals  
     - Multicollinearity check

5. **Conclusion**
   - Interpret statistical results (p-values, F-statistics)
   - Report significant findings
   - Summarize regression insights and predictive power (R² score)

---

## 🧩 Tools & Libraries
- **Python 3**
- `pandas`, `numpy`
- `matplotlib`, `seaborn`
- `scipy.stats`, `statsmodels`
- `sklearn`

---

## 📈 Expected Outcomes
- Determine if `GarageFinish` has a statistically significant effect on `SalePrice`.
- Identify which finish categories drive higher or lower sale prices.
- Build a regression model capable of predicting `SalePrice` accurately and interpretable by business or housing market analysts.

---

## 🧾 Author
**Baha Aburaiah**  
AI & Data Science Track  
2025 – Statistics & Regression Project
