# Module 4: Advanced Lookups using XLOOKUP

Finding isolated data benchmarks is useful, but mapping them back to contextual row details provides actionable operational insights. This module replaces legacy lookup methods with the modern, resilient `XLOOKUP` function.

## Extremum Target Queries
To extract the boundaries of our data scope:
* **Maximum Release Target:** `=MAX(H2:H101)`
* **Minimum Release Target:** `=MIN(H2:H101)`

  <img width="934" height="730" alt="extreme_target_queries" src="https://github.com/user-attachments/assets/41f958bf-bd81-4ab3-bd2a-1a31696daa75" />

  <img width="926" height="738" alt="data_fetching_xlookup" src="https://github.com/user-attachments/assets/79e97c9c-a1e5-4ca4-ad8f-64969de34796" />

## Contextual Data Fetching
Instead of relying on rigid, sorted-dependent functions (like `VLOOKUP`), `XLOOKUP` allows us to pull metadata associated with our extremum targets effortlessly.

### Extracting Facility Identity
Assuming the maximum release metric (4200) was found and sits in cell `B88`:
```excel
=XLOOKUP(MAX(H2:H101), H2:H101, B2:B101)

