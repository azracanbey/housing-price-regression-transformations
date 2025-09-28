# Housing Price Regression with Transformations

This repository explores the **California Housing dataset** and investigates how applying transformations to features (`X`) and the target variable (`y`) affects regression model performance.  

We experiment with **Yeo-Johnson** and **Box-Cox** transformations and benchmark multiple machine learning models.  

---

## 📂 Project Structure
- `housing.csv` → California housing dataset (from Kaggle).  
- `notebooks/` → Jupyter Notebooks with preprocessing, transformations, and model training.  
- `results/` → Model evaluation outputs and comparisons.  

---

## 🔧 Methods & Workflow
1. **Data Preprocessing**
   - Handle missing values, encode categorical features, scale numeric features.  
2. **Transformations**
   - Features (`X`): Yeo-Johnson / Box-Cox.  
   - Target (`y`): Box-Cox.  
3. **Model Training**
   - Linear Regression, Lasso, Ridge  
   - KNeighbors Regressor  
   - Decision Tree, Random Forest  
   - AdaBoost, Gradient Boosting, XGBoost  
4. **Evaluation**
   - Metrics: RMSE, MAE, R².  
   - Compare results **before and after transformations**.  

---

## 📊 Key Findings
- **Linear models (Linear, Lasso, Ridge):** Benefit from transforming `y`.  
- **KNN:** Requires transformation of `X` (big performance boost).  
- **Tree-based models (RF, GBM, XGB):** Largely unaffected or slightly worse after transformations.  
- **Best performing model:** **XGBoost (R² ~0.81 on test set)**.  

---

## 🚀 How to Run
1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/housing-price-regression-transformations.git
   cd housing-price-regression-transformations
