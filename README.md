# 🌡️ Next Day Temperature Prediction  
Machine Learning Regression Models for Weather Forecasting

Predicting next-day temperature is essential for agriculture, environment monitoring, and climate analysis.  
This project builds machine learning models to forecast **Next Day Minimum (T_MIN)** and **Next Day Maximum (T_MAX)** temperatures using historical meteorological data from the UCI Bias Correction dataset.

---

## 📁 Dataset

**Source:** UCI Machine Learning Repository  
**Link:** https://archive.ics.uci.edu/ml/datasets/Bias+Correction+of+Numerical+Prediction+Model+Temperature+Forecast

**Details:**
- ~7,750 rows  
- 25 meteorological attributes  
- Includes atmospheric pressure, humidity, wind speed/direction, temperature readings  
- **Targets:** `Next_Tmin`, `Next_Tmax`  
- Dataset is loaded directly from URL — no local files required  

---

## 🧹 Data Cleaning & Preprocessing

- KNN imputation for missing values  
- Remove redundant columns and fix data types  
- Exploratory Data Analysis (EDA):  
  - Distribution plots  
  - Boxplots  
  - Correlation heatmap  
  - Pairplots  
- Standard scaling for numerical features  
- Feature selection using `SelectKBest`  
- PCA experiments for dimensionality reduction  

---

## 🤖 Machine Learning Models Used

Models evaluated for both `Next_Tmin` and `Next_Tmax`:

- Linear Regression  
- Random Forest Regressor  
- Gradient Boosting Regressor  
- KNN Regressor  
- Support Vector Regressor (SVR)  
- VotingRegressor (ensemble)

**Training Pipeline Includes:**
- Train/Test split  
- Standardization  
- Hyperparameter tuning using GridSearchCV  
- Evaluation using four metrics  

---

## 🧪 Evaluation Metrics

- R² Score  
- Mean Squared Error (MSE)  
- Mean Absolute Error (MAE)  
- Explained Variance Score  

### **Approximate Model Performance**

#### **T_MIN Prediction**
| Model | R² Score |
|-------|----------|
| Linear Regression | ~0.82 |
| Random Forest | ~0.84–0.85 |
| Gradient Boosting | ~0.83 |
| KNN | ~0.83 |
| SVR | ~0.85 |

#### **T_MAX Prediction**
| Model | R² Score |
|-------|----------|
| Random Forest | ~0.87 |
| Gradient Boosting | ~0.81 |
| KNN | ~0.90 |
| SVR | ~0.86 |

**KNN and SVR performed best overall.**

---

## 📊 Visualizations Included

- Distribution plots  
- Correlation heatmap  
- Boxplots for outlier detection  
- Model comparison charts  
- PCA variance graph  
- Learning curves  

---

## 📂 Project Structure

next-day-temperature-prediction/
│
├── README.md
├── requirements.txt
├── .gitignore
│
├── notebooks/
│ └── next_day_temperature_prediction.ipynb
│
└── reports/
└── Next_Day_Temperature_Prediction_Presentation.pptx





## ▶️ How to Run the Project

### **1. Clone the repository**

git clone https://github.com/<your-username>/next-day-temperature-prediction.git
cd next-day-temperature-prediction


### **2. Create a virtual environment (optional)**

python -m venv venv


**Activate it:**

Windows

venv\Scripts\activate

Mac/Linux

source venv/bin/activate


### **3. Install dependencies**

pip install -r requirements.txt


### **4. Launch Jupyter Notebook**

jupyter notebook


Open:

notebooks/next_day_temperature_prediction.ipynb


##🚀 Future Improvements

Add XGBoost and LightGBM

Use rolling-window time-series validation

Deploy as a Flask/FastAPI prediction API

Build Streamlit dashboard for interactive predictions

Hyperparameter optimization using Optuna

##👤 Author

Sumanth Gannamani
Master’s in Data Science – UMBC