# 🍽️ Tipping Behavior Analysis using Seaborn's `tips` Dataset

## 📌 Project Overview

This project investigates restaurant tipping behavior using the `tips` dataset from the Seaborn library. The goal is to simulate a real-world analytics engagement: from formulating a business question, analyzing data through Python and statistics, and ending with insights and recommendations that can inform business decisions.

---

## 🎯 Business Objective

> **How do factors such as day of the week, time of day, and smoker status affect total bill amounts and tipping behavior?**

Restaurants rely on tips for staff income and performance metrics. Understanding what influences tipping can guide staffing, promotions, and operational focus.

---

## 🧾 Dataset Description

The dataset used is Seaborn’s built-in `tips` dataset, which includes 244 observations with the following fields:

| Column       | Description                              |
|--------------|------------------------------------------|
| `total_bill` | Total bill (in USD)                      |
| `tip`        | Tip amount (in USD)                      |
| `sex`        | Gender of the customer                   |
| `smoker`     | Whether the customer is a smoker         |
| `day`        | Day of the week (Thur, Fri, Sat, Sun)    |
| `time`       | Time of day (Lunch or Dinner)            |
| `size`       | Number of people at the table            |

---

## 🧪 Tools & Technologies Used

- Python
- Jupyter Notebook
- Libraries:
  - `pandas`, `numpy`
  - `matplotlib`, `seaborn`
  - `scipy.stats`, `statsmodels`
- Statistical Techniques:
  - Descriptive statistics
  - Normality & variance tests
  - Independent t-test
  - ANOVA
  - Tukey’s HSD

---

## 🧹 Data Preprocessing

- Verified data types and value ranges.
- Checked for missing values (none found).
- No duplicates present.
- Outliers in total_bill and tip were explored via boxplots.
- New columns created (e.g., tip percentage).

---

## 📊 Exploratory Data Analysis (EDA)

- **Distribution Analysis:** Histograms and KDEs for `total_bill` and `tip`.
- **Categorical Insights:**
  - Boxplots by `day`, `time`, `smoker`, and `sex`.
  - Violin plots to visualize distribution overlaps.
- **Correlation Matrix:** Heatmap of numeric correlations.
- **Visual Highlights:**
  - Average tips are higher at dinner.
  - Weekend (Sat/Sun) has higher bills and tips.
  - Non-smokers tend to tip slightly more.

---

## 📈 Inferential Statistical Analysis

- **Shapiro-Wilk Test**: Used to test normality for `tip` and `total_bill`.
- **Levene's Test**: Used to check for equal variance across groups.
- **Independent T-Test**:
  - Compared tips of smokers vs. non-smokers.
- **ANOVA**:
  - Tested tip differences across `day`.
- **Tukey’s HSD**:
  - Identified which specific days differ in tip amount.

---

## 📌 Key Observations

- 💡 **Dinner vs. Lunch**:
  - Dinner has significantly higher bills and tips.
- 🚬 **Smoker Status**:
  - Non-smokers leave higher average tips (statistically significant).
- 📅 **Day of Week**:
  - Sunday and Saturday have the highest tip and bill averages.
  - Statistically significant differences in tipping behavior across days.
- 👥 **Table Size**:
  - Tipping percentage slightly decreases as table size increases.

---

## ✅ Recommendations

1. **Staff Optimization:**
   - Assign more experienced servers during weekend dinners.
2. **Customer Targeting:**
   - Run loyalty programs during weekdays (e.g., Thursday) to boost low-tip days.
3. **Smoking Policy:**
   - Encourage seating in non-smoking zones if tips are a KPI.
4. **Upselling Strategy:**
   - Focus on smaller tables for upselling drinks/desserts since they yield better tips proportionally.

---

## ⚠️ Limitations

- Small dataset (only 244 rows).
- No demographic info (age, income, etc.).
- Observational, not experimental — cannot infer causation.
- Seaborn’s `tips` dataset may not reflect modern tipping behaviors or cultural norms.

---

## 🔮 Future Work

- Build a regression model to predict tip amounts based on multiple factors.
- Add external datasets (e.g., economic status, location).
- Conduct cluster analysis to identify customer tipping profiles.
- Develop a dashboard using Tableau or Power BI for interactive exploration.

---

## 📁 Project Structure

tips-analysis-project/
│
├── tips_analysis.ipynb 
├── README.md 
├── visuals/ 
├── requirements.txt  


---

## 🚀 How to Run This Project

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/tips-analysis-project.git
   cd tips-analysis-project
   
2. pip install -r requirements.txt
   
3. jupyter notebook tips_analysis.ipynb

---

## 🧑‍💻 Author

Vedanshi Shukla
📧 vedanshishuklas2001@gmail.com
🔗 [LinkedIn ](http://linkedin.com/in/vedanshi-shukla) | [GitHub](https://github.com/Vedanshi-shukla2001) 
   


