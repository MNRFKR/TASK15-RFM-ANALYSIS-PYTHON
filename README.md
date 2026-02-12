# TASK15-RFM-ANALYSIS-PYTHON
Step 1 – Data Import & Cleaning
We loaded the dataset (Train.csv) into pandas and removed rows with missing values in key demographic and categorical fields. This ensured a clean foundation for segmentation analysis.
Step 2 – Date Conversion (Skipped)
The dataset did not contain invoice dates, so the step of converting InvoiceDate to datetime was not applicable. We noted this clearly to avoid confusion.
Step 3 – RFM Feature Construction
Since transactional data was absent, we created proxy RFM features:
- Recency from Age
- Frequency from Family_Size
- Monetary from Spending_Score (already encoded numerically).
Step 4 – RFM Bucketing with Quantiles
We applied quantile‑based bucketing for Recency and Frequency, and discrete binning for Monetary. This produced R, F, M scores that were combined into an overall RFM_Score.
Step 5 – Segment Label Assignment
Based on RFM score ranges, customers were classified into segments: Champions, Loyal, Potential Loyalists, and At Risk. This added a clear behavioral grouping to the dataset.
Step 6 – Segment Visualization
We plotted a bar chart of segment counts, showing the distribution of customers across the four categories. This visualization highlighted which groups dominate the dataset.
Step 7 – Export to CSV
The enriched dataset, including RFM scores and segment labels, was exported as customer_segmentation.csv. This created a portable file for further analysis or reporting.
Step 8 – Business Actions per Segment
For each segment, three actionable strategies were defined. Champions were rewarded and upsold, Loyal customers nurtured, Potential Loyalists converted, and At Risk customers re‑engaged. This tied the technical segmentation back to business value
