# AeroDataCompetition

### ✈️ Flight Price Prediction
#### 📌 Project Overview

This project predicts flight ticket prices for Indian domestic flights (March–June 2019) using Machine Learning.
We preprocess the dataset, engineer features, and train regression models to estimate flight prices based on various factors like airline, source, destination, duration, and stops.

---
### 🎯 Goal
Build a machine learning model to predict flight prices.

Perform feature engineering & preprocessing on categorical and time-based data.

Evaluate the model using MAE, RMSE, and R² Score.

---
#### 📊 Dataset

The dataset contains details of domestic flights:
- Airline – Name of the airline
- Date_of_Journey – Journey date
- Source & Destination – Boarding and arrival cities
- Dep_Time & Arrival_Time – Departure and arrival times
- Duration – Flight duration
- Total_Stops – Number of stops
- Price – Ticket price (Target variable)
- 🔗 Link: https://tinyurl.com/Aero-Data

---
#### ⚙️ Tech Stack

- Python 3
- pandas, numpy – Data preprocessing
- matplotlib, seaborn – Data visualization
- scikit-learn – ML models, pipelines, hyperparameter tuning
  
---
**🛠️ Steps Implemented**
1. Data Preprocessing

   - Converted Date_of_Journey, Dep_Time, Arrival_Time into day, month, hour, minute.
   - Encoded categorical variables (Airline, Source, Destination) using OneHotEncoder.
   - Dropped irrelevant columns (Route, Additional_Info).

2. Feature Engineering

   - Extracted time features.
   - Converted flight duration into minutes.
   - Handled categorical & numerical features using ColumnTransformer.

3. Model Training
   - Used RandomForestRegressor as baseline.
   - Applied GridSearchCV for hyperparameter tuning.

5. Model Evaluation

   - Final model metrics:
   - MAE: 587.56
   - RMSE: 1359.65
   - R² Score: 0.91 ✅

---
**🔮 Key Insights**

- Jet Airways Business has the highest average ticket price in the dataset.
- Price depends heavily on airline, duration, and number of stops.
