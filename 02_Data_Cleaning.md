# Module 2: Diagnostic Testing & Data Cleaning

A major flaw in basic spreadsheet tools is that standard mathematical aggregations silently ignore numbers formatted as text. If a cell contains an operational data entry typo like `"l00"` (using a lowercase L instead of the number 1) or trailing text padding like `"1450 "`, the mathematical functions will omit the cell completely without throwing an alert. 

This module outlines how to build a diagnostic pipeline to catch these silent errors.

## Auditing and Isolating Mixed Data Types
To pinpoint hidden formatting errors across a column before running calculations, deploy these diagnostic methods:

### 1. Programmatic Type Check (`TYPE`)
Run `=TYPE(cell)` in an adjacent row to evaluate the true under-the-hood data payload type:
* `1` = True Number
* `2` = Text String

  <img width="1100" height="806" alt="sheets_alignment_proof" src="https://github.com/user-attachments/assets/c1acb9d6-eed7-4e63-8abc-f3bca13bd9b3" />


  <img width="1919" height="798" alt="helper_column_validation" src="https://github.com/user-attachments/assets/e8f156b6-e9c5-48fb-86b3-36d5345e8867" />
### 2. Logical Assertions (`ISNUMBER` / `ISTEXT`)
Create a validation helper column running a conditional check to flag clear text entry anomalies:
```excel
=IF(ISNUMBER(H2), "Valid Data", "ERROR: Text Format Detected")
