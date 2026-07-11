# Data Dictionary

## Dataset Information

Dataset Name: gsearch_jobs.csv

Date Explored: 26-06-2026

Source: Kaggle (Google Jobs Dataset)

Purpose:
This dataset contains job postings collected from Google Jobs. The goal of this project is to analyze hiring trends, salary patterns, required skills, remote work opportunities, and geographic demand for Data Analyst roles.

## Observation 1

Columns 'Unnamed: 0' and 'index' contain sequential row numbers.

They do not describe any business information about the job postings.

Decision:
Keep them for now during the understanding phase.
They will likely be removed during the data cleaning phase.


# Column: title

Observation:
This column contains the job title for each posting. Most records are for Data Analyst roles, with variations such as Senior Data Analyst, Junior Data Analyst, Marketing Data Analyst, Healthcare Data Analyst, and Financial Data Analyst.

Business Use:
Used to analyze hiring demand by role and specialization.

Decision:
Keep


# Column: company_name

Observation:
There are 13,429 unique companies in the dataset. Upwork has the highest number of Data Analyst job postings.

Business Use:
This column can be used to identify the companies hiring the most Data Analysts and compare hiring demand across companies.

Decision:
Keep

# Column: location

Observation:
The dataset contains 1,254 unique locations. The most frequent value is "Anywhere", which likely represents jobs without a fixed physical location. The column also contains different location formats such as city and state names, state abbreviations (e.g., OK, MO), and remote indicators.

Business Use:
This column can be used to analyze geographic hiring demand and identify regions with the highest number of job opportunities.

Decision:
Keep

Future Action:
Standardize location values during the data cleaning phase.


## Data Quality Findings

### Duplicate Records
- No duplicate rows were found in the dataset.

### Missing Values
- The 'commute_time' column has 100% missing values and will be removed during the cleaning phase.
- Salary-related columns contain a high number of missing values because many job postings do not disclose salary information.
- Rows with missing salary values will not be removed, as doing so would discard a large portion of the dataset.


