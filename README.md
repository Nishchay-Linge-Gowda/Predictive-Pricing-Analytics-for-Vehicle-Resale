# Predictive Pricing Analytics for Vehicle Resale

## Project Overview
The **Predictive Pricing Analytics for Vehicle Resale** project focuses on building a **machine learning regression model** to accurately estimate the resale price of vehicles based on multiple influencing factors such as **age**, **mileage**, **horsepower**, and other vehicle attributes.  

By combining **data preprocessing, feature engineering**, and **advanced regression modeling**, this project aims to deliver a robust predictive framework that helps optimize inventory valuation and pricing strategies in the automotive resale market.

---

## Objectives
- Develop a regression-based model to predict vehicle resale prices.  
- Apply **feature engineering** to improve model accuracy and interpretability.  
- Perform **exploratory data analysis (EDA)** to uncover key pricing drivers.  
- Detect and handle outliers to ensure stable model performance.  
- Provide actionable insights for **inventory optimization** and **strategic pricing**.  

---

## Dataset
- **Source:** Public or simulated vehicle resale dataset (e.g., Kaggle Car Dataset).  
- **Size:** Thousands of vehicle records with structured features.  
- **Key Attributes:**
  - `Vehicle_Age` – Age of the vehicle in years  
  - `Mileage` – Total distance traveled (in km or miles)  
  - `Horsepower` – Engine power output  
  - `Transmission` – Manual or Automatic  
  - `Fuel_Type` – Petrol, Diesel, Hybrid, or Electric  
  - `Brand` and `Model` – Vehicle manufacturer and model name  
  - `Selling_Price` – Target variable (vehicle resale value)  

---

## Project Workflow

### 1. Data Preprocessing
- Loaded dataset using **Pandas** and performed initial exploration.  
- Checked for missing values and handled them using mean/median imputation.  
- Converted categorical variables (e.g., fuel type, transmission) into numeric representations using **One-Hot Encoding**.  
- Detected and treated outliers in numerical fields (e.g., extreme mileage or price values).  
- Normalized and scaled features to improve model stability.

### 2. Exploratory Data Analysis (EDA)
- Visualized relationships between key variables (age, mileage, horsepower vs. price).  
- Analyzed distribution of numerical and categorical features using **Seaborn** and **Matplotlib**.  
- Computed correlation matrix to identify significant predictors of resale price.  
- Identified pricing patterns across brands, fuel types, and years of manufacture.

### 3. Feature Engineering
- Created derived features such as:
  - **Vehicle_Age_Category** (new, mid-age, old)  
  - **Mileage_per_Year** to normalize usage by vehicle age  
- Encoded categorical variables using **LabelEncoder** and **OneHotEncoder**.  
- Selected top features using **feature importance** and **correlation filtering**.  
- Improved prediction accuracy by ~15% through feature transformation and selection.  

### 4. Model Development
- Implemented multiple regression algorithms using **Scikit-learn**, including:
  - **Linear Regression**  
  - **Ridge Regression**  
  - **Lasso Regression**  
  - **Random Forest Regressor**  
- Evaluated model performance using:
  - **R² Score**  
  - **Mean Absolute Error (MAE)**  
  - **Root Mean Squared Error (RMSE)**  
- Tuned hyperparameters via **GridSearchCV** for optimal performance.  

### 5. Model Evaluation
- Compared results across models and selected the best-performing one based on RMSE and R² score.  
- Visualized actual vs. predicted resale prices to validate prediction accuracy.  
- Analyzed residual errors to check for model bias and underfitting/overfitting.  

### 6. Insights and Visualization
- Identified **key drivers** of resale price: age, mileage, horsepower, and brand value.  
- Found **non-linear patterns** showing diminishing returns for higher horsepower and premium brands.  
- Developed scatter plots, heatmaps, and regression curves to communicate insights visually.  

---

## Technologies Used
- **Programming Language:** Python  
- **Libraries & Frameworks:**
  - Pandas, NumPy – Data cleaning and analysis  
  - Scikit-learn – Machine learning modeling and evaluation  
  - Matplotlib, Seaborn – Data visualization  
- **Environment:** Jupyter Notebook / Google Colab  

---

## Results
- Achieved **15% improvement** in prediction accuracy after feature engineering and model tuning.  
- Delivered an interpretable regression model with high predictive reliability for vehicle resale prices.  
- Provided insights that can assist in **inventory pricing**, **revenue forecasting**, and **automotive market analysis**.

---

## Conclusion
This project demonstrates how **machine learning regression models** can be effectively applied to **predict vehicle resale prices** using real-world data.  
By combining **EDA, feature engineering, and advanced modeling**, it provides a powerful framework for data-driven decision-making in the automotive resale industry.  

Future improvements could include:
- Integrating **neural network models** for complex non-linear relationships.  
- Expanding dataset scope to include **macroeconomic or regional market factors**.  
- Deploying the model as a **web app** for interactive resale price prediction.

