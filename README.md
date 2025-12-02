💰 Salary Prediction Web App

A Machine Learning web application built from scratch using Python and Streamlit. This project analyzes real-world developer survey data to build a predictive model and deploys it via an interactive web interface.

📌 Project Overview

The goal of this project is to predict the salary of a software developer based on their Country, Education Level, and Years of Professional Experience.

The project is divided into two main stages:

Data Analysis & Model Building: Cleaning real-world data, handling outliers, and training various Machine Learning models to find the most accurate predictor.

Web App Development: Building a user-friendly frontend using Streamlit to allow users to interact with the model in real-time.

🛠️ Technologies Used

Python (Core language)

Pandas & NumPy (Data cleaning and manipulation)

Matplotlib (Data visualization)

Scikit-Learn (Machine Learning models: Linear Regression, Decision Tree, Random Forest)

Streamlit (Web framework for deployment)

Pickle (Model serialization)

📊 Workflow

Part 1: Data Analysis & Modeling (exploration.ipynb)

Data Cleaning: Handled missing values, renamed columns, and filtered data to focus on full-time developers.

Outlier Removal: Cleaned salary outliers using the Interquartile Range (IQR) method / manual thresholding.

Label Encoding: Converted categorical data (Country, Education) into numerical values for the model.

Model Training: Tested multiple algorithms (Linear Regression, Decision Tree, Random Forest) and used GridSearchCV to find the best hyperparameters.

Result: The Random Forest Regressor (or Decision Tree) provided the best accuracy and was saved for the app.

Part 2: Web App (app.py)

Built a streamlined interface using Streamlit.

Allows users to select their parameters from dropdown menus.

Loads the saved model (saved_steps.pkl) to generate instant salary predictions.

🚀 How to Run the Project

Prerequisites

Make sure you have Python installed.

1. Clone the Repository

git clone [https://github.com/your-username/salary-prediction-app.git](https://github.com/your-username/salary-prediction-app.git)
cd salary-prediction-app


2. Install Dependencies

pip install -r requirements.txt


3. Run the App

streamlit run app.py


📂 Project Structure

├── data/                   # Dataset folder
├── app.py                  # Main Streamlit application
├── predict_page.py         # Prediction logic script
├── explore_page.py         # Visualization logic script
├── salary_prediction.ipynb # Jupyter notebook for analysis & training
├── saved_steps.pkl         # Saved ML model
├── requirements.txt        # List of dependencies
└── README.md               # Project documentation


🔮 Future Improvements

Add more features (e.g., Programming Languages used).

Deploy the app to the cloud (Streamlit Cloud or Heroku).

Implement continuous data updates.

Created by Arina Sadeghi Khiabanian
