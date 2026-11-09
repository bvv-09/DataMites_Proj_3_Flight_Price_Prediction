# ✈️ Flight Fare Prediction using Machine Learning

##  Project Overview

The Flight Fare Prediction project aims to predict airline ticket prices based on various factors such as airline, source, destination, journey date, departure time, arrival time, flight duration, and number of stops.

This project uses machine learning regression algorithms to identify patterns in historical flight data and estimate flight ticket prices.

The primary objective is to build, evaluate, and compare different regression models to determine their effectiveness in predicting flight fares.

##  Problem Statement

Flight ticket prices fluctuate depending on several factors, including airline, route, travel date, departure time, and number of stops.

The objective of this project is to develop a machine learning model that can predict flight ticket prices using these features.

**Target Variable:** `Price`

**Problem Type:** Supervised Machine Learning – Regression

##  Dataset Description

The dataset contains flight-related information with the following features:

| Feature | Description |
|---|---|
| Airline | Name of the airline |
| Date_of_Journey | Date of the journey |
| Source | Departure city |
| Destination | Arrival city |
| Route | Flight route |
| Dep_Time | Departure time |
| Arrival_Time | Arrival time |
| Duration | Total flight duration |
| Total_Stops | Number of stops |
| Additional_Info | Additional flight information |
| Price | Flight ticket price (Target Variable) |

##  Technologies & Libraries Used

- **Programming Language:** Python
- **Data Manipulation:** Pandas, NumPy
- **Data Visualization:** Matplotlib, Seaborn
- **Machine Learning:** Scikit-learn
- **Development Environment:** Google Colab 

##  Project Workflow

### 1. Data Understanding
- Examined dataset dimensions, data types, and statistical summaries.
- Identified numerical and categorical variables.
- Analyzed feature distributions and unique values.

### 2. Data Cleaning & Preprocessing
- Handled missing values and duplicate records.
- Converted journey dates into numerical day and month features.
- Extracted departure and arrival hours.
- Converted flight duration into minutes.
- Extracted numerical values from the number of stops.
- Removed less useful features such as Route and Additional_Info.

### 3. Exploratory Data Analysis (EDA)
- Analyzed flight price distribution.
- Compared average prices across airlines.
- Examined the relationship between flight duration and ticket prices.
- Studied price variations based on the number of stops.
- Analyzed average prices across source-destination combinations.
- Investigated the relationship between departure time and flight prices.

### 4. Hypothesis Testing
Performed statistical hypothesis testing to investigate:
- The relationship between flight duration and ticket price using Pearson Correlation.
- Differences in average flight prices across stop categories using One-Way ANOVA.

### 5. Feature Engineering & Data Preprocessing
- Applied One-Hot Encoding to categorical features such as Airline, Source, and Destination.
- Separated independent variables (X) and the target variable (y).
- Split the dataset into training and testing sets.
- Applied Standardization using StandardScaler to selected numerical features for Linear Regression and KNN.
- Maintained unscaled data for Random Forest.

### 6. Model Implementation

Implemented and compared the following regression algorithms:

**1. Linear Regression**
- Used as the baseline regression model.
- Established an initial benchmark for model performance.

**2. K-Nearest Neighbors (KNN) Regressor**
- Used a distance-based regression approach.
- Applied feature scaling before model training.

**3. Random Forest Regressor**
- Used an ensemble-based tree regression approach.
- Trained using unscaled features.

### 7. Cross-Validation & Hyperparameter Tuning
- Applied 5-Fold Cross-Validation.
- Used GridSearchCV for hyperparameter tuning.
- Identified suitable hyperparameter combinations for each model.
- Evaluated tuned models against their initial versions.

### 8. Model Evaluation

Evaluated model performance using the following regression metrics:

- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- R² Score

##  Key Learnings

- Understanding and preprocessing real-world flight fare data.
- Performing exploratory data analysis and interpreting visualizations.
- Applying statistical hypothesis testing.
- Handling categorical variables using One-Hot Encoding.
- Understanding feature scaling and its importance across different algorithms.
- Implementing multiple regression algorithms.
- Applying cross-validation and hyperparameter tuning.
- Comparing machine learning models using regression evaluation metrics.

##  Conclusion

This project provided practical experience in developing an end-to-end machine learning regression workflow, starting from data understanding and preprocessing to model implementation, evaluation, and hyperparameter optimization.

By comparing Linear Regression, KNN Regressor, and Random Forest Regressor, the project explores different approaches to predicting flight ticket prices and evaluating their performance.

---

**Project Category:** Machine Learning | Regression | Predictive Modeling

**Author:** Vamsi Vasu Bokinala
