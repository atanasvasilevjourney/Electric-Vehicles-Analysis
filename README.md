 🚗 Electric Vehicle Population Analysis

**Author:** Atanas Vasilev  
**Project Type:** End-to-End Data Analytics & Machine Learning Project  
**Tools Used:** Power BI, Python (Pandas, Scikit-learn), SQL

---

## 📊 Overview

This project analyzes the population, characteristics, and trends of Electric Vehicles (EVs), aiming to extract actionable insights through:

- Data Profiling
- Hypothesis Testing
- Regression Modeling
- EV Segmentation via Clustering
- Interactive Power BI Dashboard

---

## 📁 Files in This Repository

| File | Description |
|------|-------------|
| `EV_PowerBI.pbix` | Interactive Power BI report visualizing EV metrics. |
| `Electric_Vehicle__Population_Analysis.pptx` | Executive presentation summarizing analysis and findings. |
| `Electric_Vehicles_Data_Dictionary.docx` | Definitions of all columns and data sources used. |
| `Electric_Vehicles_Python_All.ipynb` | Full Python workflow: profiling, statistical tests, regression, clustering. |
| `SQL_EVs.txt` | SQL queries used for filtering and preprocessing raw data. |

---

## 🔍 Key Analytical Steps

### 1. 📈 Data Profiling
Performed using Python (Pandas and Matplotlib/Seaborn). Outliers, null values, and distributions were assessed.

### 2. 📊 Power BI Dashboard
Visualizes:
- EV distribution by year and type.
- Top manufacturers and models.
- MSRP vs. Electric Range scatter plots.

**Calculated Fields & DAX Measures** used to derive KPIs.

### 3. 📐 Hypothesis Testing

**Question:**  
> Do Clean Alternative Fuel Eligible vehicles have significantly higher electric ranges?

- Performed using t-tests.
- Result: ✅ Statistically significant difference observed.

### 4. 📉 Regression Analysis

**Question:**  
> Is there a positive relationship between MSRP and Electric Range?

- Used Linear Regression in Python.
- Result: 📈 Positive correlation found, but with variability among manufacturers.

### 5. 🧠 Machine Learning Models

#### a. Supervised: Linear Regression
- Target: `Electric Range`
- Predictors: `MSRP`, `Vehicle Type`, `Eligibility`, etc.

#### b. Unsupervised: K-Means Clustering
- Segmented EVs by `MSRP`, `Range`, `Class`, and `Manufacturer`.
- Visualized clusters and buyer segments.

---

## 💡 Business Insights

- **High-Range EVs** tend to be luxury models with higher MSRPs.
- **Clean Alternative Fuel Eligibility** correlates with greater range.
- **K-Means clustering** helps identify market segments (budget vs. premium EVs).
- **Top Manufacturers**: Tesla dominates long-range category; Nissan & Chevrolet lead economy segment.

---

## 📌 How to Run This Project

1. **Power BI**  
   Open `EV_PowerBI.pbix` with Power BI Desktop.

2. **Python Notebook**  
   Install required packages with:
   ```bash
   pip install -r requirements.txt
