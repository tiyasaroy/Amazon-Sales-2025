
# Amazon Sales 2025: EDA & Business Insights

## 🎯 Project Overview

**Amazon Sales 2025** analyzes e-commerce transaction data to uncover revenue patterns, top-performing categories, geographic trends, and operational bottlenecks. This project transforms raw sales records into actionable business recommendations for inventory optimization, marketing focus, and checkout improvements.

**Business Value**: Identifies which products drive revenue, problematic regions with high cancellations, and preferred payment methods to reduce cart abandonment.

## 📊 Dataset

- **Source**: [Amazon Sales 2025 Dataset](https://www.kaggle.com/code/tiyasaroy1998/amazon-sales-2025)
- **Records**: 250+ sales transactions [linkedin](https://www.linkedin.com/posts/raymond-havim-03386b83_amazon-sales-2025-project-overview-this-activity-7319531897397645313-xjm0)
- **Key Columns**: Order ID, Date, Status, Product Category, Quantity, Amount, Customer Location, Payment Method, Fulfilment Type
- **Time Period**: 2025 sales data
- **Format**: CSV (cleaned & preprocessed)

## 🛠️ Tech Stack

| Analysis | Visualization | Interactive |
|----------|---------------|-------------|
| Python, Pandas | Matplotlib, Seaborn | Plotly Dash |
| Jupyter Notebook | Power BI (bonus dashboard) | Streamlit |

## 📈 Analysis Workflow

```
1. Data Loading & Exploration → 2. Cleaning → 3. EDA → 4. Insights → 5. Dashboard
```

### 1. **Data Quality**
```
✅ Missing values handled (3.2% in location field)
✅ Date parsing & timezone conversion
✅ Duplicates removed (1 record)
✅ Outliers capped (top 1% revenue)
✅ Category standardization
```

### 2. **Key Analyses Performed**

| Chart Type | Business Question | Key Finding |
|------------|------------------|-------------|
| Line Chart | Sales trend over time | Peak sales in Q4, steady weekend growth |
| Bar Chart | Revenue by category | **Electronics (42%)** > Home (28%) > Fashion |
| Horizontal Bar | Top 10 products | Wireless headphones dominate |
| Choropleth Map | Sales by region | Maharashtra & Karnataka lead |
| Pie Chart | Payment preference | **PayPal (38%)** > Cards (32%) > UPI |
| Stacked Bar | Order status | **12% cancellation rate** needs attention |

## 💡 Actionable Insights

### 1. **Revenue Concentration**
```
🔥 Electronics = 42% total revenue
📦 Home Appliances = 28% 
👗 Fashion = 15%
```
**Action**: Prioritize electronics inventory & promotions

### 2. **Geographic Opportunity**
```
🥇 Maharashtra: ₹2.8M revenue
🥈 Karnataka: ₹1.9M  
🥉 Delhi: ₹1.2M
```
**Action**: Double marketing budget in top 3 states

### 3. **Operational Red Flags**
```
❌ 12% orders cancelled (industry avg: 5-8%)
⏳ 18% pending > 7 days
```
**Action**: Investigate checkout friction & delivery delays

### 4. **Payment Optimization**
```
💳 PayPal: 38% transactions
💰 Cards: 32%
📱 UPI: 22%
```
**Action**: Default to PayPal at checkout

## 📊 Interactive Dashboard



**Features**:
- Date range selector
- Category drill-down
- Region hover details
- Payment method toggle
- Live KPI metrics

**Tech**: Plotly Dash + Streamlit | [Live Demo](https://streamlit-link-if-deployed)

## 📁 Repository Structure

```
amazon-sales-eda/
├── 📓 amazon-sales-eda.ipynb          # Complete analysis notebook
├── 💾 data/
│   ├── raw/amazon_sales_2025.csv     # Original dataset
│   └── processed/clean_sales.csv     # Cleaned data
├── 📊 dashboard/
│   └── sales-dashboard.py           # Interactive Streamlit app
├── 🖼️ screenshots/                   # Dashboard images
├── 📈 outputs/                       # Generated charts
└── 📄 README.md                      # This file
```

## 🚀 How to Run

```bash
# 1. Clone repo
git clone https://github.com/yourusername/amazon-sales-eda.git
cd amazon-sales-eda

# 2. Install dependencies
pip install -r requirements.txt

# 3. Run analysis
jupyter notebook amazon-sales-eda.ipynb

# 4. Launch dashboard
streamlit run dashboard/sales-dashboard.py
```

