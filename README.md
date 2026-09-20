<img width="1361" height="765" alt="screencapture-51751a8aa776b466c2-gradio-live-2026-09-20-14_24_49" src="https://github.com/user-attachments/assets/169cb804-4455-4dd4-a5f8-a027f1f70834" />
<img width="1361" height="765" alt="screencapture-51751a8aa776b466c2-gradio-live-2026-09-20-14_32_09" src="https://github.com/user-attachments/assets/94befc50-ef71-4e1c-aa68-e3444c7cb63f" />
<img width="1361" height="765" alt="screencapture-51751a8aa776b466c2-gradio-live-2026-09-20-14_37_03" src="https://github.com/user-attachments/assets/1ac4c535-c9e0-424d-8286-aea7cf7aa63a" />
v
# 🚲 Bike Rental Demand Prediction

A Machine Learning project developed during my **Big Brains AI/ML Internship** to predict bike rental demand using historical weather, seasonal, and time-based data.

## 📌 Project Overview

Bike rental demand changes according to factors such as **hour of the day, season, weather, temperature, humidity, and working days**.

The goal of this project is to build a regression model that predicts the **total number of rented bikes (`cnt`)** based on these conditions.

## 🎯 Objective

Build an end-to-end Machine Learning workflow for:

- Dataset collection and exploration
- Data cleaning and preprocessing
- Feature engineering
- Exploratory Data Analysis (EDA)
- Linear Regression model training
- Model evaluation
- Bike demand prediction

## 📊 Dataset

**Dataset:** UCI Bike Sharing Dataset  
**Dataset Type:** Hourly Bike Rental Data  
**Records:** 17,379  
**Target Variable:** `cnt` — Total number of rental bikes

The project uses the hourly dataset because it includes the **hour (`hr`)** feature required for time-based demand analysis.

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Jupyter Notebook / Google Colab
- Git & GitHub
- Gradio

## 🔄 Project Workflow

```text
Dataset Collection
        ↓
Data Exploration
        ↓
Data Cleaning & Preprocessing
        ↓
Feature Engineering
        ↓
Exploratory Data Analysis
        ↓
Train/Test Split
        ↓
Linear Regression
        ↓
Model Training
        ↓
Model Evaluation
        ↓
Bike Demand Prediction
```

## 🧹 Data Preprocessing

The dataset was prepared by:

- Checking missing values
- Checking and removing duplicate records
- Converting date information
- Creating time-based features
- Creating cyclical hour features
- Encoding categorical variables
- Removing unnecessary identifier columns
- Removing `casual` and `registered` to avoid target leakage
- Preparing the final dataset for Machine Learning

## 📈 Exploratory Data Analysis

The project analyzes rental demand according to:

- Hour of the day
- Season
- Weather conditions
- Working days
- Temperature
- Other time and environmental factors

EDA was used to identify patterns and understand which features may influence bike rental demand.

## 🤖 Machine Learning Model

### Linear Regression

Since bike rental demand is a numerical value, the project uses **Linear Regression** as the required regression model.

Dataset split:

- **Training:** 80%
- **Testing:** 20%

Training samples: **13,903**  
Testing samples: **3,476**  
Features used: **58**

## 📊 Model Evaluation

The trained Linear Regression model achieved:

| Metric | Result |
|---|---:|
| MAE | 74.09 |
| MSE | 10086.62 |
| RMSE | 100.43 |
| R² Score | 0.6815 |

These metrics were calculated on the test dataset.

## 🚲 Prediction Application

A simple prediction interface was created using **Gradio**.

Users can provide conditions such as:

- Year
- Season
- Month
- Hour
- Holiday
- Weekday
- Working Day
- Weather
- Temperature
- Feeling Temperature
- Humidity
- Wind Speed
- Day

The application then generates the predicted bike rental demand.

## 📁 Project Structure

```text
Bike_prediction_project-Internship/
│
├── Bike_Rental_Demand_Prediction.ipynb
├── README.md
└── ...
```

## ▶️ How to Run

1. Clone the repository:

```bash
git clone https://github.com/mudassar2224/Bike_prediction_project-Internship.git
```

2. Open the Jupyter Notebook:

```text
Bike_Rental_Demand_Prediction.ipynb
```

3. Run the notebook cells in order.

The notebook downloads the UCI Bike Sharing Dataset directly and performs the complete Machine Learning workflow.

## 📌 Key Learning Outcomes

Through this project, I practiced:

- Pandas and NumPy
- Data Cleaning
- Feature Engineering
- Categorical Encoding
- Time Feature Processing
- Exploratory Data Analysis
- Data Visualization
- Train/Test Splitting
- Linear Regression
- Model Evaluation
- ML Prediction Interfaces
- GitHub Project Documentation

## 🚀 Future Improvements

Possible future improvements include:

- Trying additional regression algorithms
- Hyperparameter tuning
- Improving prediction accuracy
- Better handling of demand patterns
- Advanced feature engineering
- Improved deployment of the prediction application

## 👨‍💻 Internship

**Program:** Big Brains AI/ML Internship  
**Project:** Bike Rental Demand Prediction  
**Developer:** Muhammad Mudassar

---

⭐ This project represents my practical learning and hands-on work during my AI/ML internship.
