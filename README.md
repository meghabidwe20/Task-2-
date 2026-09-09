# Task 2: Sales Data Analysis

## Dataset
The **Cleaned Data** sheet contains 67 transaction rows, 65 unique Order IDs, and 5 unique customers. The cleaning workbook states that repeated Order IDs were reviewed and retained as valid entries.

## KPI Summary

| KPI | Result |
|---|---:|
| Total Revenue | 17,090.07 |
| Total Orders / Transactions | 67 |
| Unique Order IDs | 65 |
| Average Order Value | 255.08 |
| Total Units Sold | 820 |
| Top-Selling Category | Toys |
| Best Revenue-Generating Product | Ceiling Fan |

**Note:** The dataset has 67 transaction rows but 65 unique Order IDs. The main AOV uses the 67 retained transaction rows, while AOV by unique Order ID would be 262.92.

## 8 Key Observations

1. Total revenue is **17,090.07** across the 67 retained transaction rows.
2. **Toys** is the top revenue category at **3,712.18**, contributing **21.7%** of revenue.
3. **Home & Kitchen** ranks second at **3,541.27**; the two leading categories together contribute **42.4%**.
4. **Ceiling Fan** is the highest revenue-generating product at **490.77**.
5. **Backpack** has the highest unit volume at **80 units**, showing that volume leadership and revenue leadership can differ.
6. **August 2024** is the strongest month, with revenue of **4,525.08**.
7. The top three customers generate **16,544.73**, approximately **96.8%** of total revenue, indicating strong customer concentration.
8. **North** has the highest revenue among the City/Region values at **1,896.79**.

## Trend-Based Interpretation

Revenue is highly uneven across months. August is the peak month at **4,525.08**, while revenue falls in September, October, and November. This pattern matters because planning based on an average month could understate the variability in sales performance. The dataset shows the pattern but does not establish the cause, so seasonality, promotions, product mix, or other explanations should be investigated rather than assumed.

## Customer Insights

- There are **5 unique customers**.
- Customer **17850** contributes the highest revenue (**7,373.45**) and has the highest transaction count (**28**).
- Customer **12583** records the highest unit volume (**449 units**).
- Customers **17850, 12583, and 13047** account for approximately **96.8%** of revenue.
- Two customers appear only once in the transaction data, while the other three customers account for most activity.

## Recommendations

1. Investigate the factors behind the August peak before treating it as a repeatable seasonal pattern.
2. Monitor Toys and Home & Kitchen closely because they are the two largest revenue categories.
3. Use retention and cross-selling strategies for high-value repeat customers because revenue is concentrated among a small customer base.
4. Track both revenue and units: high-volume products such as Backpack and high-revenue products such as Ceiling Fan represent different types of product performance.

## Execution

```bash
pip install pandas openpyxl matplotlib
python Sales_Data_Analysis.py
```

