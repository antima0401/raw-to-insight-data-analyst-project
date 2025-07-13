# raw-to-insight-data-analyst-project

## 🚀 Objective
Clean raw text file of customer and loan records, extract structured data, join with Python, visualize insights, and optionally apply machine learning.

## 🧱 Project Structure
- `data/`: Raw and cleaned data
- `notebooks/`: Jupyter notebooks for EDA and modeling
- `output/`: Visuals and insights
- `requirements.txt`: Python packages used

## 🛠️ Tools Used
- Python (Pandas, Matplotlib, Seaborn, Scikit-learn)
- Jupyter Notebook

## 📊 Key Analyses
- Customer demographics vs. loan amounts
- Loan default trends
- Correlation between income and repayment
- ML Model: Logistic regression for default prediction
  
## 📈 Insights from Data Analysis Dashboard

### 🔹 1. Loan Status Distribution
- Loans are nearly evenly split: **33.4% default**, **33.3% active**, **33.3% closed**.
- Suggests balanced data for classification and risk modeling.

### 🔹 2. Loan Amount Distribution
- Loan disbursement amounts are **evenly distributed** across various value bands.
- Lending strategy is consistent and inclusive across customer segments.

### 🔹 3. Days Past Due (DPD) Comparison
- Customer DPD shows wider variation than **Loan DPD**.
- Indicates potential **compliance gaps** or **customer reporting delays**.

### 🔹 4. Default Rate by Gender
- Male customers show a slightly **higher default rate** (~0.34%) than females (~0.33%).
- May reflect risk patterns based on gender behavior or socio-economic factors.

### 🔹 5. Customer Age Distribution
- Age is evenly spread from 20 to 60+, with no dominant group.
- Indicates a broad and inclusive customer base.

### 🔹 6. Default Rate by Tenure
- Higher default observed at 5 and 35 months tenure.
- Possible indication of promotional tenures or loan churn behavior.

### 🔹 7. Feature Correlation Matrix
- Weak correlation of default (`is_default`) with numerical variables.
- Strongest correlation is between `dpd_x` and `dpd_y` (~0.4).
- Reinforces the need for **non-linear models** or **feature engineering**.

### 🔹 8. Monthly Loan Origination Trends
- Loan volume and disbursement amounts fluctuate monthly.
- Signs of **seasonal demand** or campaign-based boosts (e.g., festivals).

### 🔹 9. Loan Status by Customer Risk Category
- Low, Medium, and High risk groups show **similar loan status distributions**.
- High-risk group not significantly more likely to default — might suggest **risk categorization needs refinement**.

### 🔹 10. Loan Amount vs DPD (by Default Status)
- No visible clustering by default — default cases spread across the full range.
- Suggests **non-obvious default drivers**; may need clustering or decision trees.

### 🔹 11. Top 10 Cities by Default Rate
- One city stands out with a **default rate > 0.34**.
- Indicates a **regional risk hotspot** that may require further intervention or policy change.

## 📊 Visual Dashboard Sample

Visuals are generated using Seaborn/Matplotlib, covering:

- Loan Status Pie Chart
- Loan Amount Distribution
- DPD Boxplots
- Correlation Heatmap
- Loan Origination Time Series
- Customer Age Distribution
- Loan Status by Risk Category
- City-wise Default Rate Plot
- Loan Amount vs DPD Scatter (colored by default)

## 🤖 Machine Learning Model (Optional)

- **Logistic Regression** was used to predict the probability of loan default.
- Model accuracy: ~70%
- Features used: Age, Loan Amount, Tenure, DPD, Gender

## 🧠 Key Takeaways

- Males and customers with 5 or 35-month tenures have slightly higher default tendencies.
- Loan trends fluctuate monthly, hinting at seasonality.
- Current risk categorization may need improvement due to unexpected default rates across segments.
- City-level risk analysis highlights regional issues requiring focused policies.
- Default behavior is not linearly predictable — advanced modeling needed.
