# E-commerce Sales Analysis Project

## Overview

This repository contains a synthetic e-commerce transaction dataset and an analysis notebook designed to demonstrate data analysis, visualization, and predictive modeling skills relevant for roles such as **Business Analyst**, **Data Analyst**, and **Program Manager**. The project is fully self-contained and can be run out of the box.

## Contents

- **synthetic_sales_dataset.csv** — A synthetic dataset of 1,000 e-commerce transactions. Each record includes customer demographics, transaction details, and a binary label indicating whether the transaction is a *high-value* purchase (purchase amount greater than 200).
- **sales_analysis.ipynb** — A Jupyter notebook that walks through the entire analysis pipeline:
  - Loading the dataset
  - Inspecting basic statistics and data types
  - Performing exploratory data analysis (EDA) with visualizations
  - Preprocessing the data (encoding categorical features)
  - Building and evaluating logistic regression and random forest models to classify high-value transactions
  - Discussing results and potential next steps
- **requirements.txt** — List of Python dependencies required to run the notebook.

## Getting Started

To run this project locally, follow these steps:

1. **Clone the repository** (or download it as a ZIP):
   ```bash
   git clone https://github.com/your-username/REPO_NAME.git
   cd REPO_NAME
   ```

2. **Create a virtual environment (optional but recommended)**:
   ```bash
   python3 -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scriptsctivate`
   ```

3. **Install dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

4. **Launch Jupyter Notebook**:
   ```bash
   jupyter notebook sales_analysis.ipynb
   ```

   or use `jupyter lab` if you prefer JupyterLab.

## Project Structure

```
.
├── synthetic_sales_dataset.csv
├── sales_analysis.ipynb
├── requirements.txt
└── README.md
```

## Dataset Details

The synthetic dataset simulates typical e-commerce transaction records. It includes the following columns:

| Column | Description |
|-------|-------------|
| `customer_id` | Unique identifier for the customer |
| `age` | Customer age in years |
| `gender` | Customer gender (Male, Female, Other) |
| `region` | Geographical region (North, South, East, West) |
| `product_category` | Category of the purchased product (Electronics, Clothing, Home & Kitchen, Sports, Books) |
| `purchase_date` | Date of purchase |
| `units_purchased` | Number of units purchased |
| `unit_price` | Price per unit |
| `purchase_amount` | Total purchase amount (units * unit_price + noise) |
| `return` | Indicates if the order was returned (1 = Yes, 0 = No) |
| `payment_method` | Payment method used |
| `high_value` | Target label: 1 if `purchase_amount` > 200; 0 otherwise |

## Notes

- The dataset is completely synthetic and does not represent real customer data.
- You can experiment with different models or feature engineering techniques to improve the classification performance.

## License

This project is released under the [MIT License](LICENSE).
