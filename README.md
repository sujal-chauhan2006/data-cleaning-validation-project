# Data Validation Pipeline for Customer Dataset

## Overview

This project demonstrates how to handle and clean messy real-world data using Python. It focuses on building a complete data validation pipeline including parsing, cleaning, validation, and reporting.

---

## Problem Statement

The dataset contains multiple data quality issues such as:

* Missing values (customer_id)
* Incorrect data types (e.g., age as text)
* Invalid values (age out of range, wrong dates)
* Inconsistent formats (price, phone numbers)
* Malformed CSV rows (commas inside values)

---

## Solution Approach

The pipeline is divided into the following steps:

1. Custom CSV Parsing
   Handles malformed rows using regex-based splitting.

2. Data Cleaning
   Converts data types (age, price, date) and standardizes formats (email lowercase, phone digits only).

3. Validation
   Applies rules such as:

   * Age between 0–120
   * Valid email format
   * Valid date format
   * Required field checks

4. Error Handling
   Invalid rows are captured with error messages. Clean and invalid data are stored separately.

5. Quality Metrics

   * Clean rate
   * Number of rejected rows
   * Type errors fixed
   * Format standardization count

---

## Output Files

* clean_customers.csv — Clean dataset
* validation_errors.csv — Error report
* validation_report.txt — Summary report

---

## Technologies Used

* Python
* Pandas
* Regular Expressions (re)

---

## Key Learnings

* Handling real-world messy data
* Building validation pipelines
* Data preprocessing before machine learning
* Importance of data quality

---

## Conclusion

This project highlights the importance of data cleaning and validation in real-world scenarios. A well-structured preprocessing pipeline ensures better data quality and improves downstream analysis and model performance.
