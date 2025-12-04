🌡️ NEXT DAY TEMPERATURE PREDICTION

Machine Learning Project – Regression Models for Weather Forecasting

Predicting next-day temperature is essential for agriculture, climate analysis, and environmental planning.
This project builds machine learning models to forecast Next Day Minimum (T_MIN) and Next Day Maximum (T_MAX) temperatures using historical meteorological data from the UCI Bias Correction of Numerical Prediction Model Temperature Forecast dataset.

📁 Dataset

Source: UCI Machine Learning Repository
Link: https://archive.ics.uci.edu/ml/datasets/Bias+Correction+of+Numerical+Prediction+Model+Temperature+Forecast

Dataset Details:

~7,750 rows

25 meteorological attributes

Includes:

Atmospheric pressure

Relative humidity

Wind speed & direction

Temperature readings

Targets:

Next_Tmin

Next_Tmax

Dataset is loaded directly from the UCI URL in the notebook – no local download needed.

🧹 Data Cleaning & Preprocessing

Performed steps:

KNN imputation for missing values

Remove redundant columns & set proper data types

Exploratory Data Analysis:

Distribution plots

Boxplots

Correlation heatmap

Pairplots

Standard scaling for numerical features

Feature selection using SelectKBest

PCA experiments for dimensionality reduction

🤖 Machine Learning Models

Two prediction targets:

Next_Tmin

Next_Tmax

Models evaluated:

Linear Regression

Random Forest

Gradient Boosting

KNN Regressor

Support Vector Regressor

VotingRegressor Ensemble

Training pipeline includes:

Train/test split

Feature scaling

Hyperparameter tuning (GridSearchCV)

Evaluation with four metrics

🧪 Evaluation Metrics

Metrics used:

R² Score

MSE

MAE

Explained Variance

Approximate Results:

T_MIN Prediction:

Linear Regression: ~0.82

Random Forest: ~0.84–0.85

Gradient Boosting: ~0.83

KNN: ~0.83

SVR: ~0.85

T_MAX Prediction:

Random Forest: ~0.87

Gradient Boosting: ~0.81

KNN: ~0.90

SVR: ~0.86

KNN and SVR gave the most accurate predictions.

📊 Visualizations Included

Distributions for temperature variables

Correlation heatmaps

Outlier boxplots

Model comparison charts

PCA variance graphs

Learning curves

📂 Project Structure

next-day-temperature-prediction/
│
├── README.md (this file)
├── requirements.txt
├── .gitignore
│
├── notebooks/
│ └── next_day_temperature_prediction.ipynb
│
└── reports/
└── Next_Day_Temperature_Prediction_Presentation.pptx

▶️ How to Run

Clone the repository:
git clone https://github.com/
<your-username>/next-day-temperature-prediction.git
cd next-day-temperature-prediction

Create a virtual environment (optional):
python -m venv venv
venv\Scripts\activate (Windows)
source venv/bin/activate (Mac/Linux)

Install dependencies:
pip install -r requirements.txt

Launch Jupyter Notebook:
jupyter notebook

Then open:
notebooks/next_day_temperature_prediction.ipynb

🚀 Future Improvements

Add XGBoost or LightGBM

Deploy API using Flask/FastAPI

Rolling-window time-series validation

Streamlit dashboard for predictions

Automated hyperparameter optimization (Optuna)

📘 Author

Sumanth Gannamani
Master’s in Data Science – UMBC
Machine Learning | Predictive Modeling | Data Analysis