# Airline-Passenger-Satisfaction-Analysis

This project performs **Exploratory Data Analysis (EDA)** on the [Airline Passenger Satisfaction dataset](https://www.kaggle.com/datasets/teejmahal20/airline-passenger-satisfaction), aiming to uncover the patterns that influence customer satisfaction in commercial flights.

---

## Dataset Information

- **Source**: Kaggle – Airline Passenger Satisfaction
- **Rows**: ~103,000
- **Columns**: 25
- **Target Variable**: `satisfaction` (Satisfied / Neutral or Dissatisfied)

The dataset contains passenger information such as travel class, flight delays, and various ratings for inflight services.

---

## Project Objectives

- Identify and handle **missing values**
- Detect and analyze **outliers**
- Examine **data distribution** and **skewness**
- Visualize **numerical and categorical features**
- Analyze **feature correlations** and patterns
- Prepare the dataset for potential predictive modeling

---

## Key Steps & Methods

### 1. Statistical Summary
- Calculated `mean`, `median`, `std`, and quartiles for all numerical columns.
- Compared **mean vs. median** to identify skewness.

### 2. Missing Value Handling
- Only `Arrival Delay in Minutes` had missing values (310).
- Imputed using the **median (0.0)** due to right-skewed distribution.

### 3. Outlier Analysis
- Applied **IQR method** to detect outliers.
- Visualized outliers using **boxplots**.
- Observed high delay values in arrival/departure times.

### 4. Data Visualization
- Used **histograms**, **KDE plots**, and **countplots**.
- Created **pie charts** to show distribution of categorical values.
- Plotted **correlation heatmap** for numerical features.
- Listed feature pairs with correlation > 0.5.

---

## Key Findings

- Arrival and departure delays are highly correlated (r ≈ 0.96), indicating strong dependence.
- Most passengers experienced no arrival delays; data is strongly right-skewed.
- Service-related features such as Inflight Entertainment, Food, and Seat Comfort are interrelated.
- Business class passengers tend to give higher satisfaction ratings.
- Majority of dissatisfied customers had longer delays and lower ratings on service features.
  
---

## Tools Used

- Python (Pandas, NumPy)
- Seaborn & Matplotlib for visualization
- Jupyter / Kaggle Notebook environment




