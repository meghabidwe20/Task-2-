# Sales Data Analysis

## Week 1 – Task 2

### Project Objective

The objective of this project is to analyze an e-commerce sales dataset to understand business performance, identify sales trends, evaluate product and category performance, and generate customer-focused business insights.

The analysis focuses on calculating key performance indicators (KPIs), identifying important sales trends, comparing regional performance, and understanding delivery-status patterns.

---

## Dataset Description

The dataset used for this project is an e-commerce sales dataset containing transactional information.

### Main Features

* Order ID
* Date
* Status
* Fulfilment
* Sales Channel
* ship-service-level
* Style
* SKU
* Category
* Size
* ASIN
* Courier Status
* Qty
* currency
* Amount
* ship-city
* ship-state
* ship-postal-code
* ship-country
* B2B

The dataset contains approximately 129,000 sales records.

---

## Tools and Technologies Used

* **Python**
* **Pandas** – Data cleaning and analysis
* **NumPy** – Numerical calculations
* **Matplotlib** – Data visualization
* **Jupyter Notebook** – Analysis and documentation
* **Microsoft Excel** – Dataset inspection and validation

---

## Key Steps Performed

### 1. Data Loading

The sales dataset was imported into Python using Pandas.

### 2. Data Preparation

The following preparation steps were performed:

* Checked dataset structure and column names.
* Converted the Date column into datetime format.
* Converted Amount and Qty into numeric values.
* Checked for missing values.
* Reviewed duplicate and invalid records.
* Examined different order and delivery statuses.

### 3. Completed Sales Filtering

For the main KPI analysis, records with the status:

**`Shipped - Delivered to Buyer`**

were treated as completed sales.

Cancelled, pending, returned, and other non-completed statuses were excluded from the completed-sales KPI calculations.

### 4. KPI Calculation

The following KPIs were calculated:

* Total Revenue
* Total Orders
* Average Order Value
* Total Units Sold
* Top-Selling Category
* Best Revenue-Generating Product

### 5. Trend Analysis

Sales were analyzed across time to identify:

* Monthly revenue trends
* Monthly order trends
* Sales growth and decline
* Highest and lowest performing months
* Category performance over time

### 6. Regional Analysis

Sales and order performance were analyzed by:

* State
* City
* Order density
* Revenue contribution

### 7. Delivery Status Analysis

Different delivery and order statuses were compared to understand their effect on revenue realization.

### 8. Customer Insights

Customer-related patterns were explored using available fields such as city, state, category, order frequency, and B2B status.

---

## KPI Summary

| KPI                 |      Result |
| ------------------- | ----------: |
| Total Revenue       | ₹18,650,815 |
| Total Orders        |      26,566 |
| Average Order Value |     ₹702.06 |
| Total Units Sold    |      28,886 |
| Top Category        |         Set |
| Best Product/Style  |     JNE3797 |

---

## Major Findings

1. The business generated approximately **₹18.65 million** in completed sales revenue.

2. The average completed order value was approximately **₹702**.

3. The **Set category** was the highest revenue-generating category, contributing approximately **47.19%** of completed revenue.

4. **Set, kurta, and Western Dress** together contributed more than **93% of completed revenue**, indicating strong sales concentration in these categories.

5. **April recorded the highest completed sales revenue**, with approximately **₹5.63 million** in revenue.

6. Sales declined significantly after April, with substantial decreases during May, June, and July.

7. **Maharashtra** generated the highest state-level completed revenue.

8. **Bengaluru** recorded the highest completed-order density among cities.

9. **JNE3797** was the highest revenue-generating product/style.

10. The dataset contains significant cancelled and non-delivered orders, making delivery-status monitoring important for revenue realization.

---

## Trend-Based Interpretation

April was the strongest sales month, with completed revenue reaching approximately ₹5.63 million. This represented a significant increase compared with March.

However, sales declined considerably after April. This suggests that the April increase may have been influenced by temporary factors such as promotions, seasonal demand, product availability, or marketing campaigns.

### Business Recommendation

The business should investigate the factors responsible for the April sales spike and determine which successful strategies can be repeated during lower-performing months.

---

## Customer Insights

The dataset does not contain a dedicated **Customer ID** field. Therefore, the following customer-level metrics cannot be reliably calculated:

* Repeat customer rate
* Unique customer count
* Customer lifetime value
* Revenue from repeat customers
* Individual customer purchase frequency

However, location-based and product-based customer insights can still be generated.

### Key Customer Insights

* Bengaluru had the highest completed-order density.
* Maharashtra was the highest-revenue state.
* Set was the most preferred/highest-revenue category.
* High sales were concentrated in a relatively small number of categories.
* Future datasets should include a reliable Customer ID to enable detailed customer segmentation and repeat-purchase analysis.

---

## Recommendations

* Maintain sufficient inventory for high-performing categories such as **Set, kurta, and Western Dress**.
* Investigate the reasons behind the exceptional April sales performance.
* Develop promotional strategies to reduce the sharp sales decline after peak periods.
* Focus marketing efforts on high-performing states and cities.
* Monitor cancelled and returned orders to reduce revenue leakage.
* Promote high-performing products such as **JNE3797**.
* Add Customer ID information to future datasets for better customer-level analysis.

---

## Project Folder Structure

```text
Sales-Data-Analysis/
│
├── README.md
│
├── data/
│   ├── raw/
│   │   └── Sales Data Analysis.xlsx
│   │
│   └── cleaned/
│       └── cleaned_sales_data.xlsx
│
├── notebooks/
│   └── Sales_Data_Analysis.ipynb
│
├── scripts/
│   └── sales_analysis.py
│
├── outputs/
│   ├── kpi_summary.csv
│   ├── category_analysis.csv
│   ├── monthly_sales.csv
│   ├── regional_analysis.csv
│   └── product_analysis.csv
│
└── visuals/
    ├── monthly_sales_trend.png
    ├── category_revenue.png
    └── regional_sales.png
```

---

## How to Run the Project

### Step 1: Install Required Libraries

```bash
pip install pandas numpy matplotlib openpyxl jupyter
```

### Step 2: Open the Project

Navigate to the project directory:

```bash
cd Sales-Data-Analysis
```

### Step 3: Start Jupyter Notebook

```bash
jupyter notebook
```

### Step 4: Open the Notebook

Open:

```text
notebooks/Sales_Data_Analysis.ipynb
```

### Step 5: Run the Notebook

Run all cells from top to bottom to reproduce the analysis, KPI calculations, tables, and visualizations.

---

## Important Methodology

For the primary KPI analysis, only orders with the status:

```text
Shipped - Delivered to Buyer
```

were considered completed sales.

This approach prevents cancelled, pending, returned, or otherwise incomplete transactions from being incorrectly counted as completed revenue.

---

## Limitations

* The dataset does not contain a Customer ID.
* Detailed repeat-customer analysis is therefore not possible.
* Some records contain missing values.
* Different order statuses represent different stages of fulfillment.
* Revenue should not be interpreted solely from the Amount field without considering order status.

---

## Conclusion

The sales analysis demonstrates that business revenue is concentrated in a few major product categories and regions. The Set category was the strongest contributor to revenue, while April was the strongest sales month.

The significant decline following April highlights the need for consistent demand-generation strategies. Regional analysis also indicates opportunities to focus marketing and inventory planning on high-performing locations.

Overall, the analysis provides actionable insights into **sales performance, product demand, regional performance, delivery status, and customer behavior**.

---

## Author

**Name:** Megha Bidwe
**Project:** Sales Data Analysis
**Task:** Week 1 – Task 2
**Tools:** Python, Pandas, NumPy, Matplotlib, Jupyter Notebook, Excel
