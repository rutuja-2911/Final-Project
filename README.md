# E-commerce Return Rate Reduction Analysis

## Objective
Identify why customers return products and how return rates vary by **category**, **geography**, and **marketing channel**. The aim is to help reduce return rates by uncovering key patterns and risk factors.

## Tools & Technologies
- **Python** (Pandas, NumPy, Matplotlib, Scikit-learn, pandasql)
- **SQL** (via pandasql)
- **Power BI** (interactive dashboard)

## Project Workflow

1. **Data Cleaning**
   - Removed rows with missing values (`price`, `shipping_days`, `customer_rating`).
   - Selected only relevant fields for analysis.

2. **Return Rate Analysis**
   - Grouped data by product category.
   - Calculated and visualized return % using bar plots.

3. **Predictive Modeling**
   - Applied **Logistic Regression** to predict return likelihood.
   - Used `get_dummies` for encoding and `StandardScaler` for normalization.
   - Evaluated using classification report and confusion matrix.

4. **Risk Scoring**
   - Calculated return probability for each product.
   - Exported products with **> 40% predicted return risk** to CSV.

5. **Power BI Dashboard**
   - Visualized return risk by **region** and **category**.
   - Drill-through filter for **order-level** insights.
   - KPIs for return flag counts and shipping days.

## Deliverables

- `high_risk_products.csv`: High-risk items based on model prediction.
- `MAIN2_merged.pdf`: Power BI Dashboard showing return analysis.
- Python codebase for modeling and prediction.

## Sample Dashboard Insights

- **Clothing** has the highest return probability across categories.
- Regions like **South** and **Central** show more returns.
- Products with **9+ shipping days** tend to have a higher return risk.
