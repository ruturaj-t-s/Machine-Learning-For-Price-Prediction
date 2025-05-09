# 🏡 Airbnb Price Prediction and Insights

## 📌 Project Overview

This project applies **Machine Learning** to predict Airbnb listing prices based on various features such as property type, room type, location, amenities, and host characteristics.\
The goal is not just accurate price prediction, but also uncovering insights that can help optimize pricing strategies for hosts and platforms.

---

## 🎯 Objectives

- Predict listing prices using regression models
- Analyze the impact of various listing attributes on price
- Perform Exploratory Data Analysis (EDA) and outlier detection
- Apply feature engineering to improve model performance
- Provide actionable insights for Airbnb hosts and analysts

---

## 📂 Dataset Summary

- **Rows:** 74,111  
- **Columns:** 29  
- **Key Features:**  
  - `property_type`, `room_type`, `neighbourhood`, `latitude`, `longitude`  
  - `accommodates`, `bathrooms`, `bedrooms`, `beds`, `price`  
  - `availability`, `review_scores_rating`, `host_listings_count`

---

## 🧪 Workflow

### 1. 📊 Exploratory Data Analysis (EDA)
- Visualized relationships between features and price
- Explored the impact of room type, property type, and neighborhood on pricing
- Plotted heatmaps, boxplots, and scatter plots
- Checked data types and structure
- Detected missing values and outliers

### 2. 🔍 Data Preprocessing and Manipulation
- Handled missing values and outliers using appropriate methods
- Converted price to numeric and cleaned currency formatting
- Dropped redundant or highly null columns
- Applied feature transformation methods


### 3. 🛠️ Feature Engineering
- Converted categorical variables using **One-Hot Encoding**
- Normalized/standardized numerical variables where needed
- Created new features such as:
  - `price_per_person = price / accommodates`
  - `is_superhost` from host metadata (if available)
- Removed skewed distributions using log transformation on price

### 4. 🤖 Model Building
- Trained and evaluated:
  - Linear Regression
  - Random Forest Regressor
  - Gradient Boosting Regressor
- Performance metrics:
  - RMSE (Root Mean Squared Error)
  - MAE (Mean Absolute Error)
  - R² Score

## 📊 Key Visualizations

- Correlation heatmap of numeric features  
- Boxplots of price by room/property type  
- Scatter plots: price vs. bedrooms, accommodates, etc
- Feature importance bar charts from ensemble models 
