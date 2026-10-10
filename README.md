# 🚗 Used Car Price Prediction

A **used car price prediction system using machine learning** that estimates a car's price based on features such as brand, model, mileage, engine volume, fuel type, registration status, body type, and manufacturing year. The project uses **Linear Regression and Random Forest Regressor** to learn patterns from car data and predict the estimated selling price based on the features provided by the user.

The main objective of this project is to understand the end-to-end workflow of a machine learning regression problem, including **data cleaning**, handle **missing values and outliers**, perform **exploratory data analysis (EDA)**, **feature engineering**, **model training**, **hyperparameter tuning(`GridSearchCV`)**, and **model evaluation(`MSE`)**. The trained Random Forest model is integrated into a Streamlit web application, allowing users to enter car details and receive an estimated used car price.

> **Note:** This project focuses on a supervised machine learning regression problem. Linear Regression and Random Forest Regressor are trained and evaluated to compare their performance, and the saved Random Forest model is used by the web application to generate price predictions.


## 📸 Application Preview
![Used Car Price Prediction App](images/app_screenshot.png)


## 🌐 Live Demo
https://car-price-analyzer.streamlit.app/


## 🔄 How It Works

1. Load the raw used car dataset and clean and preprocess the data.
2. Perform exploratory data analysis (EDA) to understand data distributions and relationships between features.
3. Perform feature engineering and encode categorical features into numerical representations.
4. Train Linear Regression and Random Forest Regressor models.
5. Tune Random Forest hyperparameters using `GridSearchCV` and `RandomizedSearchCV`.
6. Evaluate and compare model performance using appropriate regression evaluation metrics(`MSE`).
7. Save the trained Random Forest model using `Joblib`.
8. Integrate the trained model into the Streamlit web application to predict used car prices based on user-provided details.


## 📂 Project Structure

The project contains the following main files and folders:

* **Data/** – Contains the raw and cleaned datasets used for training and analysis.

  * `Car_Raw_Data.csv`
  * `Car_preproccesed.csv`
  * `Car_cleaned.csv`
  * `Car_cleaned_with_Model.csv`

* **1_1Data_Cleaning_Car_drop_Model.ipynb** – Data cleaning and preprocessing notebook without the model feature.

* **1__2Data_Cleaning_Car_with_Model.ipynb** – Data cleaning and preprocessing notebook including the model feature.

* **2_Checking_Assumptions_EDA.ipynb** – Exploratory Data Analysis (EDA), feature relationships, correlation analysis.

* **Linear_Regression.ipynb** – Linear Regression model training and evaluation.

* **Random_Forest_Model.ipynb** – Random Forest model training, hyperparameter tuning, and evaluation.

* **rf1_base_rf.pkl** – Saved Random Forest model used by the web application.

* **main.py** – Streamlit application file for user interaction and price prediction.

* **requirements.txt** – List of required Python libraries.

* **README.md** – Project documentation and usage instructions.


## 🛠️ Tech Stack

Python · NumPy · Pandas · Matplotlib · Seaborn · Scikit-learn · Joblib · Streamlit
