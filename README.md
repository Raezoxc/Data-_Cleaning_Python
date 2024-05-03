# Data_Cleaning_Python

# Customer Call List Processing

## Overview

This Python script utilizes the pandas library to process a customer call list stored in an Excel file format (.xlsx). The script performs various data cleaning and manipulation tasks to prepare the data for further analysis or use.

## Requirements

- Python 3.x
- pandas library

## Usage

1. Ensure you have Python installed on your system.
2. Install the required libraries by running `pip install pandas` in your terminal or command prompt.
3. Download the 'Customer Call List.xlsx' file and place it in the same directory as the Python script.

## Description

- **Reading Data:** The script reads the customer call list data from the Excel file using pandas.
- **Removing Duplicates:** Duplicate rows in the dataset are removed.
- **Removing Unnecessary Columns:** Certain columns deemed not useful are dropped from the DataFrame.
- **Cleaning Data:** 
    - The 'Last_Name' column is stripped of specific characters.
    - Non-digit characters in the 'Phone_Number' column are removed.
    - Phone numbers are formatted to follow the XXX-XXX-XXXX pattern.
    - Any remaining 'NaN' or empty values in the 'Phone_Number' column are handled.
    - Addresses are split into 'Street Address', 'State', and 'Zip Code' columns.
    - 'Paying Customer' and 'Do_Not_Contact' columns are standardized ('Yes' -> 'Y', 'No' -> 'N').
    - 'N/a' values are replaced with empty strings.
- **Data Filtering:**
    - Rows with 'Do_Not_Contact' flag set to 'Y' are removed.
    - Rows with empty phone numbers are removed.
- **Data Reindexing:** The DataFrame index is reset to ensure sequential index values.

## Output

The processed customer call list DataFrame is ready for further analysis or use.

## Author
Ravi Mhatre
