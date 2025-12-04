# HR Employee Attrition Analysis: End-to-End Deep Dive

## Project Overview
This project performs an end-to-end data analysis to investigate the factors driving **employee attrition** within a Human Resources dataset. The analysis follows a typical data science workflow, incorporating data loading, cleaning, feature engineering, Exploratory Data Analysis (EDA), and SQL-based analysis for deeper insight.

## Key Findings & Recommendations
The initial visual and statistical exploration highlighted strong correlations that were investigated further.

### 1. Key Attrition Drivers
* **Age and Tenure:** Younger employees and those with short tenure show the **highest flight risk**.
* **Compensation and Overtime:** **Low Monthly Income** and working **Overtime** are strongly associated with a higher attrition rate.
* **Satisfaction:** Low scores on **Environment Satisfaction** were a significant correlating factor.

### 2. Strategic Recommendations
* **Targeted Retention:** Focus retention efforts on **junior, short-tenure, and lower-income employees** who are identified as the highest-risk groups.
* **Compensation/Overtime Review:** Re-evaluate compensation and staffing levels, particularly for employees who work **Overtime**, to reduce the high associated attrition rate.
* **Performance/Promotion Pathway:** Develop clear development pathways for mid-career employees to improve tenure and performance.

## Methodology & Technologies
The analysis was conducted in several steps:

1.  **Data Retrieval & Cleaning:** The HR Attrition dataset was loaded and cleaned, including addressing outliers in columns like Monthly Income and Total Working Years.
2.  **Feature Engineering & EDA:** New features were created (e.g., `AgeGroup`, `IncomeBin`, `Tenure_Years`) to facilitate grouping and segmentation. Univariate and bivariate explorations were then performed.
3.  **SQL-Based Analysis:** The processed data was loaded into a SQLite database to run complex queries for deeper segmentation and rate calculation (e.g., Attrition Rate by Age Group).

### Technologies Used
* **Python:** pandas, numpy, seaborn, matplotlib.pyplot
* **Database:** SQLite
