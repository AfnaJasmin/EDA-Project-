# EDA-Project-

# 🚦 Indian Road Accident Exploratory Data Analysis (EDA) Project
## 📌 Project Overview

This project performs Exploratory Data Analysis (EDA) on an Indian Road Accident dataset (2022–2025) to understand accident patterns, risk factors, and trends over time.

The main objective of this project is to:

Understand the structure and quality of the dataset
Clean and preprocess raw data
Perform univariate and bivariate analysis
Conduct statistical testing
Perform time-based analysis
Engineer new features
Generate meaningful insights for road safety

## 📂 Dataset Description

The dataset contains information about road accidents across different cities and states in India.
Each row represents one accident record.

## 🔑 Key Columns
accident_id – Unique accident identifier
city – City where accident occurred
state – State of accident
latitude, longitude – Location coordinates
date, time – Date and time of accident
hour – Hour of accident
day_of_week – Day of occurrence
is_weekend – Weekend indicator
weather – Weather condition
visibility – Visibility condition
traffic_density – Traffic level
cause – Cause of accident
accident_severity – Severity (minor, major, fatal)
vehicles_involved – Number of vehicles
casualties – Number of casualties
risk_score – Risk level of accident


## 🏗️ Project Structure
eda-project/
│
├── data/
│   ├── raw/
│   ├── interim/
│   └── processed/
│
├── notebooks/
│   ├── 01_data_overview.ipynb
│   ├── 02_cleaning_preprocessing.ipynb
│   ├── 03_univariate_bivariate_eda.ipynb
│   └── 04_stats_time_features_final_insights.ipynb
│
├── reports/
│   └── figures/
│
├── README.md
└── requirements.txt

🧹 Data Cleaning
Handled missing values in the festival column
Converted the date column to datetime format
Removed duplicate records
Standardized categorical variables
Performed outlier detection using IQR (no significant outliers found)
Saved the cleaned dataset


📊 Exploratory Data Analysis

🔹 Univariate Analysis
Distribution of casualties
Vehicles involved analysis
Accident severity distribution
Weather condition distribution


🔹 Bivariate Analysis
Vehicles involved vs casualties
Accident severity vs casualties
Weather vs accident severity
Correlation heatmap


📈 Statistical Tests

T-test → Compared casualties between weekend and weekday accidents
ANOVA → Compared casualties across accident severity levels
Chi-square test → Analyzed relationship between weather and accident severity

These tests helped validate patterns statistically.


⏳ Time-Based Analysis
Extracted and analyzed:

Year
Month
Hour
Day of week

👉 This helped identify accident trends and peak accident periods.


🛠️ Feature Engineering
Created new features:

year
month
day
is_weekend_flag

👉 These features improved analysis and pattern detection.

🔍 Key Insights
Most accidents are minor with fewer casualties
Accidents increase during peak traffic hours
Accident patterns vary across months and years
Accident severity strongly impacts casualties
Multi-vehicle accidents lead to higher casualties
Weather conditions influence accident severity
Weekday accidents are more frequent
Regional differences exist in accident severity
Time-based trends highlight peak accident periods
Feature engineering improved analysis depth
🧰 Tools Used
Python
Pandas
NumPy
Matplotlib
Seaborn
SciPy
Jupyter Notebook
Git & GitHub
▶️ How to Run the Project
Clone the repository

Install required libraries:

pip install -r requirements.txt
Run notebooks in order:
Day 1 → Day 2 → Day 3 → Day 4
📁 Final Dataset

The final cleaned dataset is available at:

data/processed/final_cleaned_day4.csv
📌 Conclusion

This project demonstrates a complete EDA workflow including data cleaning, visualization, statistical testing, and feature engineering.

It provides meaningful insights into accident patterns and risk factors, which can help improve road safety awareness and decision-making.
