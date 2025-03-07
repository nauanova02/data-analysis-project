# 💧 Data Analysis & Machine Learning for Steam Consumption Prediction  
**Category:** Data Analysis | Machine Learning | Time-Series Forecasting | Power BI  

## **🔹 Overview**  
This project predicts **steam (water) consumption in a building** using **K-Nearest Neighbors (KNN) and Random Forest** models.  
The dataset is sourced from **[Building Data Genome Project 2](https://www.kaggle.com/datasets/claytonmiller/buildingdatagenomeproject2)** and merged with **hourly weather statistics from Ottawa**.  
A **Power BI dashboard** is included to visualize the **correlation between temperature and steam consumption**.  

✅ **Data preprocessing & feature engineering**  
✅ **Machine learning models: KNN (Min-Max Scaling) & Random Forest**  
✅ **Merging building water consumption with weather data**  
✅ **Power BI dashboard for data insights & correlations**  

📌 **Skills Demonstrated:**  
- **Data Cleaning & Preprocessing**  
- **Feature Engineering & Scaling Techniques**  
- **Supervised Learning (KNN & Random Forest)**  
- **Data Visualization (Power BI)**  

---

## **🛠️ Technical Framework**  

### **1️⃣ Dataset Details**
🔹 **Primary Dataset:** [Building Data Genome Project 2](https://www.kaggle.com/datasets/claytonmiller/buildingdatagenomeproject2)  
🔹 **Supplementary Data:** Hourly **Ottawa weather statistics**  
🔹 **Key Features:**
   - **Steam (water) consumption (target variable)**
   - **Temperature (°C)**
   - **Humidity (%)**
   - **Wind Speed (m/s)**
   - **Pressure (hPa)**
   - **Dew Point (°C)**  

📌 **Data Processing:**  
- Merging **building consumption data** with **weather statistics**  
- Handling **missing values & outliers**  
- Applying **Min-Max Scaling** to normalize features  

---

### **2️⃣ Machine Learning Models**
✅ **K-Nearest Neighbors (KNN)** – Uses **Min-Max Scaling** for better distance-based predictions  
✅ **Random Forest** – Captures **non-linear relationships** in the dataset  

📌 **Feature Engineering:**  
- **Rolling Averages** for temperature & humidity  
- **Time-Based Features** (Hour, Day of Week, Season)  
- **Interaction Terms** (e.g., Temperature × Humidity)  

## **📈 Model Performance Results**  

| **Model**                     | **R² Score** | **MSE**     | **RMSE**  | **MAE**   |
|--------------------------------|-------------|------------|----------|----------|
| **Random Forest Regression**   | **0.89**    | 47,599.25  | 218.17   | 126.46   |
| **Random Forest (Tuned)**      | **0.90**    | 45,807.51  | 216.35   | 110.45   |
| **K-Nearest Neighbors (KNN)**  | **0.85**    | 65,027.42  | 255.00   | 154.61   |
| **KNN with Min-Max Scaling**   | **0.84**    | 0.01       | 0.09     | 0.06     |

📌 **Key Observations:**  
✅ **Tuned Random Forest achieved the best performance (R² = 0.90, RMSE = 216.35)**, making it the most reliable model.  
✅ **Standard Random Forest performed well (R² = 0.89) but slightly worse than the tuned version.**  
✅ **KNN struggled compared to Random Forest, with higher RMSE (255.00) and MAE (154.61).**  
✅ **KNN with Min-Max Scaling had the lowest error values but may have been overfitting due to an abnormally low MSE (0.01).**  

📌 **Conclusion:** The **tuned Random Forest model** is the best choice for predicting steam consumption due to its **higher accuracy and lower error rates**. 🚀


