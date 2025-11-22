# 🛒 BlinkIT Grocery Data Analysis & Sales Prediction

![Python](https://img.shields.io/badge/Python-3.10-blue) ![Library](https://img.shields.io/badge/Library-Pandas%20%7C%20ScikitLearn-orange) ![Platform](https://img.shields.io/badge/Platform-Google%20Colab-yellow) ![Status](https://img.shields.io/badge/Status-Completed-green)

## 📌 Project Overview
This project involves a comprehensive data analysis and machine learning pipeline built for **BlinkIT** (a Quick Commerce grocery platform). The goal is to analyze historical sales data to understand customer purchasing behavior, optimize inventory strategies, and build a predictive model to forecast sales for different outlet types.

By leveraging **Random Forest Regression**, this project identifies key revenue drivers and provides actionable business recommendations for store expansion and pricing strategies.

## 📊 Key Features
* **Smart Data Cleaning:** Implemented advanced imputation strategies (Item-specific mean for weight, Mode by Outlet Type for size) rather than standard mean filling.
* **Exploratory Data Analysis (EDA):** Visualized sales distributions, correlation heatmaps, and categorical performance.
* **Feature Engineering:** Created new features like `Outlet_Age` and standardized `Item_Category` to improve model context.
* **Machine Learning:** Built and tuned a Random Forest Regressor to predict `Item_Outlet_Sales`.

## 🛠️ Tech Stack
* **Language:** Python
* **Libraries:**
  * `Pandas` & `NumPy` (Data Manipulation)
  * `Matplotlib` & `Seaborn` (Data Visualization)
  * `Scikit-Learn` (Machine Learning & Preprocessing)
* **Environment:** Jupyter Notebook / Google Colab

---

## 🔍 Key Insights & Findings

### 1. Pricing is the Primary Driver
There is a strong positive correlation between **Item MRP** and **Sales**. Premium/Higher-priced items are the biggest revenue generators, suggesting that stocking high-value inventory is critical for revenue growth.

### 2. Outlet Architecture Matters
**Supermarket Type 3** (Large Warehouses) significantly outperforms small Grocery Stores.
* **Recommendation:** BlinkIT should prioritize expanding larger warehouse-style dark stores in Tier 2/3 cities to maximize throughput.

### 3. The "Low Fat" Myth
Despite the trend towards healthy eating, the data shows no significant difference in sales volume between **Low Fat** and **Regular** items.
* **Recommendation:** Inventory should remain balanced; do not overstock niche health items at the expense of regular staples.

### 4. Outlet Age & Stability
Older, established outlets show more consistent sales patterns compared to newer stores, indicating the importance of customer trust and long-term local presence.

---

## 📈 Model Performance
We used a **Random Forest Regressor** due to its ability to handle non-linear relationships and resistance to overfitting.

| Metric | Score | Interpretation |
| :--- | :--- | :--- |
| **R² (Accuracy)** | **~56%** | Standard for retail data with high human behavioral variance. |
| **RMSE** | **~1,050** | Average error margin in sales currency. |

---

## 📸 Visualizations

### Correlation Heatmap
> Shows the relationship between numerical features, highlighting the link between MRP and Sales.

### Feature Importance (Random Forest)
> Visualizes which factors (MRP, Outlet Type) the AI considers most important for prediction.

---

## 🚀 How to Run This Project

1. **Clone the Repository**
   ```bash
   git clone [https://github.com/yourusername/BlinkIT-Sales-Prediction-Analysis.git](https://github.com/AnuragRai7/BlinkIT-Sales-Prediction-Analysis.git)
