# 📊 Sales Dashboard with EDA (Power BI + Python)

## 📌 Objective

Analyze and visualize sales performance using Python (EDA) and Power BI dashboard.

---

## 🛠 Tools Used

* Python (Pandas, Matplotlib, Seaborn)
* Power BI
* Excel / CSV

---

## 🔍 Exploratory Data Analysis (Python)

Performed using Python to understand data before visualization:

* Data Cleaning (handled missing values)
* Converted date columns
* Checked data types
* Summary statistics
* Sales & Profit analysis
* Top products identification

### ▶ Sample Code

```python
import pandas as pd

df = pd.read_csv("sales_data.csv")

df["Order Date"] = pd.to_datetime(df["Order Date"], dayfirst=True)

print(df.describe())

top_products = df.groupby("Product Name")["Sales"].sum().sort_values(ascending=False).head(10)

print(top_products)
```

---

## 📊 Power BI Dashboard Features

* 📌 KPIs:

  * Total Sales
  * Total Profit
  * Total Orders

* 📈 Visuals:

  * Sales by Region
  * Sales by Category
  * Top 10 Products

* 🎯 Filters:

  * Region
  * Category
  * Date

---

## 📈 Key Insights

* Technology category generates highest revenue
* Some products have high sales but low profit
* Discounts reduce profit margins
* Regional performance varies significantly

---

## 📂 Files in Repository

* `Sales_Dashboard.pbix`
* `sales_data.csv`
* `eda_analysis.py`

---

## 🚀 How to Use

1. Run Python file for EDA:

   ```bash
   python eda_analysis.py
   ```
2. Open `.pbix` file in Power BI
3. Explore dashboard with filters

---

