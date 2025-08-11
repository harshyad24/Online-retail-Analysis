# Online Retail Analysis

A comprehensive data analysis project exploring transactional data from an online retail store specializing in gift items. This project provides insights into customer behavior, sales patterns, and business performance through exploratory data analysis and advanced analytics techniques.

## 📊 Dataset Overview

This analysis uses the Online Retail dataset containing **541,909 transactions** from a UK-based online retail company specializing in gift items. After data cleaning (removing 135,080 rows with missing CustomerID), the final dataset contains **397,924 transactions** from **4,339 unique customers** across **37 countries**.

**Dataset Period:** December 1, 2010 to December 9, 2011

### Key Dataset Statistics:
- **Total Revenue:** $8,911,407.90
- **Average Transaction Value:** $22.39
- **Countries Served:** 37 (primarily UK-based)
- **Unique Products:** 3,665 stock codes
- **Date Range:** 13 months of transaction data

### Dataset Features:
- `InvoiceNo`: Unique invoice identifier (18,536 unique invoices)
- `StockCode`: Product code (3,665 unique products)
- `Description`: Product description (3,877 unique descriptions)
- `Quantity`: Number of products purchased
- `InvoiceDate`: Transaction date and time
- `UnitPrice`: Product price per unit ($0.00 - $8,142.75)
- `CustomerID`: Unique customer identifier
- `Country`: Customer's country (37 countries)

## 🎯 Project Objectives

1. **Exploratory Data Analysis (EDA)**
   - Understand data structure and quality
   - Identify patterns in sales and customer behavior
   - Detect seasonal trends and anomalies

2. **Customer Analytics**
   - Customer segmentation and profiling
   - RFM (Recency, Frequency, Monetary) analysis
   - Customer lifetime value assessment

3. **Business Insights**
   - Revenue analysis and growth patterns
   - Product performance evaluation
   - Geographic market analysis
   - Return and cancellation analysis

4. **Advanced Analytics**
   - Market basket analysis
   - Customer churn prediction
   - Sales forecasting

## 🛠️ Tools and Technologies

- **Python 3.x**
- **Pandas** - Data manipulation and analysis
- **NumPy** - Numerical computing
- **Matplotlib & Seaborn** - Data visualization
- **Plotly** - Interactive visualizations
- **Scikit-learn** - Machine learning algorithms
- **Jupyter Notebook** - Development environment

## 📁 Project Structure

```
Online-retail-Analysis/
│
├── online_retail-2.ipynb    # Main analysis notebook
├── data/                    # Dataset files (if included)
├── images/                  # Generated plots and charts
├── requirements.txt         # Python dependencies
└── README.md               # Project documentation
```

## 🚀 Getting Started

### Prerequisites

Ensure you have Python 3.7+ installed along with the required packages:

```bash
pip install pandas numpy matplotlib seaborn plotly scikit-learn jupyter
```

### Installation

1. Clone this repository:
```bash
git clone https://github.com/harshyad24/Online-retail-Analysis.git
cd Online-retail-Analysis
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

3. Launch Jupyter Notebook:
```bash
jupyter notebook online_retail-2.ipynb
```

### Dataset Setup

The analysis uses the Online Retail dataset. The notebook handles data loading and preprocessing automatically. Key preprocessing steps include:

- Removal of transactions with missing CustomerID values
- Date parsing and temporal feature extraction  
- Revenue calculation (Quantity × UnitPrice)
- Data type conversions and validation

**Note:** The dataset contains 541,909 initial records, reduced to 397,924 valid transactions after cleaning.

## 📈 Key Findings and Insights

### 🌍 Geographic Analysis
- **United Kingdom** dominates with $7.3M revenue (82% of total sales) from 354,345 orders
- **Top International Markets:**
  - Netherlands: $285K revenue (avg. order: $120.80)
  - Germany: $229K revenue from 9,042 orders
  - France: $209K revenue from 8,342 orders
  - EIRE: $266K revenue from 7,238 orders

### 👥 Customer Insights
- **Top Customer** (ID: 14646): $280K total spent across 2,080 orders
- **Customer Distribution:** Highly concentrated with top customers generating significant revenue
- **Geographic Spread:** Active customers across 37 countries
- **Average Customer Value:** Varies significantly by region

### 🛍️ Product Performance
**Top Revenue Generators:**
1. **PAPER CRAFT, LITTLE BIRDIE:** $168K (80,995 units sold)
2. **REGENCY CAKESTAND 3 TIER:** $143K (12,412 units)
3. **WHITE HANGING HEART T-LIGHT HOLDER:** $100K (36,725 units)
4. **JUMBO BAG RED RETROSPOT:** $85K (46,181 units)
5. **MEDIUM CERAMIC TOP STORAGE JAR:** $81K (77,916 units)

### 📅 Temporal Patterns
- **Peak Sales Month:** September 2011 ($953K revenue)
- **Best Day of Week:** Thursday ($1.98M total sales)
- **Peak Sales Hour:** 12:00 PM ($1.38M total sales)
- **Seasonal Trends:** Strong holiday season performance

### 💰 Price Analysis
**Price Categories Performance:**
- **Low (<$2):** $3.6M revenue, 3.8M units (highest volume)
- **Medium ($2-5):** $3.5M revenue, 1.2M units
- **High ($5-10):** $1.1M revenue, 159K units
- **Premium (>$10):** $668K revenue, 38K units

### 🔍 Business Insights
- **Market Concentration:** Heavy reliance on UK market (82% of revenue)
- **Product Strategy:** Mix of high-volume low-cost and premium items
- **Customer Segmentation:** Few high-value customers drive significant revenue
- **Operational Timing:** Clear patterns in daily and hourly sales activity

## 🔍 Analysis Highlights

The notebook provides comprehensive analysis across multiple dimensions:

### 1. **Data Preprocessing & Quality Assessment**
- Cleaned dataset from 541,909 to 397,924 valid transactions
- Handled missing CustomerID values (135,080 removals)
- Date parsing and feature engineering (hour, day, month, year)
- Data validation and outlier identification

### 2. **Descriptive Statistics & Data Profiling**
- Complete statistical summary of numerical variables
- Data distribution analysis across all dimensions
- Missing value analysis and data quality metrics
- Unique value counts and data cardinality assessment

### 3. **Geographic Market Analysis**
- Revenue and order analysis across 37 countries
- Customer concentration by region
- Average order values by country
- Market penetration and opportunity identification

### 4. **Customer Behavior Analysis**
- Customer ranking by total spending and frequency
- Purchase pattern identification
- Customer value segmentation
- Loyalty and retention insights

### 5. **Product Performance Evaluation**
- Revenue-based product ranking
- Quantity-based bestsellers analysis
- Price point analysis across product categories
- Product portfolio optimization insights

### 6. **Temporal Pattern Analysis**
- Monthly sales trends and seasonality
- Daily and hourly sales pattern identification
- Peak performance periods
- Time-based forecasting opportunities

### 7. **Price Strategy Analysis**
- Price distribution and categorization
- Revenue impact by price segments
- Volume vs. value trade-offs
- Pricing optimization insights

### 8. **Visualization Dashboard**
- Interactive charts for sales trends
- Geographic distribution maps
- Customer and product performance rankings
- Time-series analysis plots
- Price category breakdowns

## 📊 Sample Visualizations

The analysis includes comprehensive visualizations:

### 📈 **Sales Trend Analysis**
- Monthly revenue trends showing peak performance in September 2011
- Daily sales patterns with Thursday as the best performing day
- Hourly sales distribution with peak at 12:00 PM

### 🌍 **Geographic Distribution**
- Country-wise revenue and order volume analysis
- Customer concentration maps
- International market performance comparison

### 🏆 **Performance Rankings**
- Top 10 products by revenue and quantity
- Customer spending leaderboards
- Country-wise market analysis

### 💰 **Price Category Analysis**
- Revenue distribution across price segments (Low, Medium, High, Premium)
- Volume vs. value analysis by price category
- Price optimization insights

### 📅 **Temporal Patterns**
- Seasonal sales patterns over 13-month period
- Day-of-week performance analysis
- Hourly transaction patterns for operational optimization

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request. For major changes, please open an issue first to discuss what you would like to change.

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👨‍💻 Author

**Harsh Yadav**
- GitHub: [@harshyad24](https://github.com/harshyad24)

## 🙏 Acknowledgments

- UCI Machine Learning Repository for providing the dataset
- The open-source Python community for the amazing tools and libraries
- Contributors and reviewers who helped improve this analysis

## 📞 Contact

For questions or suggestions regarding this project, please open an issue or reach out through GitHub.

---

*This project is for educational and analytical purposes, demonstrating data science techniques applied to retail analytics.*
