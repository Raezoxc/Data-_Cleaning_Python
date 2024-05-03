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

## Use of Code

- **Reading Data:** The script reads the customer call list data from the Excel file using pandas.

<img width="557" alt="image" src="https://github.com/Raezoxc/Data_Cleaning_Python/assets/153198226/edce457b-d9b3-472f-911c-2570b03a0c13">

- **Removing Duplicates:** Duplicate rows in the dataset are removed.

<img width="560" alt="image" src="https://github.com/Raezoxc/Data_Cleaning_Python/assets/153198226/5d80b3ff-7be4-45dd-b637-4b3f4537e0f9">

- **Removing Unnecessary Columns:** Certain columns, like 'Not_Useful_Column', are dropped from the DataFrame.

<img width="557" alt="image" src="https://github.com/Raezoxc/Data_Cleaning_Python/assets/153198226/cc5af4c8-031c-49dd-aa00-9325e1e511fe">

- **Cleaning Data:** 
    - The 'Last_Name' column is stripped of specific characters.
    - Non-digit characters in the 'Phone_Number' column are removed.
    - Phone numbers are formatted to follow the XXX-XXX-XXXX pattern.
    - Any remaining 'NaN' or empty values in the 'Phone_Number' column are handled.
    - Addresses are split into 'Street Address', 'State', and 'Zip Code' columns.
    - 'Paying Customer' and 'Do_Not_Contact' columns are standardized ('Yes' -> 'Y', 'No' -> 'N').
    - 'N/a' values are replaced with empty strings.
 
  <img width="555" alt="image" src="https://github.com/Raezoxc/Data_Cleaning_Python/assets/153198226/40a00c40-6f44-4dad-92a6-5ddb65a21d63">
  <img width="554" alt="image" src="https://github.com/Raezoxc/Data_Cleaning_Python/assets/153198226/8ab146b4-37c7-4960-ba18-605678bd3b6d">
  <img width="551" alt="image" src="https://github.com/Raezoxc/Data_Cleaning_Python/assets/153198226/b2c78076-0fb0-4a3e-b4b7-9a260a3a162e">
  <img width="554" alt="image" src="https://github.com/Raezoxc/Data_Cleaning_Python/assets/153198226/8ebb19d6-bc72-41f9-8c79-228edcf0db97">
  <img width="553" alt="image" src="https://github.com/Raezoxc/Data_Cleaning_Python/assets/153198226/fbfd6f7f-620e-4238-a003-ecf63b804337">
  <img width="549" alt="image" src="https://github.com/Raezoxc/Data_Cleaning_Python/assets/153198226/1fd42fd6-68eb-4062-a542-80696457c53d">
  <img width="551" alt="image" src="https://github.com/Raezoxc/Data_Cleaning_Python/assets/153198226/1babd077-e4f9-4d24-8ed6-c867210b6a92">
  <img width="544" alt="image" src="https://github.com/Raezoxc/Data_Cleaning_Python/assets/153198226/2f451499-eaa2-4c15-a40f-bef963a51b76">
  <img width="549" alt="image" src="https://github.com/Raezoxc/Data_Cleaning_Python/assets/153198226/a345b3ff-c6d0-4e7d-845d-99cde48c95e0">
  <img width="547" alt="image" src="https://github.com/Raezoxc/Data_Cleaning_Python/assets/153198226/45c68dda-576f-4975-aaa1-0a7541c90fcf">
 
  - **Data Filtering:**
    - Rows with 'Do_Not_Contact' flag set to 'Y' are removed.
    - Rows with empty phone numbers are removed.
   
    <img width="547" alt="image" src="https://github.com/Raezoxc/Data_Cleaning_Python/assets/153198226/882c8c52-d72b-423e-862f-beb13bf7c345">
    <img width="554" alt="image" src="https://github.com/Raezoxc/Data_Cleaning_Python/assets/153198226/c5509752-fbe4-438b-9cff-fd3d3aa5c887">

- **Data Reindexing:** The DataFrame index is reset to ensure sequential index values.
<img width="548" alt="image" src="https://github.com/Raezoxc/Data_Cleaning_Python/assets/153198226/b243de88-eea0-40e5-8503-cb509982b364">

   markdown
Copy code
## Saving Processed Data

After processing the customer call list data, you can save the cleaned and filtered DataFrame as a new CSV file using pandas.

# Save the processed DataFrame as a new CSV file
<img width="551" alt="image" src="https://github.com/Raezoxc/Data_Cleaning_Python/assets/153198226/29feb7da-57d0-4cc2-a727-dfc7f6c0ac0f">











## Output

The processed customer call list DataFrame is ready for further analysis or use.

## Author
Ravi Mhatre
