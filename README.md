# Customer Segmentation & Retention Priority Analysis

**Scout AI — Data Scientist Intern Take-Home Assessment**
Submitted by Luke

## Business Question

Which customer segments are most valuable, which are at risk of churning, and how should retention budget be allocated across them?

## Files

| File | Description |
|---|---|
| `decision_memo.pdf` | 1-page decision memo — bottom line, findings, and recommendation for a fictional retention marketing stakeholder |
| `customer_segmentation_analysis.ipynb` | Full analysis notebook — data cleaning, EDA, RFM scoring, segmentation, and summary charts |

## Summary

Using RFM (Recency, Frequency, Monetary) analysis on 12 months of transaction data (4,338 customers, ~398K line items after cleaning), customers were grouped into six segments: Champions, Loyal Customers, At Risk, Needs Attention, Hibernating, and New Customers.

**Key finding:** Champions make up 22% of customers but generate 65% of revenue. The clearest retention opportunity is the At Risk segment — 10.5% of customers, ~$742K in historical revenue, who haven't purchased in 142 days on average despite a strong buying history.

**Recommendation:** Prioritize a win-back campaign for At Risk customers, protect Champions with light-touch loyalty perks, apply low-cost nurture to Needs Attention and New Customers, and deprioritize retention spend on Hibernating customers.

Full reasoning and caveats are in `decision_memo.pdf`.

## Data Source

[Online Retail II](https://www.kaggle.com/datasets/tunguz/online-retail-ii/data), Kaggle (Chen, London South Bank University). ~540K rows of UK-based online retail transactions, 01/12/2010–09/12/2011.

## Running the Notebook

The notebook expects `online_retail_II.csv` in the same directory. Requires `pandas`, `numpy`, and `matplotlib`.