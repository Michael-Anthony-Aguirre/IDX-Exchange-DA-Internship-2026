# IDX Exchange - Data Analyst Intern (Summer 2026)

## Overview
The following describes a data analyst internship for IDX Exchange revolving around Multiple Listing Service (MLS) analytics with Python and Tableau as the primary tools. This 12-week internship is divided into phases of data cleaning, market analytics, competitive intelligence, dashboard development, and market insights.

## Week 0 - Retrieval
### Objectives
* Retrieve datasets from the California Regional Multiple Listing Service (CRMLS) on properties that have been listed (CRMLSListing) and sold (CRMLSSold).
* Datasets are exported as CSVs on a monthly basis from January 2024 to May 2026.

## Week 1 - Aggregation
### Objectives
* Aggregate the monthly CRMLSListing and CRMLSSold files into 2 datasets.
### How to Run
Set the filepath of `os.chdir(r"...")` (Cell 1) to the folder containing the monthly CSV files. "CRMLSListing_1.csv" and "CRMLSSold_1.csv" will be output to the same folder as the other CSVs.

## Weeks 2-3 - Structuring & Validation
### Objectives
* Identify the proportion of missing values in each column, flagging columns with >90% missing values.
* Provide summary statistics for key numeric fields (ClosePrice, LivingArea, DaysOnMarket, etc.).
* Retrieve mortgage rate data (MORTGAGE30US) from FRED, resample the weekly rates to monthly averages, and merge the datasets on a "year_month" key basis.
* resample it from weekly to monthly frequency, and merge it onto both combined datasets using a year-month key derived from transaction dates)
### How to Run
* Before running "file1.ipynb", ensure that "CRMLSListing_1.csv" and "CRMLSSold_1.csv" are also in the same folder. Output will include "CRMLSListing_2.csv" and "CRMLSSold_2.csv".
* "file2.ipynb" requires "CRMLSListing_2.csv" and "CRMLSSold_2.csv", it can be run immediately after "file1.ipynb" has completed.

## Weeks 4-5 - Data Cleaning & Preparation (WIP)
### Objectives
* (WIP)
### How to Run
* (WIP)





