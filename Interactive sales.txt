#1.Importing Libraries and Loading data set

import pandas as pd
df = pd.read_csv("Interactive sales.csv", encoding='latin1')
print(df.head())
print(df["Order Date"].head(10))

#2.Exploratary Data Analysis

total_sales = df["Sales"].sum()
total_profit = df["Profit"].sum()
total_orders = df["Order ID"].nunique()
print("Total Sales:", total_sales)
print("Total Profit:", total_profit)
print("Total Orders:", total_orders)

