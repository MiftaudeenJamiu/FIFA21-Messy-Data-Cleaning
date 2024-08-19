# FIFA21-Messy-Data-Cleaning

## Table of Content
- Project Overview
- Issues Identified
- Data Cleaning Process: Key Steps
- Conclusion

## Project Overview 
This project focuses on the FIFA 21 Data Cleaning process. The initial dataset was quite messy and required thorough cleaning. Data cleaning is a vital step for any data enthusiast, as it prepares the data for accurate analysis or the development of machine learning models. This process ensures that the insights or models produced are reliable and not distorted by inconsistencies, errors, or imperfections in the data. The dataset, sourced from [Kaggle](https://www.kaggle.com/datasets/yagunnersya/fifa-21-messy-raw-dataset-for-cleaning-exploring), contains detailed information about football players and their performance, updated through 2021. Upon careful examination, several issues within the data were identified and systematically addressed.

## Issues Identified
- Missing Values
- Inconsistent Entries
- Incorrect Data Types
- Duplicate Records
- Spelling and Value Errors
- Irrelevant Data

## Data Cleaning Process: Key Steps
Here’s a summary of the cleaning process performed on the FIFA 21 dataset:

- Player Name Standardization:
Added a new column to store the cleaned and standardized version of player names.
Extracted player names from URLs and removed any special characters to ensure consistency in the `LongName` column.

- Contract Data Structuring:
Standardized the contract details by converting loan labels and free agents to a consistent format.
Created and populated new columns to store contract start and end years, along with a status column indicating whether the contract is active, on loan, or free.
Updated contract end dates for loaned players based on their loan end date.

- Club Name Cleaning:
Removed unwanted characters like dots and numbers from club names to maintain consistency.

- Height Standardization:
Converted height measurements from feet and inches to centimeters.
Removed the "cm" unit from the height values and rounded them to whole numbers.

- Weight Standardization:
Converted weight measurements** from pounds to kilograms.
Removed the "kg" unit from the weight values and rounded them to whole numbers.

- Value and Wage Standardization:
Converted abbreviated values (e.g., K for thousand, M for million) in the player value and wage columns to full numeric values for easier analysis.

- Release Clause Standardization:
Standardized the release clause amounts by removing symbols and converting them to numeric values.

- Cleaning Ratings Columns:
Removed special characters like stars from the columns representing ratings for Weak Foot, Skill Moves, and Injury Resistance.

- Hits Column Standardization:
Converted abbreviated hits (e.g., K for thousand) to full numeric values and rounded them to whole numbers.

- Duplicate Check:
Identified and counted duplicate records based on player IDs to ensure data integrity.

- Column Cleanup and Renaming:
Dropped unnecessary columns to streamline the dataset.
Added new columns with clear names to replace outdated ones, ensuring that the dataset is easier to work with and understand.

This cleaning process aimed to ensure consistency, accuracy, and clarity in the dataset, making it more suitable for analysis.
[The cleaned data](https://github.com/MiftaudeenJamiu/FIFA21-Messy-Data-Cleaning/blob/647eb7044a0e4dac86012a159545ad06f7644506/Cleaned_FIFA21_data.xlsx) is significantly different from the [original dataset](https://github.com/MiftaudeenJamiu/FIFA21-Messy-Data-Cleaning/blob/800f717cd5be12abe1fed645caa3aaeb9ff467bb/fifa21%20.xlsx) downloaded from Kaggle. After undergoing a thorough data cleaning process, the cleaned data is now free from inconsistencies, errors, and irrelevant information that were present in the raw data. Missing values have been addressed, duplicate entries removed, and data types corrected, resulting in a dataset that is more accurate and reliable. Additionally, spelling errors and value inconsistencies have been corrected, ensuring that the data is consistent and ready for meaningful analysis or model development. This transformation allows for more precise and trustworthy insights, clearly distinguishing the cleaned data from its original, unrefined state.
