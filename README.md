# Combined Google and Facebook Ads Analysis: Merging Data and Aggregating Metrics

This project aims to merge data from Google and Facebook ad campaigns using CTE (Common Table Expressions) and perform aggregation to analyze campaign performance. The following steps detail the process:

## Steps Undertaken

### Step 1: SQL Query with CTE to Merge Data
A SQL query was written using CTE to combine data from the given tables and retrieve the following:
- **ad_date**: The date the ads were displayed on Google and Facebook.
- **media_source**: The source of the click (Google Ads / Facebook Ads). This column was created manually.
- **spend, impressions, reach, clicks, leads, value**: Campaign and ad set metrics for each day.

### Step 2: Aggregate Data Using CTE
Using the merged data from the CTE, an aggregated dataset was created with the following columns:
- **ad_date**: The date the ad was displayed.
- **media_source**: The source of the click.
- Aggregated values by date and media source for the following metrics:
  - **Total Spend**
  - **Number of Impressions**
  - **Number of Clicks**
  - **Total Conversion Value**

The table was grouped by `ad_date` and `media_source`.

## Final Product
The resulting analysis provides a comprehensive view of ad performance across Google and Facebook. By merging and aggregating key metrics, this project enables detailed evaluation of cross-platform ad effectiveness, helping to identify the most cost-efficient and high-performing sources.
