# Automatidata TLC Data Inspection (Google Advanced Data Analytics - Course 1)

## Project overview
This project is part of the **Google Advanced Data Analytics Certificate** (Course 1 end-of-course project).

In this fictional scenario, Automatidata is working with the **New York City Taxi and Limousine Commission (TLC)** to support the future development of a fare estimation app. The goal of this first project stage is to **load, inspect, organize, and prepare the TLC dataset** for exploratory data analysis (EDA) and future regression modeling.

## Objectives
- Load and inspect TLC trip data in Python
- Build a working dataframe for the project
- Review and summarize column data types and non-null counts
- Identify initial data quality issues
- Prepare the dataset for future EDA
- Communicate findings in an executive-style summary

## Dataset
The dataset used in this project contains yellow taxi trip records and includes variables such as:
- pickup/dropoff datetime
- passenger count
- trip distance
- pickup/dropoff location IDs
- payment type
- fare amount
- total amount
- tip amount

> Note: This project scenario and dataset were provided for educational purposes in the course.

## Tools used
- Python
- pandas
- NumPy
- Jupyter Notebook

## Key preprocessing and inspection steps
- Loaded CSV data into a pandas dataframe
- Reviewed shape, column names, dtypes, and non-null counts
- Standardized mixed datetime formats in:
  - `tpep_pickup_datetime`
  - `tpep_dropoff_datetime`
- Inspected invalid/unusual values (e.g., out-of-range `RatecodeID`, negative fares/amounts)
- Applied initial filtering to support analysis-ready data preparation

## Initial findings
- Datetime columns were stored as object strings with mixed formats and required conversion
- No null values were found in the initial inspection
- Some records contained questionable values (e.g., negative fare amounts, outlier fare values)
- Additional validation and EDA are needed before model development

## Repository structure
```text
automatidata-tlc-data-inspection/
├── README.md
├── .gitignore
├── requirements.txt
├── notebooks/
│   └── Automatidata-QC.ipynb
└── data/
    └── 2017_Yellow_Taxi_Trip_Data.csv