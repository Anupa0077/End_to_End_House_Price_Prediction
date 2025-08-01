#  Bengaluru House Price Predictor

A complete end-to-end machine learning project to **predict house prices in Bengaluru**, built using regression models and deployed with a **Flask backend**, tested with **Postman**, and connected to a **custom frontend**.

---

## 🚀 Demo Preview

 Input features:  
- Location (dropdown)  
- BHK  
- Bathroom count  
- Size in square feet  

 Output:  
- Estimated price in lakhs (₹)

---

##  Tech Stack

| Layer        | Technology       |
|-------------|------------------|
| ML Model    | scikit-learn (Linear Regression) |
| Backend     | Flask + Python   |
| Data Flow   | NumPy, Pandas    |
| Testing     | Postman          |
| Frontend    | HTML + CSS + JS  |
| Deployment  | (Localhost)      |

---

##  How It Works

1. **Data Preprocessing**:  
   - Cleaned and processed housing data  
   - Handled outliers and missing values  
   - Performed one-hot encoding on locations  

2. **Model Building**:  
   - Trained a linear regression model  
   - Saved model using `pickle`  

3. **Backend (Flask)**:  
   - Exposes two endpoints:
     - `/get_location_names` (GET)  
     - `/predict_home_price` (POST)  

4. **Frontend Integration**:  
   - User selects location, enters BHK, bath, and size  
   - On form submission, frontend fetches prediction from Flask backend

---

## 📂 Project Structure

Bengaluru-House-Price-Predictor/
- server.py # Flask application entry point
- util.py # Utility functions for loading model and making predictions
- artifacts/ # Serialized model and metadata
- Bengaluru_House_Price_model.pickle # Trained regression model (saved using pickle)
- columns.json # List of feature columns (used for encoding input)
- client/ # (Optional) Frontend UI
- index.html # Basic HTML form to interact with the API
