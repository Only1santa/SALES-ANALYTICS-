# SALES-ANALYTICS-
Group 27 work on Sales analytics


Started by cleaning the file , removed duplicates on 2 rows , two products had similar id's so we made a unique id on one product 
calculated revenue , cost of goods and profit margin for efficieny in new columns
Merged hierachical region comprising of region , country, location

#ANALYSIS TASK
This repository documents  analytical workings for part B of sales analysis assignment built entirely in excel using helper columns , pivot tables and formulae driven calculations
Each task is shown in the sheet with methodology used so the working is transparent


We created an interactive dashboard on sales showing monthly revenue , sku revenue and profit by region and channel . 

Built an interactive scenario model to test the financial impact of three business levers — discount policy, cost inflation, and demand changes — against baseline performance, without altering raw sales data.
Approach
Created a dedicated Scenario_Model sheet, isolated from raw SalesData to preserve data integrity
Defined three named input cells (DiscountCap, CostInflation, QtyUplift) with data validation to enforce realistic bounds (0–25%, 0–15%, 0–20% respectively)
Used SUMPRODUCT array logic (in place of PivotTables, due to WPS limitations) to calculate Revenue and COGS dynamically across the full dataset
Applied MIN() logic to cap discounts at the scenario threshold while preserving actual values below the cap
Built a side-by-side Baseline vs. Scenario comparison table with absolute and percentage deltas, using conditional formatting to flag favorable/unfavorable shifts
Extended the model with a static sensitivity table (Conservative / Base Case / Optimistic) to show outcomes across three named futures simultaneously
