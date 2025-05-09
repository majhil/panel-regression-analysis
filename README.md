# Panel Regression Analysis on Life Expectancy

This project performs a panel data regression analysis to examine the impact of various socioeconomic and environmental factors on life expectancy across countries. The analysis includes both developed and developing nations using fixed effects, random effects, and dynamic panel data models.

---

## 📁 Files

- `panelRegressionAnalysis.ipynb`: Main analysis notebook.
- `blueprint 3.1.csv`: Full dataset of countries.
- `developed.csv`: Dataset of developed countries.
- `developing.csv`: Dataset of developing countries.

---

## 📊 Data Description

Each dataset includes the following variables:

- `Code`, `Year`: Country identifier and year.
- `Life_Expectancy`: Dependent variable.
- `Annual_CO2_emissions`
- `GDP_per_capita`
- `Infant_Mortality_Rate`
- `Military_Expenditure`
- `health_expenditure_per_capita`

---

## 🧪 Methodology

1. **Descriptive Analysis**
   - Summary statistics and correlation matrix via heatmap.

2. **Panel Data Models**
   - Pooled OLS
   - Fixed Effects (FE)
   - Random Effects (RE)
   - Hausman Test (FE vs RE)

3. **Diagnostics**
   - Breusch-Pagan Test for heteroskedasticity
   - Ramsey RESET Test
   - VIF for multicollinearity

4. **Dynamic Panel Regression**
   - GMM using `pydynpd` to control for endogeneity and dynamic effects.

---

## 🛠 Requirements

Install dependencies using pip:
```bash
pip install numpy==1.24.3 pandas matplotlib seaborn statsmodels linearmodels arch pydynpd
