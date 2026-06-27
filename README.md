# Supply Chain Delivery Risk Analysis & Delay Prediction

## Overview

This project analyzes a global e-commerce supply chain dataset to identify delivery bottlenecks, understand the root causes of shipment delays, and build predictive models for delay risk.

The business problem focuses on inconsistent shipping performance, where actual delivery times frequently exceed scheduled timelines, leading to customer dissatisfaction and reduced profitability.

## Objectives

* Analyze delivery performance across regions, shipping modes, and product categories
* Detect operational bottlenecks causing shipment delays
* Identify key drivers affecting delivery time and profitability
* Forecast shipment patterns using time series analysis
* Build machine learning models to predict delayed deliveries

## Project Workflow

Exploratory Data Analysis (EDA) -> Diagnostic Analytics -> Time Series Analysis -> Predictive Modeling

## Key Insights

* Longer processing times strongly increase delay probability
* Certain shipping methods show consistently higher delay rates
* Delayed orders negatively impact profitability
* Delivery performance varies significantly across regions

## Tech Stack

* **Python**
* **Pandas**
* **NumPy**
* **Matplotlib / Seaborn**
* **Scikit-learn**

## Business Impact

This analysis helps supply chain teams:

* Reduce late deliveries
* Improve operational efficiency
* Optimize shipping decisions
* Increase customer satisfaction and profitability

## Repository Structure

```bash
├── data
├── notebooks
├── report
├── README.md
```
## Recommendations

Based on the analysis, the following actions are recommended to improve delivery performance and reduce profit loss:

* **Audit Premium Shipping Modes (Critical)**
  First Class has a **100% delay rate** and Second Class reaches **79.8%**, indicating major SLA failures. Reassess carrier performance and shipping route allocation.

* **Deploy Predictive Alert System (High)**
  The **Random Forest model (74% accuracy)** can be integrated into operations to identify high-risk orders before shipment and enable proactive intervention.

* **Optimize Payment Processing (High)**
  Orders under payment review show elevated delay risk. Automating payment validation and reducing approval bottlenecks can shorten fulfillment time.

* **Build Seasonal Capacity Plans (Medium)**
  Delay peaks occur during **August, September, and December**, suggesting capacity shortages during high-demand periods. Improve inventory planning and logistics staffing during these months.

* **Improve Shipping Assignment Logic (Medium)**
  Standard Class performs significantly better than premium modes in many cases. Shipping mode selection should prioritize historical route performance.

* **Reduce Loss-Making Orders (Low)**
  Around **18.7% of orders are loss-making**. Review pricing, discounts, and operational inefficiencies to improve margin performance.
