# Building a Robust Data Auditing Workflow in Spreadsheets

## Project Overview
When running a large-scale data analysis, silent spreadsheet bugs can severely compromise the accuracy of your results. This project walks through a step-by-step production workflow to structure, audit, clean, and analyze an environmental dataset containing 100 industrial facility emission records. 

By implementing strict validation methods, formatting rules, and modern lookup functions, this framework ensures 100% data integrity before insights are generated.

## Dataset Architecture
The workflow utilizes a dataset containing 8 core attributes:
* `YEAR` (Numeric)
* `FACILITY_NAME` (Text)
* `CITY` (Text)
* `COUNTY` (Text)
* `STATE` (Text)
* `CHEMICAL` (Text)
* `UNIT_OF_MEASURE` (Text)
* `TOTAL_RELEASES` (Numeric)

## Comprehensive Documentation Modules
To view the direct technical implementations, browse the modules below:
1. [Module 1: Structural Setup & Alignment Validation](01_Data_Validation.md)
2. [Module 2: Diagnostic Testing & Data Cleaning](02_Data_Cleaning.md)
3. [Module 3: Aggregations & Descriptive Analytics](03_Descriptive_Analysis.md)
4. [Module 4: Advanced Lookups using XLOOKUP](04_Advanced_Lookups.md)
