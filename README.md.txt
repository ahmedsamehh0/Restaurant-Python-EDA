# Restaurant Sales Data Analysis Project

## 📊 Project Overview
This project analyzes restaurant sales data to uncover business insights, customer behavior patterns, and sales trends. The analysis includes data cleaning, exploratory data analysis (EDA), and visualization of key metrics.

## 📁 Dataset Information
The dataset contains **17,534 orders** with the following columns:
- `Order ID` - Unique identifier for each order
- `Customer ID` - Unique identifier for each customer
- `Category` - Menu category (Main Dishes, Side Dishes, Desserts, Drinks)
- `Item` - Specific menu item ordered
- `Price` - Price per unit
- `Quantity` - Number of units ordered
- `Order Total` - Total amount for the order
- `Order Date` - Date of the order
- `Payment Method` - Payment type (Credit Card, Digital Wallet, Cash)

## 🎯 Project Objectives
1. Clean and preprocess raw sales data
2. Analyze sales trends over time
3. Identify most popular menu items and categories
4. Examine customer purchasing behavior
5. Analyze payment method preferences
6. Validate data integrity and consistency

## 🔧 Technical Stack
- **Python 3.8+**
- **Pandas** - Data manipulation and analysis
- **NumPy** - Numerical computations
- **Matplotlib** - Data visualization
- **Seaborn** - Statistical data visualization
- **Jupyter Notebook** - Interactive development environment

## 📈 Key Analysis Steps

### 1. Data Loading and Initial Exploration
- Loaded the dataset containing 17,534 rows and 9 columns
- Examined data types and structure
- Checked date range: Orders from Jan 1, 2022 to Dec 31, 2023 (729 days)

### 2. Data Cleaning
- **Missing Values Handled:**
  - Item: 1,758 missing
  - Price: 876 missing
  - Quantity: 430 missing
  - Order Total: 430 missing
  - Payment Method: 1,082 missing
- Removed rows with missing values
- Removed duplicate entries
- Converted `Order Date` to datetime format

### 3. Data Validation
- Created `calculated_total` column (Price × Quantity)
- Verified no mismatches between `Order Total` and `calculated_total`
- Summary statistics for numeric columns:
  - Average Price: $6.60
  - Average Quantity: 3.02 units
  - Average Order Total: $19.96

### 4. Data Analysis
#### Category Analysis:
- **Main Dishes**: Most revenue-generating category
- **Desserts**: Popular with consistent sales
- **Drinks**: Lower average price but high frequency
- **Side Dishes**: Frequently ordered with main dishes

#### Temporal Analysis:
- Sales trends across 2022-2023
- Seasonal patterns and monthly performance
- Daily sales distribution

#### Customer Behavior:
- Repeat customer analysis
- Average order value per customer
- Customer segmentation by purchase frequency

## 📊 Visualizations Created
1. **Category Distribution** - Bar chart showing sales by menu category
2. **Sales Trend Over Time** - Line chart of daily/monthly sales
3. **Top Selling Items** - Horizontal bar chart of most popular items
4. **Payment Method Distribution** - Pie chart showing payment preferences
5. **Price Distribution** - Histogram of price points

## 📋 Key Findings

### Business Insights:
1. **Revenue Optimization**: Main dishes contribute ~60% of total revenue
2. **Peak Seasons**: Highest sales during holiday seasons (Q4 2023)
3. **Customer Preferences**: Credit card is the most popular payment method (45%)
4. **Menu Performance**: Grilled Chicken and Pasta Alfredo are top sellers in Main Dishes
5. **Data Quality**: 8.7% of records had missing values requiring cleaning

### Recommendations:
1. **Menu Strategy**: Focus on promoting high-margin main dishes
2. **Inventory Management**: Stock up on popular items before peak seasons
3. **Payment Processing**: Optimize credit card transaction systems
4. **Customer Loyalty**: Implement rewards program for repeat customers
5. **Data Collection**: Improve data entry processes to reduce missing values

## 🚀 Getting Started

### Prerequisites:
- Python 3.8+
- Jupyter Notebook
- Required Python packages (see requirements.txt)