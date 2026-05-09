# Customer Data Analysis

A comprehensive data analysis project exploring customer shopping behavior, demographics, and purchasing patterns. This repository contains exploratory data analysis notebooks, data preprocessing pipelines, and business intelligence visualizations.

## 📋 Project Overview

This project analyzes customer shopping behavior data to extract meaningful insights about purchasing patterns, customer demographics, seasonal trends, and product preferences. The analysis includes data exploration, feature engineering, and database integration for scalable data management.

## 📁 Project Structure

```
Customer Data Analysis/
├── Datasets/
│   └── customer_shopping_behavior.csv       # Main dataset
├── Basic_EDA.ipynb                          # Exploratory data analysis
├── Customer_Shopping_Behavior_Analysis.ipynb # Advanced analysis & preprocessing
├── Customer Behavior Analysis BI Report.pbix # Power BI dashboard
└── README.md                                # This file
```

## 📊 Analysis Dashboard Preview

![Customer Behavior Analysis Dashboard](Customer%20Behavior%20Analysis.png)

## 📊 Dataset Description

**File:** `customer_shopping_behavior.csv`

The dataset contains 3,900 records of customer transactions with 18 features:

### Customer Demographics
- **Customer ID**: Unique identifier for each customer
- **Age**: Customer age
- **Gender**: Male/Female
- **Location**: US state location

### Product Information
- **Item Purchased**: Specific product name
- **Category**: Product category (Clothing, Accessories, Outerwear, Footwear, etc.)
- **Size**: Product size (S, M, L, XL)
- **Color**: Product color

### Transaction Details
- **Purchase Amount (USD)**: Transaction amount
- **Season**: Shopping season (Spring, Summer, Fall, Winter)
- **Discount Applied**: Yes/No indicator
- **Promo Code Used**: Yes/No indicator
- **Shipping Type**: Standard, Express, 2-Day Shipping

### Customer Behavior
- **Frequency of Purchases**: Purchase frequency (Weekly, Monthly, Quarterly, Annually, etc.)
- **Previous Purchases**: Number of previous purchases
- **Subscription Status**: Active subscription indicator
- **Review Rating**: Customer rating (1-5 scale)
- **Payment Method**: Cash, Credit Card, Debit Card, Apple Pay, etc.

## 📓 Notebooks

### 1. **Basic_EDA.ipynb**
Performs initial exploratory data analysis including:
- Dataset shape and structure analysis
- Missing value detection
- Descriptive statistics (mean, median, std, etc.)
- Unique value counts for categorical variables
- Distribution analysis of numerical columns
- Visualizations:
  - Histograms for numerical features
  - Boxplots for purchase amount
  - Count plots for categories, gender, and season
  - Correlation heatmap
  - Age distribution with KDE

### 2. **Customer_Shopping_Behavior_Analysis.ipynb**
Advanced data analysis and preprocessing including:
- **Data Cleaning**: Missing value imputation using category-wise median for Review Ratings
- **Feature Engineering**: 
  - Age grouping into categories (Young Adult, Adult, Middle-aged, Senior)
  - Purchase frequency conversion to days (Fortnightly → 14 days, etc.)
  - Column standardization (snake_case naming convention)
- **Exploratory Analysis**: Summary statistics and data quality checks
- **Database Integration**: PostgreSQL connection setup for scalable data storage

## 🛠️ Technologies & Libraries

- **Python 3.11**
- **Pandas**: Data manipulation and analysis
- **NumPy**: Numerical computations
- **Matplotlib & Seaborn**: Data visualization
- **PostgreSQL**: Database integration (via SQLAlchemy)
- **Jupyter Notebook**: Interactive analysis environment
- **Power BI**: Business intelligence and dashboard creation

## 🚀 Getting Started

### Prerequisites
```bash
pip install pandas numpy matplotlib seaborn psycopg2-binary sqlalchemy jupyter
```

### Running the Analysis

1. **Clone/Download the repository**
   ```bash
   cd "Customer-Data-Analysis"
   ```

2. **Install dependencies**
   ```bash
   pip install -r requirements.txt  # If available
   ```

3. **Launch Jupyter Notebook**
   ```bash
   jupyter notebook
   ```

4. **Run the notebooks in order**
   - Start with `Basic_EDA.ipynb` for initial exploration
   - Follow with `Customer_Shopping_Behavior_Analysis.ipynb` for advanced analysis

### Database Setup (Optional)
To load data into PostgreSQL:

1. Update database credentials in the notebook:
   ```python
   username = "postgres"
   password = "your_password"
   host = "localhost"
   port = "5432"
   database = "your_database"
   ```

2. Run the PostgreSQL connection cells

## 📈 Key Insights & Analysis Areas

- **Customer Demographics**: Age distribution, gender breakdown, geographic distribution
- **Purchasing Patterns**: Frequency of purchases, average order value by category
- **Seasonal Trends**: Purchase behavior across seasons
- **Product Preferences**: Most popular categories and products
- **Discount Impact**: Effect of discounts and promo codes on purchases
- **Customer Loyalty**: Subscription status and review ratings
- **Payment Methods**: Popular payment options among customers

## 📊 Power BI Dashboard

The `Customer Behavior Analysis BI Report.pbix` file contains interactive visualizations and dashboards for business intelligence insights. Open with Microsoft Power BI Desktop.

## 🔍 Data Quality

- **Dataset Size**: 3,900 customer transactions
- **Missing Values**: Review Rating column (handled through median imputation by category)
- **Duplicates**: None identified
- **Outliers**: Present in purchase amounts (visible in boxplot analysis)

## 💡 Use Cases

- **Customer Segmentation**: Identify distinct customer groups for targeted marketing
- **Inventory Planning**: Optimize stock based on category and seasonal preferences
- **Pricing Strategy**: Analyze discount impact on purchase behavior
- **Marketing Campaigns**: Time campaigns around peak shopping seasons
- **Customer Retention**: Identify high-value customers and retention patterns

## 📝 Notes

- All monetary values are in USD
- Age is grouped into 4 quartile-based categories in advanced analysis
- Purchase frequency is standardized to days for mathematical operations
- The dataset is cleaned and preprocessed for analysis-ready format

## 📄 License

This project is provided for educational and analytical purposes.

## 📧 Contact

For questions or suggestions about this analysis, please reach out.

---

**Last Updated:** May 2026  
**Project Status:** Active
"# Customer-Data-Analysis" 
