# 🌦️ Weather_Data_Analysis_and_Prediction

## 📘 Project Overview
This project focuses on **analyzing weather data and predicting temperature trends** using multiple **machine learning models** — including **Linear Regression**, **Random Forest**, and **XGBoost**.  
It covers complete steps from **data preprocessing** to **model evaluation** and **30-day temperature forecasting**, providing visualizations, performance metrics, and automated report generation.  
Developed as part of the **Codec Technologies Internship Program**.

---

## 🎯 Objective
To design and implement an end-to-end machine learning pipeline that:
- Analyzes historical weather data.
- Identifies seasonal patterns and temperature trends.
- Predicts future temperature values for the next 30 days.
- Compares multiple regression models for performance.

---

## 🧩 Technologies Used
- **Python**
- **NumPy**, **Pandas**
- **Matplotlib**, **Seaborn**
- **Scikit-learn**
- **XGBoost** *(optional)*
- **ReportLab** *(for PDF generation)*
- **Google Colab / Jupyter Notebook**

---


---

## 🧠 Steps in the Project

### **1️⃣ Data Loading**
- Loads `weather.csv` containing `date` and `temp` columns.
- Generates synthetic data if no CSV is provided.

### **2️⃣ Exploratory Data Analysis (EDA)**
- Summary statistics and trend visualization.
- Time-series plots and seasonal decomposition.

### **3️⃣ Feature Engineering**
Creates lag and time-based features:
temp_lag1, temp_lag7, rolling_7, rolling_30, dayofyear, month, dayofweek, time_index


### **4️⃣ Train/Test Split**
- Uses last 90 days as the test set for time-aware validation.

### **5️⃣ Model Training**
Models trained:
- **Linear Regression**
- **Random Forest Regressor** (GridSearchCV tuning)
- **XGBoost Regressor** *(if installed)*

### **6️⃣ Evaluation Metrics**
- **MAE** — Mean Absolute Error  
- **RMSE** — Root Mean Squared Error  
- **R² Score** — Coefficient of Determination

### **7️⃣ Forecasting**
- Recursive 30-day forecast using trained models.
- Results plotted and exported to `forecast.csv`.

### **8️⃣ Visualization (10 Charts)**
1. Temperature Time Series  
2. Seasonal Decomposition  
3. 7-day and 30-day Rolling Averages  
4. Temperature Distribution  
5. Monthly Average Temperature  
6. Day-of-Week Temperature  
7. Correlation Heatmap  
8. Actual vs Predicted (Linear Regression)  
9. Actual vs Predicted (Random Forest)  
10. 30-Day Forecast Comparison  

### **9️⃣ PDF Report Generation**
- Automatically generates a summary report using ReportLab:
  - Dataset statistics
  - Model performance
  - Forecast results

---

## 📊 Example Model Performance
| Model | MAE | RMSE | R² |
|--------|------|------|----|
| Linear Regression | ≈ 1.2–1.8 | ≈ 1.5–2.1 | ≈ 0.90+ |
| Random Forest | ≈ 0.8–1.2 | ≈ 1.0–1.6 | ≈ 0.95+ |
| XGBoost | ≈ 0.7–1.0 | ≈ 1.0–1.5 | ≈ 0.96+ |

*(Actual results depend on dataset.)*

---

## ✅ Project Conclusion
The **Weather Data Analysis and Prediction** project successfully demonstrates how machine learning can forecast temperature trends using historical data.  
Among all models, **Random Forest** achieved the best performance, capturing non-linear temperature variations effectively.  
The project’s pipeline — from EDA to forecasting and report generation — serves as a foundation for advanced **climate analytics** and **predictive modeling applications**.

---

## 🚀 Future Enhancements
1. Add additional weather parameters — humidity, wind speed, pressure.  
2. Integrate **LSTM / GRU** deep learning models for better time-series forecasting.  
3. Deploy model as an **API or Streamlit dashboard** for real-time updates.  
4. Expand forecasting to multi-variable prediction (e.g., rainfall + temperature).  

---

## 🧾 Author
**Developed by:** *Jay Vishwakarma*  
**Organization:** *Codec Technologies Internship Project*  
**Year:** 2025  
**Location:** India  

---

### 🌟 Acknowledgements
Special thanks to **Codec Technologies** for the opportunity to work on this project and explore real-world applications of machine learning in environmental forecasting.

---

### 📬 Contact
For collaboration or queries:  
📧 **jayvishwakarma0308@gmail.com**  
🔗 [LinkedIn Profile](www.linkedin.com/in/jay-vishwakarma03)

---

### ⭐ How to Use
1. Upload your `weather.csv` file (with `date` and `temp` columns).  
2. Run the notebook step-by-step in **Google Colab**.  
3. View the 10 generated charts for insights.  
4. Check your outputs:
   - `forecast.csv` → Next 30-day predictions  
   - `weather_report.pdf` → Model summary and metrics  

---

### 🎓 End of Project
**Project Completed Successfully ✅**

