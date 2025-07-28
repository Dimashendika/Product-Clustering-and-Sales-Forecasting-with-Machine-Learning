# Product Clustering and Sales Forecasting with Machine Learning

An end-to-end data science project that leverages **EDA**, **machine learning**, and **time series forecasting** to uncover actionable insights from Superstore sales data (2011–2014). The goal is to optimize sales performance through product segmentation and predictive analytics.

---

##  Overview

###  Objective:
- Analyze sales and profit patterns.
- Segment products based on performance.
- Forecast future sales with seasonality in mind.
- Provide strategic recommendations for pricing, inventory, and marketing.

---

##  Dataset

- **Source**: [Kaggle - Superstore Sales Dataset](https://www.kaggle.com/datasets/laibaanwer/superstore-sales-dataset)
---

##  Exploratory Data Analysis (EDA)

Key findings from the EDA include:

- **General Sales Growth**: Steady increase from 2011 to 2014.
- **Monthly Seasonality**: Peaks in November and December; dips in January and February.
- **Regional Performance**: Central region leads in both sales and profit.
- **Product Categories**: Office Supplies dominate in count, while Consumer segment drives most revenue.
- **Discount Impact**: Discounts significantly reduce profit — each 1% increase reduces average profit by ~$2.60.

---

##  Machine Learning Models

### 1. **Linear Regression**

- **Purpose**: Understand the relationship between discounts and profit.
- **Model Insight**: A 1% increase in discount decreases profit by approximately $2.60.
- **R² Score**: 0.10 (suggests other factors also influence profit).
- **Business Takeaway**: Over-discounting harms margins — optimize discount strategy.

### 2. **KMeans Clustering**

- **Features Used**: Sales and Profit
- **Optimal Clusters**: 3 (determined via Elbow Method)
- **Cluster Interpretation**:
  - **Cluster 0**: Low Sales – Low Profit → Candidates for removal or promotion.
  - **Cluster 1**: High Sales – High Profit → Best-sellers with healthy margins.
  - **Cluster 2**: High Sales – Low Profit → May need cost optimization or pricing review.
- **Business Use**: Enables targeted actions like repositioning, discontinuation, or bundling.

---

##  Time Series Forecasting (Holt-Winters)

- **Method**: Holt-Winters Exponential Smoothing
- **Insight**: Clear upward trend with strong seasonality — peak expected around June 2015.
- **Use Case**: Supports proactive planning for inventory, staffing, and promotions during high-demand periods.

---

##  Key Business Insights

- **Central Region** is the top performer — replicate its success across other regions.
- **South Region** has high sales but low profit — investigate margin issues.
- **Underperforming Regions** (e.g., Canada, Southeast Asia) require targeted interventions.
- **Home Office Segment** lags behind — consider new strategies to boost performance.
- **Office Supplies** dominate in quantity, but **Consumer Segment** drives most revenue.

---

##  Tools & Technologies

- Python (Pandas, NumPy, Matplotlib, Seaborn)
- Scikit-learn (Linear Regression, KMeans)
- Statsmodels (Holt-Winters Forecasting)
- Jupyter Notebook


