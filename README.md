# 🏠 House Price Prediction - Bengaluru

A Machine Learning project to predict house prices in Bengaluru based on various features such as location, square footage, number of bedrooms, and bathrooms.  
The model uses **Linear Regression** along with feature engineering and hyperparameter tuning to deliver accurate predictions.

---

## 📊 Dataset
- **Name:** Bengaluru House Price Dataset  
- **Source:** [Kaggle](https://www.kaggle.com/datasets/amitabhajoy/bengaluru-house-price-data)  
- **File:** `Bengaluru_House_Data.csv`  
- **Features used:**
  - `location`
  - `total_sqft`
  - `bath`
  - `bhk`

---

## ⚙️ Tech Stack
- **Language:** Python 3  
- **Libraries:**  
  - pandas  
  - numpy  
  - matplotlib / seaborn  
  - scikit-learn  

---

## 🔑 Project Workflow
1. **Data Cleaning & Preprocessing**  
   - Handled missing values  
   - Converted categorical data (locations) using One Hot Encoding  
   - Removed outliers  

2. **Feature Engineering**  
   - Created new features (`bhk`, `bath`)  
   - Reduced dimensionality of locations  

3. **Model Building**  
   - Trained a **Linear Regression model**  
   - Used `GridSearchCV` for best hyperparameters  
   - Evaluated using R² and cross-validation  

4. **Prediction Function**  
   ```python
   predict_price('1st Phase JP Nagar', 1000, 2, 2)
   # Example Output → 83.86 Lakhs
