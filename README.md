# 🚕 TripFare: Predicting Urban Taxi Fare with Machine Learning

This project aims to build a predictive model that estimates taxi fares using real-world trip data. It involves data preprocessing, feature engineering, model training, evaluation, and deployment using Streamlit.

---

## 📌 Project Objective

To enhance fare estimation systems for urban mobility by predicting the total trip fare based on various ride-related features such as distance, time, passenger count, and more.

---

## 🧠 Problem Type

- **Machine Learning Task**: Supervised Regression
- **Target Variable**: `total_amount`

---

## 🗂 Dataset

- **Source**: [Google Drive Link](https://drive.google.com/file/d/1VUb9ucTsroGDBOPcwpOfXwzDi-rd4wqQ/view?usp=sharing)
- **Format**: CSV
- **Records**: NYC Yellow Taxi trip data

---

## 📊 Features Used

- `trip_distance`: Calculated using Haversine formula from GPS coordinates  
- `passenger_count`: Number of passengers  
- `pickup_hour`: Hour of the day  
- `is_weekend`: Whether the trip occurred on weekend  
- `is_night`: Flag for night rides (10 PM – 5 AM)

---

## 📈 Project Workflow

### 1️⃣ Data Collection
- Load CSV using `pandas`

### 2️⃣ Data Cleaning
- Remove nulls and irrelevant entries

### 3️⃣ Feature Engineering
- Extract and derive features such as time, distance, night/weekend flags

### 4️⃣ Exploratory Data Analysis (EDA)
- Understand relationships between fare and other features using plots

### 5️⃣ Model Building
- Models Used:
  - Linear Regression
  - Lasso & Ridge
  - Random Forest
  - Gradient Boosting
- Evaluation Metrics:
  - R² Score
  - RMSE
  - MAE

### 6️⃣ Hyperparameter Tuning
- `GridSearchCV` or `RandomizedSearchCV` on best model

### 7️⃣ Streamlit Deployment
- Build a user-friendly UI where users can input trip details and get fare predictions

---

## 💻 Streamlit Interface

> A simple web interface for users to:
- Input trip details (distance, hour, passengers, etc.)
- Click **Predict** and get the estimated fare
- Powered by the trained RandomForest model saved as `model.pkl`

---

## 🛠 Tech Stack

- **Languages**: Python
- **Libraries**: pandas, numpy, matplotlib, seaborn, scikit-learn, streamlit
- **Deployment**: Streamlit App

Process: 

Python notebook with:
EDA
Cleaned and feature-engineered data
Model evaluation and comparison
Trained .pkl model
Streamlit app UI

