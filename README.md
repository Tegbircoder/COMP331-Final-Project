# COMP331 Final Project – Data Quality & Bias Analysis  
**University of the Fraser Valley**  
**Student: Tegbir Singh**

---

## Project Overview  
This project analyzes the **Adult Income Dataset** from the UCI Machine Learning Repository to evaluate data quality issues and identify fairness and bias concerns in preparation for machine learning classification tasks.  
The dataset contains **32,537 records** describing demographic and employment features such as age, sex, race, education, workclass, and income level.

This work corresponds to **Option 2: Data Mining Quality & Bias Analysis** from the COMP 331 Final Project guidelines.

---

## Objectives  
This project evaluates data quality using three major dimensions:

### 1. **Completeness**  
Identifying missing values (e.g., “?” placeholders) and measuring how incomplete data affects analysis quality.

### 2. **Validity & Consistency**  
Checking whether:  
- Numeric values fall within logical ranges  
- Categories follow consistent formatting  
- Labels match expected patterns  
(Aligned with Week 10 concepts: ETL Cleaning & Standardization)

### 3. **Fairness & Bias**  
Measuring demographic imbalance and income inequality across sensitive groups:  
- **Sex** (Male vs Female)  
- **Race** (White, Black, Asian-Pac-Islander, etc.)

This connects to course topics from **Week 11: Bias, Fairness, Data Mining Ethics**.

---

## Dataset  
- **Source:** UCI Machine Learning Repository  
- **File Used:** `adult_clean.csv`  
- **Rows:** 32,537  
- **Columns:** 15  
- **Format:** CSV with added headers

---

## Bias Summary Tables  
### Sex Bias
| Group | Count | % of Dataset | >50K Income % |
|-------|--------|----------------|------------------|
| Male | 21,775 | 66.9% | 30.6% |
| Female | 10,762 | 33.1% | 10.9% |

### Race Bias
| Race Group | Count | % of Dataset | >50K Income % |
|------------|---------|----------------|------------------|
| White | 27,795 | 85.4% | 25.6% |
| Black | 3,122 | 9.6% | 12.4% |
| Asian-Pac-Islander | 1,038 | 3.1% | 26.6% |
| Amer-Indian-Eskimo | 311 | 1.0% | 11.5% |
| Other | 271 | 0.8% | 9.2% |

---

## Repository Structure  
COMP331-Final-Project/
│
├── data/
│ └── adult_clean.csv
│
├── notebooks/
│ └── placeholder.txt (Excel-based project – no code)
│
├── results/
│ ├── sex_bias_table.csv
│ └── race_bias_table.csv
│
└── README.md 

---

## Notes  
- This project uses **Excel** for analysis (no coding).  
- CSV output files in the `results/` folder contain the bias summary tables.  
- The final PDF report includes the full discussion, analysis, and recommendations.

---

## Status  
This repository contains all required components for the COMP331 Final Project.  


