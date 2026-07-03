# IDX Exchange - Data Analyst Intern (Summer 2026)

## Overview
The following describes a data analyst internship for IDX Exchange, a real estate technology companies, which revolves around Multiple Listing Service (MLS) analytics with Python and Tableau as the primary tools. This 12-week internship is divided into phases of data cleaning, market analytics, competitive intelligence, dashboard development, and market insights.

## Week 0 - Retrieval
### Objectives
* Retrieve datasets from the California Regional Multiple Listing Service (CRMLS) on properties that have been listed (CRMLSListing) and sold (CRMLSSold).
* Datasets are exported as CSVs on a monthly basis from January 2024 to May 2026.
### How to Run
* Not applicable.

## Week 1 - Aggregation
### Objectives
* Aggregate the monthly CRMLSListing and CRMLSSold files into 2 datasets.
### How to Run
Set the filepath of `os.chdir(r"...")` (Cell 1) to the folder containing the monthly CSV files. Upon completion, "CRMLSListing.csv" and "CRMLSSold.csv" will be output to the same folder.

## Week 2 - Structuring & Validation
### Objectives
* Identify the proportion of missing values in each column, flagging columns with >90% missing values.
* Provide summary statistics for key numeric fields (ClosePrice, LivingArea, DaysOnMarket, etc.).
* (WIP)
### How to Run
* Before running "file1.ipynb", ensure that "CRMLSSold.csv" and "CRMLSListing.csv" are also in the same folder (see "Week 1 - Aggregation").







