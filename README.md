# Vancouver-Crime-Prediction-Using-Machine-Learning
This project analyzes and predicts Vancouver’s criminal activity using machine learning techniques. It includes data preprocessing, exploratory data analysis (EDA), classification models (Random Forest, Decision Tree, XGBoost), and time-series forecasting. The final product includes a Flask-based web application for crime prediction 

# 🔍 Vancouver Crime Prediction Using Machine Learning  

## 📌 Project Overview  
This project aims to analyze and predict **Vancouver’s criminal activity** using machine learning techniques. The dataset consists of **crime reports from 2003 to 2023**, obtained from the **Vancouver Open Data Catalogue**. The analysis includes:  
✅ **Data Cleaning & Preprocessing** (handling missing values, feature engineering)  
✅ **Exploratory Data Analysis (EDA)** (crime trends, time-based patterns, high-crime areas)  
✅ **Machine Learning Classification** (Random Forest, Decision Tree, XGBoost, KNN)  
✅ **Time-Series Forecasting** (Holt-Winters method for predicting future crime trends)  
✅ **Deployment of a Crime Prediction Model** using **Flask**  

## 🚀 Technologies Used  
- **Python (Pandas, NumPy, Matplotlib, Seaborn, Scikit-Learn)**  
- **Jupyter Notebook** for analysis & model training  
- **Flask** for web-based crime prediction  
- **Machine Learning Models:**  
  - Random Forest  
  - Decision Tree  
  - XGBoost  
  - K-Nearest Neighbors (KNN)  
- **Time-Series Forecasting:** Holt-Winters Method  

---

## 📂 Repository Structure  

📂 Vancouver-Crime-Prediction
│── 📂 data/ # Contains dataset files
│ ├── crimedata.csv # Raw dataset link
│── 📂 notebooks/ # Contains Jupyter Notebook(s)
│ ├── Vancouver_Crime_Analysis.ipynb # Main analysis notebook
│── 📂 reports/ # Contains project documentation
│ ├── FINALREPORT.pdf # Full project report
│── 📂 reports/ # Contains project documentation
│ ├── Presentation.pdf # Project presentation slides

---

## 📊 Exploratory Data Analysis (EDA)  
Before building models, **EDA** was performed to analyze crime trends over time and across different neighborhoods.  

📌 **Key Insights from EDA:**  
- **Theft from vehicles** is the most common crime in Vancouver.  
- **Crime rates peaked in 2019**, then declined after 2020, likely due to COVID-19 restrictions.  
- **Crime activity is highest on Fridays and Saturdays**, especially between **6 PM – Midnight**.  
- **Downtown Vancouver (Central Business District) has the highest crime rate**.  

---

## 🤖 Machine Learning Models  
The project implemented **classification models** to predict crime categories based on location data.  

📌 **Model Performance:**  
| Model | Accuracy (%) | Best Use Case |  
|------------|--------------|----------------|  
| **Random Forest** | 55.08% | Best for general crime prediction |  
| **Decision Tree** | 54.96% | Interpretable model |  
| **XGBoost** | 49.62% | Stronger in high-frequency crime categories |  
| **KNN** | 52.32% | Sensitive to neighborhood crime patterns |  

📌 **Time-Series Forecasting:**  
The **Holt-Winters method** was used to forecast future crime trends. **Results indicate a general decline in crime rates in the coming years.**  

---

## 🚀 Deployment of the Crime Prediction Model  
A **Flask web application** was developed to predict potential criminal activities based on user-provided geographic inputs (longitude, latitude).  

📌 **How It Works:**  
1️⃣ User enters location coordinates.  
2️⃣ Model predicts the most likely type of crime.  
3️⃣ Results are displayed in real-time via a web interface.  

📌 **Local Deployment:**  
To run the Flask app locally:  
```bash
python app.py
```

- The app is currently deployed locally but can be extended to cloud platforms like AWS, GCP, or Heroku.
