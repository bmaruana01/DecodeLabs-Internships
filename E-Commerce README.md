# E-Commerce Orders Data Analysis Project

##  Project Overview

This project performs a comprehensive data analysis of e-commerce order data to understand customer purchasing patterns, identify sales trends, detect anomalies, and uncover key business insights. The analysis includes statistical calculations, trend identification, outlier detection, and distribution analysis.

##  Key Objectives

- Calculate basic statistics (mean, median, count, standard deviation)
- Identify sales trends and patterns over time
- Detect outliers in order values and quantities
- Analyze distributions across key metrics
- Generate actionable business recommendations

##  Tools & Technologies Used

| Tool | Version | Purpose |
|------|---------|---------|
| **Python** | 3.12.12 | Primary programming language |
| **Pandas** | Latest | Data manipulation and analysis |
| **NumPy** | Latest | Numerical computations |
| **Matplotlib** | Latest | Data visualization |
| **Seaborn** | Latest | Statistical visualizations |
| **SciPy** | Latest | Outlier detection |
| **Jupyter Notebook** | Latest | Interactive development |

##  Dataset Information

### Data Source
E-Commerce Orders Dataset (cleaned)

### Dataset Size
- **Total Records:** 1,200 orders
- **Total Columns:** 14
- **Time Period:** January 1, 2023 - June 30, 2025 (911 days)

### Column Descriptions

| Column Name | Data Type | Description |
|-------------|-----------|-------------|
| `OrderID` | object | Unique identifier for each order |
| `Date` | datetime64[ns] | Order placement date |
| `CustomerID` | object | Unique customer identifier |
| `Product` | object | Name of purchased product |
| `Quantity` | int64 | Number of units ordered |
| `UnitPrice` | float64 | Price per unit in USD |
| `ShippingAddress` | object | Delivery address |
| `PaymentMethod` | object | Payment type used (online, credit card, debit card, gift card, cash) |
| `OrderStatus` | object | Current fulfillment status (Delivered, Shipped, Pending, Cancelled, Returned) |
| `TrackingNumber` | object | Shipping tracking ID |
| `ItemsInCart` | int64 | Total items in cart at checkout |
| `CouponCode` | object | Discount code applied (25.8% missing) |
| `ReferralSource` | object | How customer found the store (instagram, email, google, facebook, referral) |
| `TotalPrice` | float64 | Final order total after discounts |

##  Key Findings Summary

### Sales Metrics
- **Average Order Value:** $1,053.97
- **Median Order Value:** $823.62
- **Top Product (Revenue):** Chair ($195,620.11)
- **Product Distribution:** 7 unique products with balanced sales distribution

### Customer Behavior
- **Average Items Per Cart:** 5.5 items
- **Most Common Purchase Quantity:** 1 unit
- **Preferred Payment Method:** Online (21.5% of orders)
- **Primary Referral Source:** Instagram (21.6%)

### Operational Metrics
- **Order Completion Rate:** 19.2% (Delivered status)
- **Order Status Distribution:** 
  - Cancelled: 20.8%
  - Returned: 20.6%
  - Pending: 19.8%
  - Shipped: 19.6%
  - Delivered: 19.2%

### Data Quality
- **Data Completeness:** 98.3%
- **Missing Data:** Only CouponCode has missing values (25.8%)
- **Outliers Detected:** 8 high-value orders (0.7% of total)

### Revenue Distribution
- **68.1%** of orders exceed $500
- **19.9%** of orders fall in $200-500 range
- **6.8%** of orders fall in $100-200 range

### Monthly Trends (Last 6 Months)
| Month | Total Revenue | Order Count | Total Quantity |
|-------|--------------|-------------|----------------|
| Jan 2025 | $29,099.40 | 27 | 80 |
| Feb 2025 | $35,317.55 | 37 | 99 |
| Mar 2025 | $39,200.66 | 49 | 133 |
| Apr 2025 | $31,821.20 | 32 | 89 |
| May 2025 | $43,396.64 | 37 | 113 |
| Jun 2025 | $53,047.40 | 49 | 146 |

##  Visualizations Included

The analysis includes six key visualizations:
1. **Total Price Distribution** - Histogram of order values
2. **Daily Orders Trend** - Time series of order volume
3. **Top 10 Products by Revenue** - Bar chart
4. **Payment Method Distribution** - Pie chart
5. **Items Per Cart Distribution** - Bar chart
6. **Order Status Distribution** - Bar chart

##  How to Run the Analysis

### Prerequisites
```bash
pip install pandas numpy matplotlib seaborn scipy openpyxl
