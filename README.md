🛵 Food Delivery Time Prediction using Machine Learning & Streamlit

This project predicts food delivery time (in minutes) using Machine Learning regression models and a Streamlit web application for real-time predictions.

The application allows users to input delivery-related parameters and receive instant predictions powered by a trained ML model.

🔗 Project Links

🌐 Live Streamlit App
https://food-delivery-analysis-prediction-dhnqmtsnwfflkv4k3cpwkj.streamlit.app/

📁 GitHub Repository
https://github.com/ShreyaAnde/food-delivery-analysis-prediction

📌 Project Overview

The objective of this project is to estimate delivery time based on real-world delivery conditions.

The model considers multiple influencing factors such as:

Distance (km)

Weather conditions

Traffic level

Time of day

Vehicle type

Preparation time

Courier experience

Using historical delivery data, we built and evaluated regression models to generate accurate delivery time predictions.

📊 Dataset Information

The dataset contains historical food delivery data.

Target Variable: Delivery_Time_min

Data preprocessing and cleaning performed

Outliers analyzed and handled

Categorical variables encoded manually

🔍 Key Insights from Exploratory Data Analysis (EDA)
🔹 1. Distance is the Strongest Predictor

Delivery time increases significantly with distance. A strong positive correlation was observed.

🔹 2. Traffic Level Impacts Delivery Duration

High traffic conditions significantly increase delivery time compared to low and medium traffic.

🔹 3. Weather Conditions Affect Performance

Rainy and foggy weather increase average delivery duration.

🔹 4. Preparation Time Directly Adds to Total Time

Higher preparation time proportionally increases final delivery time.

🔹 5. Courier Experience Improves Efficiency

Experienced couriers tend to deliver faster, especially under moderate traffic.

🧠 Machine Learning Workflow

The complete ML pipeline included:

Data Cleaning & Preprocessing

Feature Selection

Manual Encoding of Categorical Variables

Train-Test Split

Feature Scaling using StandardScaler

Model Training & Evaluation

Model & Scaler saved using joblib

The same scaler used during training is reused during prediction to ensure consistent and accurate results.

🤖 Models Evaluated

Linear Regression

Decision Tree Regressor

Random Forest Regressor

✅ Final Model Selected: Random Forest Regressor
📌 Why Random Forest?

Handles non-linear relationships effectively

More robust to outliers

Reduces overfitting compared to Decision Tree

Better generalization on unseen data

Higher R² score and lower RMSE compared to other models

Random Forest provided the best balance between bias and variance and was selected for deployment.

🌐 Streamlit Application Features

The deployed Streamlit app allows users to:

Enter delivery-related details

Predict estimated delivery time

View predictions in minutes

Experience real-time inference

Application Highlights:

Model loaded using caching

Correct feature scaling applied during inference

Clean and user-friendly interface

Deployed on Streamlit Cloud

📂 Project Structure
food-delivery-analysis-prediction/
│
├── app.py
│   └── Streamlit web application
│
├── delivery_time_model.pkl
│   └── Trained ML model
│
├── scaler.pkl
│   └── StandardScaler used during training
│
├── food_delivery_times.csv
│   └── Dataset
│
├── requirements.txt
│   └── Dependencies
│
└── README.md
    └── Project documentation

📦 Requirements
streamlit
numpy
pandas
scikit-learn
joblib

🛠 How to Run Locally
git clone https://github.com/ShreyaAnde/food-delivery-analysis-prediction
cd food-delivery-analysis-prediction
pip install -r requirements.txt
streamlit run app.py

🚀 Future Improvements

Hyperparameter tuning

Real-time traffic API integration

Advanced feature engineering

Model comparison dashboard

CI/CD automation for deployment

🛠 Technologies Used

Python

Pandas

NumPy

Scikit-learn

Joblib

Streamlit

👩‍💻 Author

Shreya Ande

🔗 GitHub: https://github.com/ShreyaAnde

🔗 Project Repository: https://github.com/ShreyaAnde/food-delivery-analysis-prediction


