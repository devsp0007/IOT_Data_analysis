# Credit Card Fraud Analysis Dashboard

## Project Description

This project performs an Exploratory Data Analysis (EDA) on the `creditcard1111.xlsx - creditcard.csv` dataset. Its primary goal is to identify patterns and characteristics of fraudulent transactions.

The Python script (`analysis.py`) automatically loads and cleans the data, performs a full analysis, and generates a single, consolidated 2x2 dashboard image named `fraud_dashboard.png`.

---

## Key Features & Analysis

The dashboard summarizes the four most critical insights from the dataset:

1.  **Overall Fraud Distribution:** A pie chart showing the severe class imbalance (Legit vs. Fraud) in the dataset.
2.  **Transaction Amount Analysis:** A box plot comparing the (log-transformed) monetary amounts of fraudulent vs. legitimate transactions.
3.  **Temporal Risk Analysis:** A bar chart showing the *percentage* of transactions that are fraudulent, broken down by the hour of the day.
4.  **Top Fraud Categories:** A horizontal bar chart identifying the top 10 most common transaction categories targeted by fraudsters.

---

## Key Insights from the Dashboard

The analysis reveals several classic fraud patterns:

* **Fraud is Rare:** The dataset is highly imbalanced, with fraudulent transactions making up a very small fraction (less than 1%) of the total.
* **Fraudulent Transactions are for Higher Amounts:** The box plot shows that the median amount for a fraudulent purchase is significantly higher than for a legitimate one.
* **Fraud Spikes at Night:** The *risk* of fraud (the percentage of transactions that are fraudulent) increases dramatically during the late-night and early-morning hours (approx. 10 PM - 4 AM), when the cardholder is likely asleep.
* **Fraud Targets Specific Categories:** Fraudsters appear to focus on specific categories (like `grocery_pos` and `shopping_net`), likely to purchase items that are easy to resell.

---

## How to Use

### 1. Dependencies

This script requires Python 3 and several libraries. You can install them using pip:

```bash
pip install pandas matplotlib seaborn numpy
