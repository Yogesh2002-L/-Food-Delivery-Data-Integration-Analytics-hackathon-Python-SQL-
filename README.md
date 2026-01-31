# Food-Delivery-Data-Integration-Analytics-hackathon-Python-SQL

# 📌 Project Overview

This project focuses on data engineering + analytics for a food delivery platform.
The goal is to build a single clean master dataset by integrating multiple data sources and then perform analysis on:

✅ Order trends over time
✅ User behavior patterns
✅ City-wise and cuisine-wise performance
✅ Membership impact (Gold vs Regular)
✅ Revenue distribution and seasonality

# 🎯 Objectives

# 1. Data Integration (ETL)

Load multiple datasets:
orders.csv → transactional order data
users.json → user master data
restaurants.sql → restaurant master data
Perform Left Join to ensure all order records are retained:
orders.user_id → users.user_id
orders.restaurant_id → restaurants.restaurant_id
Export final dataset:

✅ final_food_delivery_dataset.csv

# 2. Business Insights (Analytics)
Identify top performing cities and cuisines
Study user spending patterns
Evaluate membership effect on revenue
Determine high-value restaurants and rating impact

# 🧾 Dataset Details
✅ Input Files
File Name	Type	Description
orders.csv	CSV	Order-level transactional dataset
users.json	JSON	User information + membership status
restaurants.sql	SQL Script	Restaurant metadata like cuisine & rating

# ✅ Final Output File
File Name	Type	Description
final_food_delivery_dataset.csv	CSV	Integrated dataset (orders + users + restaurants)
🧩 Data Integration Logic

# 🔗 Join Keys Used
Orders + Users: user_id
Orders + Restaurants: restaurant_id

# ✅ Join Type
Left Join
Keeps all orders even if user/restaurant details are missing
Missing values become NaN

# 🛠️ Tech Stack
Python
Pandas
Matplotlib

SQLite (in-memory DB)

Jupyter Notebook / VS Code
