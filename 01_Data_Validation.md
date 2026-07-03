# Module 1: Structural Setup & Alignment Validation

Before running any calculations, a spreadsheet must be formatted for maximum readability and checked for structural validity. This document outlines the foundational setup rules.

## Step-by-Step Layout Engineering
To build an optimal interface for analysis, apply these presentation steps:
* **Header Enforcement:** Highlight row 1 and execute `Ctrl + B` (Windows) / `Cmd + B` (Mac) to bold headers. Navigate to **View > Freeze > 1 row** to lock it in place during vertical scrolling.
* **Text Wrapping:** Select text columns like `FACILITY_NAME` and `CHEMICAL`, click the **Text Wrapping** tool on the toolbar, and choose **Wrap**.
* **Data Uniformity:** Highlight categorical identification data (e.g., `YEAR` or `UNIT_OF_MEASURE`) and change **Horizontal Align** to **Center**.
* **Auto-Fit Adjustments:** Click the select-all grid intersection (top-left block), hover between any two column letters until the double-headed arrow (`↔`) appears, and **double-click** to automatically snap every column width to its maximum text content size.

![My Google Sheets Layout Setup](sheets_layout_setup.png)<img width="906" height="914" alt="sheets_layout_setup" src="https://github.com/user-attachments/assets/25c654d0-ec8d-4566-97fa-b588546c8049" />


## Native Data Type Identification
Spreadsheets separate text data types from numeric data types. Without override configurations, look for these default alignment cues:
* **Left-Aligned Fields:** Read natively as **Text Strings** (Strings). Expected across `FACILITY_NAME`, `CITY`, `COUNTY`, `STATE`, `CHEMICAL`, and `UNIT_OF_MEASURE`.
* **Right-Aligned Fields:** Read natively as **Numeric Values** (Integers/Floats). Expected across `YEAR` and `TOTAL_RELEASES`.

![Data Alignment Cues Left vs Right](sheets_alignment_proof.png)<img width="1100" height="806" alt="sheets_alignment_proof" src="https://github.com/user-attachments/assets/d8229f3b-016d-4210-ba37-de616855d46e" />
