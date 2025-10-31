## Laptop Price Prediction & Feature Analysis

---

### 🧩 **Overview**

This project explores and models laptop price data to understand which factors influence price the most.
It involves **data cleaning, feature engineering, exploratory visualization**, and a **machine learning pipeline** to predict `Price_euros`.

---

### 📊 **Objectives**

* Perform EDA on laptop specifications
* Engineer new features like **Pixels Per Inch (PPI)** and **Total Storage**
* Visualize trends between features and price
* Predict laptop price using **Random Forest Regressor**

---

### ⚙️ **Technologies Used**

* **Python**
* **Pandas**, **NumPy**, **Matplotlib**, **Seaborn**
* **Scikit-learn** (for ML pipeline)
* **Jupyter Notebook / Google Colab**

---

### 🧠 **Key Steps**

1. **Data Cleaning**

   * Standardized column names
   * Converted yes/no columns to binary (1/0)
   * Handled missing and numeric type conversions

2. **Feature Engineering**

   * Computed `PPI = √(ScreenW² + ScreenH²) / Inches`
   * Combined `PrimaryStorage` and `SecondaryStorage` into `TotalStorageGB`
   * Extracted CPU and GPU features

3. **EDA (Exploratory Data Analysis)**

   * Distribution of prices
   * Box plots of price vs RAM
   * Median prices per company

4. **Model Building**

   * Encoded categorical variables using `OneHotEncoder`
   * Scaled numeric features with `StandardScaler`
   * Trained a **Random Forest Regressor** with pipeline
   * Evaluated using **MSE**, **RMSE**, and **R²**

---

### 📈 **Results**

| Metric                        | Description                                 |
| ----------------------------- | ------------------------------------------- |
| **MSE**                       | Measures average squared prediction error   |
| **R² Score (~0.75 expected)** | Model explains about 75% of price variation |
| **Top Features**              | RAM, CPU frequency, PPI, Company            |

---

### 📊 **Generated Visuals**

* Price Distribution
* Price by RAM and Company
* Actual vs Predicted Price Scatter Plot
* Top Feature Importances

---

### 📂 **Output Files**

* `laptops_cleaned.csv` — cleaned dataset after processing
* Visualizations and model performance plots

---
