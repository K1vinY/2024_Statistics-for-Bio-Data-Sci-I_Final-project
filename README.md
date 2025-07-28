# 2024_Statistics-for-Bio-Data-Sci-I_Final-project

# 🧠 Does Wealth Protect Emotional Well-being?  
**An Analysis Using NHANES Data in R**

## 📌 Project Overview

This project investigates whether **income level** is significantly associated with emotional and physiological indicators of well-being. Inspired by personal experiences and social observations of class-based stress, the study aims to answer:

> **Do people from high-income families experience better emotional health?**

Using publicly available NHANES data, this project evaluates how income correlates with:
- Sleep hours
- Systolic blood pressure
- Marijuana use
- Self-reported depression levels

---

## 🎯 Research Question & Hypothesis

The hypothesis is that individuals from higher-income households experience:
- **Better sleep**
- **Healthier blood pressure**
- **Less marijuana use**
- **Lower likelihood of depression**

These outcomes are assumed to result from reduced stress levels associated with financial security.

---

## 📊 Data Source

- **Dataset:** [NHANES – National Health and Nutrition Examination Survey](https://www.cdc.gov/nchs/nhanes/index.htm)
- **Variables Used:**
  - `HHIncome`: Household income category
  - `SleepHrsNight`: Average hours of sleep per night
  - `BPSysAve`: Systolic blood pressure average
  - `RegularMarij`: Regular marijuana usage (Yes/No)
  - `Depressed`: Days felt down/depressed/hopeless

---

## 🛠️ Tools & Libraries

Project is written in **R (Quarto `.qmd` format)** using the following packages:

- `tidyverse` / `dplyr` – Data manipulation
- `ggplot2` – Data visualization (histograms, box plots, bar charts)
- `stats` – ANOVA, Chi-square test
- `NHANES` – Data source package

---

## 🔬 Methodology

### 🧹 Data Cleaning
- Removed missing values using `na.omit()`
- Categorical and numerical variables handled separately

### 📈 Visualizations
- **Histograms:** Income distribution, Depression levels
- **Box plots:** Sleep hours, Blood pressure
- **Bar charts:** Marijuana usage
- All visuals annotated and interpreted

### 📊 Statistical Analysis
- **ANOVA:** Assessed impact of income on numeric variables
  - Post-hoc: Tukey's HSD test
- **Chi-Square Tests:** Income vs. categorical outcomes (marijuana, depression)

---

## ✅ Key Findings

- Higher-income individuals:
  - Sleep significantly longer (p < 0.001)
  - Have lower systolic blood pressure (p < 0.001)
  - Are less likely to use marijuana regularly (p ≈ 0.0001)
  - Are less likely to report feelings of depression (p < 2.2e-16)
- **All null hypotheses were rejected**, suggesting strong relationships between income and health/emotional indicators.

---

## 📌 Conclusion

The study confirms that income is significantly associated with **both emotional and physiological well-being**. Wealth appears to offer protective effects, reducing stress-related symptoms and promoting healthier lifestyles.

---

## 📚 References

1. Szabó, M. (2011). *The emotional experience associated with worrying: anxiety, depression, or stress?*  
2. Martire et al. (2020). *Stress & sleep: A relationship lasting a lifetime.*  
3. Gasperin et al. (2009). *Effect of psychological stress on blood pressure increase.*  
4. Pomerleau & Pomerleau (1991). *Research on stress and smoking.*  
5. Kim et al. (2019). *The relationship between sleep duration and perceived stress.*  
6. Flint et al. (2019). *Effect of blood pressure on cardiovascular outcomes.*

---

**Author:** Kevin Yu  
**Language:** R with Quarto (`.qmd`)  
**Data Size:** ~10,000 rows / 75 variables  
