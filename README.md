# COMP331 Final Project – Data Quality & Bias Analysis  
**University of the Fraser Valley**  
**Student: Tegbir Singh**

---

## Project Overview  
The Adult Income dataset (32,537 rows) from the UCI Machine Learning Repository is examined for data quality in this study. The dataset's demographic, employment, and income-related characteristics are used to forecast whether a person makes more than $50,000 a year. Because model accuracy, fairness, and ethical reliability are directly impacted by missing values, discrepancies, and demographic imbalances, data quality is essential. In accordance with course principles from Weeks 10 (ETL and Data Warehousing) and 11 (Data Mining, Bias, and Fairness), this report assesses three fundamental aspects of data quality: completeness, validity/consistency, and fairness/bias. 

This work corresponds to **Option 2: Data Mining Quality & Bias Analysis** from the COMP 331 Final Project guidelines.

---

## Objectives  
This project evaluates data quality using three major dimensions:

### 1. **Completeness**  
Three properties have significant gaps, according to a search for missing values and placeholder "?" symbols: 
### 2. **Validity & Consistency**  

Income labels (<=50K, >50K) were consistent, and numerical ranges (e.g., age 18–90, no negatives) were valid. Although there were no structural irregularities discovered, standardization—such as removing spaces and using consistent formatting—is still required to guarantee long-term data integrity. These actions are in line with ETL standardization procedures. 

### 3. **Fairness & Bias**  
A demographic analysis revealed significant sampling bias and historical bias, directly tied to Week 11 concepts. -

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

## Status  
This repository contains all required components for the COMP331 Final Project.  


