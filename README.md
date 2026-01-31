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


# 📊 Analysis & Insights
# ✅ 1. Order Trends Over Time
Month-wise order coun
Month-wise revenue growth
Quarterly revenue peak analysis

# ✅ 2. User Behavior Patterns
Top active users
High spenders
Average order value per user

# ✅ 3. City-wise and Cuisine-wise Performance
Cities with maximum revenue
Top cuisines by revenue
Cuisine AOV (average order value)

# ✅ 4. Membership Impact (Gold vs Regular)
Order share by membership
Revenue contribution by membership
Gold vs Regular spending distribution

# ✅ 5. Revenue Distribution & Seasonality
Histogram distribution of revenue
Seasonality analysis by month & quarter

# ✅ Key Learnings
Practical experience in ETL pipeline creation
Handling multiple data formats (CSV, JSON, SQL)
Real-world data merging logic (joins)
Business analytics and visualization
Insights generation for decision-making

# 🏁 Conclusion
This project demonstrates a full cycle of:
✅ data ingestion → ✅ integration → ✅ transformation → ✅ analysis → ✅ insights.
It is useful for roles like:
Data Analyst
Data Engineer (Beginner)
Business Analyst
Python Developer
