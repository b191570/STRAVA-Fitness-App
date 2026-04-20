## Strava Fitness EDA Analysis

##  Project Overview
This project focuses on performing **Exploratory Data Analysis (EDA)** on fitness tracking data inspired by Strava. The objective is to analyze user activity patterns, identify trends, and generate actionable insights that can help improve user engagement, retention, and subscription conversion.

Strava is a fitness tracking platform that allows users to record physical activities such as running and cycling, analyze performance metrics, and interact with a community.

## Business Objectives

- Identify **user activity trends** to attract new users  
- Analyze behavior patterns to **increase subscription adoption**  
- Understand **fitness habits and engagement levels**  
- Extract insights to improve **user experience and retention**
- 
## Dataset Information

Multiple datasets were merged to create a unified dataset:
- Daily Activity Data  
- Calories Burned Data  
- Intensity Data  
- Steps Data  
- Sleep Data  
- Weight Log Data  

###  Final Dataset Summary

- **Total Rows:** 6,222  
- **Total Columns:** 39  
- **Unique Users:** 7  
- **Missing Values:** Present in sleep and weight-related columns (handled)  

## Data Preprocessing

Key steps performed:
- Merged multiple datasets using **Id + Date columns**
- Removed duplicate records  
- Handled missing values:
  - Replaced sleep-related nulls with `0`
  - Replaced categorical nulls with `"Missing"`
- Standardized column names  
- Ensured dataset is **analysis-ready**

## Exploratory Data Analysis (EDA)

The analysis follows the **UBM Rule**:
### 🔹 Univariate Analysis
- Distribution of steps, distance, calories  
- Sleep records and activity intensity patterns  
### 🔹 Bivariate Analysis
- Steps vs Calories  
- Distance vs Activity Date  
- Logged vs Tracked Distance  
### 🔹 Multivariate Analysis
- Correlation heatmaps  
- Pairplots for multiple features  

## Key Insights & Numerical Findings

###  Activity Insights
- Average daily steps ≈ **7,954 steps**
- Maximum recorded steps: **13,162**
- Most users fall within **6,000 – 14,000 steps range**
- Average distance covered ≈ **5.36 km**

### Calories & Activity
- Strong relationship between **steps and calories burned**
- Users with **low steps (0)** still show calorie burn → indicates passive activity

###  Sleep Analysis
- Average sleep duration ≈ **468 minutes (~7.8 hours)**
- Sleep records are limited → indicates **low tracking engagement**

### Distance Tracking
- Users track steps more consistently than distance
- Logged activity distance is often **lower than tracker distance**

### Correlation Insights
- **TotalSteps vs TotalDistance → 0.98 (very strong correlation)**
- **Moderate Activity vs Fair Activity → 0.97**
- **Very Active Minutes vs Distance → 0.88**

### Observed Issues
- Very small number of active users (**only 7 unique IDs**)  
- Weight & BMI data almost missing → not useful  
- Some duplicated/overlapping columns from merging  

## 📊 Visualizations Created

- Bar Charts (Steps, Distance, Sleep Records)  
- Pie Charts (Step Distribution)  
- Treemaps (Steps & Distance Frequency)  
- Histograms (Activity Metrics Distribution)  
- Stacked Bar Charts (Calories vs Steps)  
- Line Charts (Trend Analysis)  
- Correlation Heatmap  
- Pairplot  

## Business Recommendations

### Improve User Engagement
- Introduce **daily step challenges**
- Reward users for achieving milestones  

###  Increase Subscription Conversion
- Offer **discounts for active users**
- Introduce **premium analytics dashboards**

### Enhance Tracking Behavior
- Encourage users to log **distance + sleep consistently**
- Add **reminders and gamification features**

### Gamification Strategy
- Leaderboards and achievements  
- Weekly/monthly fitness challenges  
- Social sharing incentives  

## Conclusion

- Users are **consistent with step tracking**, but less engaged with sleep and weight tracking  
- Strong correlation between steps and distance validates **data reliability**  
- Engagement can be significantly improved through **gamification and incentives**  
- Strava can leverage these insights to **increase user retention and premium subscriptions**

## Tech Stack

- **Python**
- **Pandas, NumPy**
- **Matplotlib, Seaborn**
- **Plotly**
- **Scikit-learn**

## 🙌 Final Note

This project demonstrates how data-driven insights can help fitness platforms like Strava:
- Improve user engagement  
- Increase subscriptions  
- Deliver better personalized experiences  
