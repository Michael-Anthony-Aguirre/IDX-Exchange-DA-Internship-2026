# IDX Exchange - Data Analyst Intern (Summer 2026)

## Overview
The following describes a data analyst internship for IDX Exchange revolving around Multiple Listing Service (MLS) analytics with Python and Tableau as the primary tools. This 12-week internship is divided into phases of data cleaning, market analytics, competitive intelligence, dashboard development, and market insights.

## How to Run
* Every single file has a "dataset_folder" string variable, which must be set to the path of the desired folder to have CSVs saved to.
* With few exceptions (check for "NOTES" in each week), this path should be exactly the same across all files.
* The order in which the files should be run is denoted by the number at the start of each file name (e.g., "1_aggregation.ipynb", "2_structuring-validation.ipynb", etc.).

## Week 0 - Retrieval
### Objectives
* Retrieve datasets from the California Regional Multiple Listing Service (CRMLS) on properties that have been listed (CRMLSListing) and sold (CRMLSSold).
* Datasets are exported as CSVs on a monthly basis from January 2024 to May 2026.

## Week 1 - Aggregation
### Objectives
* Aggregate the monthly CRMLSListing and CRMLSSold files into 2 datasets.
### NOTES
* In the code provided, the first instance of "dataset_folder" is set to "monthly data" subfolder within the "datasets" folder. The path is then set to the "datasets" folder itself in the very last block when saving the dataframes as CSVs. This is for organization purposes, separating the 60 monthly data CSVs from the primary CSVs of aggregated data that will be iterated upon going forward.

## Weeks 2-3 - Structuring & Validation
### Objectives
* Identify the proportion of missing values in each column, flagging columns with >90% missing values.
* Provide summary statistics for key numeric fields (ClosePrice, LivingArea, DaysOnMarket, etc.).
* Retrieve mortgage rate data (MORTGAGE30US) from FRED, resample the weekly rates to monthly averages, and merge the datasets on a "year_month" key basis.
* resample it from weekly to monthly frequency, and merge it onto both combined datasets using a year-month key derived from transaction dates)

## Weeks 4-5 - Data Cleaning & Preparation
### Objectives
* Convert date fields from string format to datetime format.
* Remove columns that are unnecessary or redundant.
* Appropriately handle missing values.
* Verify that numeric fields are formatted correctly.
* Flag rows with invalid numeric values, illogical date field order, and coordinate errors.

# Week 6 - Feature Engineering & Market Metrics (WIP)
### Objectives
* Create key metrics (price ratio, price per square foot, year-month, close-to-original-list ratio, listing-to-contract days, contract-to-close days) for later use in the development of Tableau dashboards.
* Add school district mapping using the latitude and longitude values of each property.
* Conduct analysis on market patterns by generating summary statistics based on segmented data (PropertyType & PropertySubType, CountyOrParish & MLSAreaMajor, ListOfficeName & BuyerOfficeName).
