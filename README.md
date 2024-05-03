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

    <img width="557" alt="image" src="https://github.com/Raezoxc/Data_Cleaning_Python/assets/153198226/4dc290e2-6ca1-4644-ac11-04bc422d75d8">

- **Removing Duplicates:** Duplicate rows in the dataset are removed.

    <img width="551" alt="image" src="https://github.com/Raezoxc/Data_Cleaning_Python/assets/153198226/27af6cf2-af23-4f08-ad06-70e1ae16cabe">

- **Removing Unnecessary Columns:** Certain columns, like 'Not_Useful_Column', are dropped from the DataFrame.

    <img width="540" alt="image" src="https://github.com/Raezoxc/Data_Cleaning_Python/assets/153198226/1462d652-f6bb-4425-8aa5-80a595d8e701">

- **Cleaning Data:** 

    - The 'Last_Name' column is stripped of specific characters.
    <img width="545" alt="image" src="https://github.com/Raezoxc/Data_Cleaning_Python/assets/153198226/d363f762-a3ac-4940-abea-528567225187">

    - Non-digit characters in the 'Phone_Number' column are removed.
    <img width="542" alt="image" src="https://github.com/Raezoxc/Data_Cleaning_Python/assets/153198226/fc63f616-e562-4365-b051-761e405edf6d">

    - Phone numbers are formatted to follow the XXX-XXX-XXXX pattern.
    <img width="536" alt="image" src="https://github.com/Raezoxc/Data_Cleaning_Python/assets/153198226/b144239e-c14c-48f8-9c3b-685581ec6978">

    - Any remaining 'NaN' or empty values in the 'Phone_Number' column are handled.
    <img width="559" alt="image" src="https://github.com/Raezoxc/Data_Cleaning_Python/assets/153198226/ab9f1725-7ca6-4473-9b7d-7176e4b60725">
    <img width="547" alt="image" src="https://github.com/Raezoxc/Data_Cleaning_Python/assets/153198226/e2922320-851a-4ec0-a3a9-1e3d495a19fe">


    - Addresses are split into 'Street Address', 'State', and 'Zip Code' columns.
    <img width="546" alt="image" src="https://github.com/Raezoxc/Data_Cleaning_Python/assets/153198226/04ba240e-a66c-451d-b4d9-b1e2a95b63fe">

    - 'Paying Customer' and 'Do_Not_Contact' columns are standardized ('Yes' -> 'Y', 'No' -> 'N').
    <img width="544" alt="image" src="https://github.com/Raezoxc/Data_Cleaning_Python/assets/153198226/6140e852-b55f-4c1b-8c8e-129bf652a4a4">
    <img width="549" alt="image" src="https://github.com/Raezoxc/Data_Cleaning_Python/assets/153198226/6b0055a4-7f94-4c53-a516-674990e425a1">


    - 'N/a' values are replaced with empty strings.
    <img width="545" alt="image" src="https://github.com/Raezoxc/Data_Cleaning_Python/assets/153198226/5792db9d-0385-403d-a344-3b9844cb4cfc">
    <img width="543" alt="image" src="https://github.com/Raezoxc/Data_Cleaning_Python/assets/153198226/faf1f624-08b4-44d5-baf1-7fa80d0e0cc2">

- **Data Filtering:**
    
    - Rows with 'Do_Not_Contact' flag set to 'Y' are removed.
    <img width="545" alt="image" src="https://github.com/Raezoxc/Data_Cleaning_Python/assets/153198226/efc5faf0-950a-4256-a9b5-5e6742356ffb">

    - Rows with empty phone numbers are removed.
    <img width="547" alt="image" src="https://github.com/Raezoxc/Data_Cleaning_Python/assets/153198226/1c60f5a5-afea-4b23-975f-0254554bf6dd">

- **Data Reindexing:** The DataFrame index is reset to ensure sequential index values.
    <img width="545" alt="image" src="https://github.com/Raezoxc/Data_Cleaning_Python/assets/153198226/91625901-d496-47b0-a93a-3b1afa063e64">


## Saving Processed Data

After processing the customer call list data, you can save the cleaned and filtered DataFrame as a new CSV file using pandas.

# Save the processed DataFrame as a new CSV file
     <img width="551" alt="image" src="https://github.com/Raezoxc/Data_Cleaning_Python/assets/153198226/abb23cd8-82ce-455f-891c-2403d986bc4a">


