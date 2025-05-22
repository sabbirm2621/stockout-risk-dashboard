# Stockout Risk Dashboard

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/sabbirm2621/stockout-risk-dashboard/blob/main/01_data_cleaning.ipynb)
This project analyzes inventory sales data to identify products at risk of stockouts. It includes a full pipeline from data cleaning to feature engineering and risk scoring — ideal for supply chain teams seeking better visibility into stockout patterns.

---

## Dataset

Synthetic inventory sales data simulating multiple products across stores:
- Sales performance
- Inventory levels
- Reorder points
- Lead times
- Promotion status

---

## Project Structure

| File                                | Description                            |
|-------------------------------------|----------------------------------------|
| `01_data_cleaning.ipynb`            | Loads and explores raw inventory data  |
| `02_feature_engineering.ipynb`      | Calculates custom features like:       |
|                                     | - Days of inventory left               |
|                                     | - At-risk flags                        |
|                                     | - Stockout risk scores (scaled 0–1)    |
| `03_stockout_risk_model.ipynb`      | Applies risk scoring and exports summary
| `inventory_sales_data.csv`          | Raw input dataset                      |
| `inventory_with_features.csv`       | Data after feature engineering         |
| `stockout_risk_summary.csv`         | Final output with stockout risk flags  |

---

## Key Features Engineered

- **Days of Inventory Left**: Estimates how many days each product will last
- **At-Risk Flag**: Binary flag if inventory < reorder point
- **Stockout Risk Score**: Scaled score between 0 (safe) and 1 (critical)

---

## Insights Enabled

- Detect vulnerable SKUs before stockouts occur
- Visualize risk over time
- Segment risk by product or store

---

## Tools Used

- Python
- Pandas & NumPy
- Matplotlib / Seaborn
- Google Colab

---

## Author

Built by Sabbir Ahamed — data analyst with an interest in supply chain intelligence & operational optimization.

