#⚡EnerGenius : Appliance Energy Consumption Prediction

EnerGenius is a supervised machine learning project aimed at predicting the **energy consumption of appliances** using environmental and weather-related sensor data.

## 📘 Project Overview

The main steps of the notebook are:

- Dataset exploration and feature explanation
- Data cleaning and preprocessing (e.g., date decomposition, outlier handling)
- Exploratory visualization (e.g., temperature vs energy consumption)
- Training and evaluating multiple regression models
- Comparing model performance based on R² score

## 📊 Dataset Description

The dataset includes indoor environmental features (e.g., temperature, humidity per room) and weather data collected from the Chievres meteorological station, such as:

- `T1` to `T9`, `RH_1` to `RH_9`: Indoor temperature and humidity (kitchen, living room, bedrooms, etc.)
- `T_out`, `RH_out`, `Windspeed`, `Visibility`, `Press_mm_hg`, `Tdewpoint`: External weather conditions
- `rv1`, `rv2`: Random variables without dimension
- `Date`: Timestamp (later decomposed and dropped)
- Target: `Appliances` (energy consumption in Wh)

## ⚙️ Models Implemented

The following regression models were tested:

- Linear Regression
- Lasso Regression
- Gradient Boosting Regressor
- Random Forest Regressor
- XGBoost (XGBRegressor)
- k-Nearest Neighbors (KNN)

## 📈 Evaluation Metric

The main evaluation metric used is the **coefficient of determination (R²)**.

> ⚠️ Most models achieved relatively low R² scores (below 0.5), indicating limited predictive power for this dataset. KNN performed slightly better than others.

## 📦 Requirements

Install dependencies with:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn xgboost
```

## 📁 Usage

- Clone the repository or download the notebook.
- Open `Projet.ipynb` in Jupyter Notebook or JupyterLab.
- Run the cells step-by-step to follow the analysis and model training.

## 📝 License

This project is open-source and available under the [MIT License](https://opensource.org/licenses/MIT).
---
Feel free to contribute, modify the code, or apply it to other datasets for experimentation.
