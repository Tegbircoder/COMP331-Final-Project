# COMP331 Final Project - Data Quality Analysis

## Author
Tegbir Singh

## Project Overview
This project analyzes data quality issues in the Global Superstore dataset from a data warehousing perspective, focusing on completeness, consistency, and validity dimensions.

## Dataset
- **Name:** Global Superstore Dataset
- **Records:** 51,290 transactions
- **Download:** [Kaggle - Global Superstore](https://www.kaggle.com/datasets/shekpaul/global-superstore)

## Repository Structure
```
├── results/
│   ├── data_quality_issues.png
│   └── summary.txt
├── analysis.ipynb
└── README.md
```

## Key Findings

### 1. Completeness: 100%
- No missing values found in any column

### 2. Consistency Issues Found
- **457 Product IDs** have multiple different Product Names
- This creates **476 duplicate dimension records**
- Example: Product ID `FUR-BO-10000087` has 2 different names

### 3. Validity: All Valid
- All categorical values follow business rules
- All dates are logically correct

## Data Warehousing Impact
The product inconsistency violates star schema design principles:
- DIM_PRODUCT table would have duplicate records
- Referential integrity would be compromised
- Business reports would be unreliable

## Tools Used
- Python 3
- pandas, matplotlib
- Jupyter Notebook
- Claude AI (for code assistance)

## Course
COMP331 - University of the Fraser Valley - Fall 2025
