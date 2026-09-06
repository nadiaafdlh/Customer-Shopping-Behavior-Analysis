
# Customer Shopping Behavior Analysis

End-to-end data analysis project covering exploratory data analysis, data cleaning, and an interactive Power BI dashboard, built on a synthetic customer shopping dataset from Kaggle.

## Project Background

Understanding what actually drives customer spending is a common challenge for retail businesses. Common assumptions — that subscriptions, discounts, or high review ratings automatically translate into higher spending — are often taken at face value without being tested against data. This project investigates whether these commonly held assumptions actually hold true, using a synthetic customer shopping dataset.

## Objective

This analysis was framed around five core business questions:
1. Does subscription status affect customer engagement and spending?
2. Does applying a discount increase transaction value?
3. Which products are most popular, and does popularity align with revenue contribution?
4. Does purchase frequency relate to spending behavior?
5. Does customer satisfaction (review rating) relate to purchase value?

## Dataset

- **Source**: [Customer Shopping Trends Dataset](https://www.kaggle.com/datasets/iamsouravbanerjee/customer-shopping-trends-dataset) — Kaggle (synthetic data, not from a real company)
- **Size**: 3,900 rows, 19 columns after cleaning
- **Key fields**: age, gender, category, item purchased, purchase amount, review rating, subscription status, discount applied, previous purchases, purchase frequency, location

## Tools & Process

| Stage | Tool |
|---|---|
| Data exploration & cleaning | Python (Pandas, Matplotlib,Seaborn) on Google Colab |
| Business & data understanding | Manual analysis based on 5 business questions |
| Dashboard & visualization | Power BI Desktop |

**Workflow**: Kaggle dataset → EDA & data cleaning (Google Colab) → business understanding & insight extraction → interactive dashboard (Power BI).

## Key Insights

- **Subscription status shows no meaningful effect on spending.** Average purchase amount is nearly identical between subscribers ($59.49) and non-subscribers ($59.87).
- **Discounts do not correlate with higher transaction value.** Discounted purchases do not show a higher average value than non-discounted ones.
- **Jeans is a clear underperformer** — it has both the lowest purchase count and the lowest revenue among all 25 products, standing well below the rest of the catalog.
- **Purchase frequency does not meaningfully affect spending** — customers across all frequency groups (Weekly to Annually) spend similarly on average.
- **Review ratings show virtually no correlation** with purchase amount or purchase history, meaning satisfaction scores should not be used as a proxy for customer value.
- The customer base skews heavily male (68% vs 32% female), and this imbalance means demographic findings should not be generalized.

## Business Recommendations

1. Re-evaluate the subscription program's value proposition.
2. Reassess the discount strategy — blanket discounting may not be the most effective approach.
3. Investigate Jeans specifically for a pricing, marketing, or assortment review.
4. Avoid relying on purchase frequency alone for customer segmentation.
5. Do not use review ratings as a proxy for customer value.
6. Expand future data collection to include transaction dates and quantities, enabling deeper analysis such as RFM or customer lifetime value.

## Limitations

- The dataset is **synthetic**, not sourced from a real company.
- Data is structured as **one row per customer**, not a full transaction history.
- **No transaction dates** are available — time-based trends, RFM, and CLV analysis are not possible.
- All findings are **associative, not causal**.
- Gender distribution is imbalanced (68% male / 32% female) and should not be generalized to a real population.

## Dashboard Preview

Screenshots of each dashboard page are available in the `/screenshots` folder:
- Executive Overview
- Demographics & Geography
- Subscription Engagement
- Promotion Strategy
- Product Performance
- Purchase Frequency
- Customer Experience
- Key Takeaways (Recommendations & Limitations)

## How to View the Dashboard

The `.pbix` file is included in the `/dashboard` folder. To explore it interactively:
1. Download Power BI Desktop (free) from Microsoft's website.
2. Open the `.pbix` file from the `/dashboard` folder.

*(A live web-hosted version may be added here later — see the linked video walkthrough in the meantime if available.)*

## Repository Structure

```
customer-shopping-behavior-analysis/
├── notebook/
│   └── Customer_Shopping_Behavior_Analysis_Update.ipynb
├── data/
│   └── customer_shopping_behavior_clean_Update.csv
├── dashboard/
│   └── Dashboard_Customer_Shopping_Behavior.pbix
├── screenshots/
│   └── (dashboard page screenshots)
└── README.md
```

## Author

Nadia Faadhillah
Undergraduate, Computer Engineering, Universitas Diponegoro
