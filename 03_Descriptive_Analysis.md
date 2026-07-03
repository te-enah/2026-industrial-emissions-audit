# Module 3: Aggregations & Descriptive Analytics

Once the dataset is validated and free of formatting errors, we can proceed to descriptive analysis. This module focuses on aggregating the `TOTAL_RELEASES` by `CHEMICAL` type to identify emission trends.

## Summary Metrics
To provide high-level operational oversight, we implement pivot tables and aggregate functions:

### 1. Pivot Table Aggregation
By utilizing a Pivot Table, we can map `CHEMICAL` against the sum of `TOTAL_RELEASES` to normalize the data across all facilities.
* **Rows:** `CHEMICAL`
* **Values:** `SUM` of `TOTAL_RELEASES`
* **Sort Order:** Descending by value to highlight top-priority chemicals.

  <img width="1340" height="766" alt="pivot_table_aggregation" src="https://github.com/user-attachments/assets/9d18ec69-0d40-457e-b054-6609533dd39d" />


### 2. Descriptive Statistical Baseline
Beyond simple sums, we utilize the following functions to establish a baseline for 2026 performance:
* `=AVERAGE(H2:H101)` – Calculates the mean release volume per facility.
* `=MEDIAN(H2:H101)` – Identifies the central tendency, minimizing the impact of extreme outliers.
* `=MAX(H2:H101)` – Highlights the highest individual facility emission record.

![Descriptive Analytics Summary]<img width="920" height="717" alt="descriptive_analytics_summary" src="https://github.com/user-attachments/assets/9cc17ac4-7634-434c-babd-641c818046f7" />


## Strategic Insights
The resulting summary table provides immediate visibility into which chemical categories contribute most significantly to the total industrial footprint. This allows for data-driven prioritization of compliance resources.
