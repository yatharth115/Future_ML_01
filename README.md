# 📈 AI-Powered Retail Sales Forecasting Dashboard

## 🎯 Project Overview
This project delivers a complete predictive analytics solution for a retail business using the Superstore Sales dataset. We leverage time series modeling (Facebook Prophet) to forecast future sales and visualize the insights in an interactive Power BI dashboard, providing actionable intelligence for inventory planning and resource allocation.

**Task Status:** ✅ Complete
**Files Included:** Jupyter Notebook (Model Training), Processed Data, Power BI Dashboard (.pbix and screenshot).

---

## 🛠️ Tech Stack & Tools

* **Data Analysis & Modeling:** Python (Pandas, NumPy)
* **Forecasting Model:** Facebook Prophet
* **Environment:** Jupyter Notebook
* **Visualization & Dashboard:** Power BI Desktop
* **Version Control:** Git & GitHub

---

## 🔍 Methodology (What I Did)

### 1. Data Cleaning & Feature Engineering
* Loaded the raw `Sample - Superstore.csv` dataset.
* Converted the 'Order Date' column to datetime format.
* Aggregated sales to a **daily** level (for Prophet compatibility) and **monthly/regional** level (for segmented analysis).
* Created a combined dataset of **Actuals** and **Forecasts** for seamless visualization in Power BI.

### 2. Time Series Forecasting (Prophet)
* **Model Selection:** Facebook Prophet was chosen for its robustness in handling multiple seasonalities (weekly, yearly) and missing data, and for providing interpretable trend/seasonality components.
* **Training:** The model was trained on historical daily sales data from 2014 to 2017.
* **Forecast Generation:** A forecast was generated for **18 months** into the future (mid-2018 to end of 2019).
* **Output:** The final forecast, including confidence intervals (`yhat_lower`, `yhat_upper`), was exported to `final_sales_forecast.csv`.

### 3. Power BI Dashboard Development
* The actual and forecasted data were merged and imported.
* A custom Date Dimension table was created for precise date comparisons.
* The dashboard was built following the key requirements (see Key Features below).

---

## 🔑 Key Deliverables & Features

### 1. Forecast vs. Actuals Trend
* A primary line chart visualizing historical sales (Actuals) seamlessly transitioning into the future prediction (Forecast). The forecast includes the upper and lower confidence bounds.

### 2. Decision-Making Insight Cards
| Metric | Purpose |
| :--- | :--- |
| **Forecasted Next Qtr Sales** | Budgeting and Goal Setting |
| **Y-o-Y Growth % (Forecast)** | Assessing future performance |
| **Top 3 Selling Categories** | Inventory Focus |

### 3. Interactive Analysis
* Filters allow users to slice data by **Region** and **Category** to understand localized trends.
* Monthly sales comparisons highlight high-demand and low-demand periods for operational planning.

### 🖼️ Dashboard Screenshot



---

## 💡 Business Recommendations

* **Seasonal Inventory**: The forecast clearly shows a peak in **Q4** (October/November/December) sales. **Recommendation:** Increase inventory and staffing levels by **15%** (based on forecasted growth) starting in early October.
* **Regional Focus**: The **West** region consistently shows the highest sales volume but the **Central** region shows higher forecasted growth variance. **Recommendation:** Allocate targeted marketing budget to the Central region to capture this emerging growth.
* **Product Strategy**: Technology remains the highest-grossing category. **Recommendation:** Focus procurement efforts to ensure the highest-profit technology items are consistently in stock.

---