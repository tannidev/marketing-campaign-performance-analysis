# Marketing Campaign Performance Analysis

## Overview
This project analyzes digital marketing campaign data using Python to measure campaign effectiveness across key performance metrics such as click-through rate (CTR), cost per click (CPC), conversion rate, cost per acquisition (CPA), and return on investment (ROI).

The analysis compares campaign performance across different campaign IDs and age groups to identify which campaigns and customer segments perform better.

## Business Problem
Marketing teams need to understand whether their advertising spend is generating meaningful engagement, conversions, and profitability. Without proper analysis, budget may be allocated to campaigns that are inefficient or underperforming.

This project helps answer questions such as:
- Which campaign has the highest CTR?
- Which campaign has the best conversion performance?
- Which campaign has the lowest or highest acquisition cost?
- Which campaign delivers the strongest ROI?
- How do performance metrics vary across age groups?

## Dataset
- File used in analysis: `data.csv`
- Dataset source: [Add Kaggle dataset link here](PASTE_KAGGLE_LINK_HERE)
- Note: The raw dataset is not included in this repository.

## Tools and Technologies
- Python
- pandas
- numpy
- matplotlib
- seaborn
- Jupyter Notebook

## Project Workflow
The project was completed in the following steps:

1. Loaded the dataset
2. Inspected the dataset structure and missing values
3. Filled missing values in conversion-related columns
4. Calculated click-through rate (CTR)
5. Cleaned and standardized campaign IDs
6. Calculated cost per click (CPC)
7. Calculated conversion rate
8. Calculated cost per acquisition (CPA)
9. Estimated revenue using approved conversions
10. Calculated return on investment (ROI)
11. Compared performance across campaigns
12. Compared performance across age groups
13. Built summary tables and visualizations

## Data Cleaning
The notebook includes the following cleaning steps:
- Filled missing values in `total_conversion` with 0
- Filled missing values in `approved_conversion` with 0
- Converted `campaign_id` to numeric
- Dropped invalid `campaign_id` values after conversion
- Replaced infinite and missing values in `CPC` with 0
- Replaced infinite and missing values in `CPA` with 0
- Replaced infinite and missing values in `ROI` with 0

## Metrics Used

### Click-Through Rate (CTR)
CTR measures the percentage of impressions that resulted in clicks.

**Formula:**  
`CTR = clicks / impressions`

### Cost Per Click (CPC)
CPC measures the average amount spent per click.

**Formula:**  
`CPC = spent / clicks`

### Conversion Rate
Conversion rate measures the percentage of impressions that resulted in approved conversions.

**Formula:**  
`conversion_rate = approved_conversion / impressions`

### Cost Per Acquisition (CPA)
CPA measures the average cost to acquire one approved conversion.

**Formula:**  
`CPA = spent / approved_conversion`

### Return on Investment (ROI)
ROI estimates campaign profitability relative to ad spend.

**Formula used in this notebook:**  
`ROI = (revenue - spent) / spent`

Revenue in this project was estimated using:

`revenue = approved_conversion × 50`

This means ROI is based on an assumed revenue value of **$50 per approved conversion**.

## Analysis Performed

### Campaign-Level Analysis
The notebook calculates:
- Average CTR by campaign
- Average CPC by campaign
- Average conversion rate by campaign
- Average CPA by campaign
- Average ROI by campaign

### Age Group Analysis
The notebook calculates:
- CTR by age group
- Conversion rate by age group
- CPA by age group

### Summary Table
A summary table is created containing:
- CTR (%)
- Average CPC ($)
- Conversion Rate (%)
- CPA ($)

for each campaign.

## Key Results

### Campaign Performance
Based on the notebook results:

- **Highest CTR:** Campaign `916`
- **Highest Conversion Rate:** Campaign `936`
- **Lowest CPC:** Campaign `936`
- **Highest CPC:** Campaign `1178`
- **Lowest CPA:** Campaign `916`
- **Highest CPA:** Campaign `1178`
- **Highest ROI:** Campaign `916`
- **Lowest ROI:** Campaign `1178`

### Age Group Performance
Based on the notebook results:

- **Highest CTR:** Age group `45-49`
- **Highest Conversion Rate:** Age group `30-34`
- **Lowest CPA:** Age group `30-34`
- **Highest CPA:** Age group `40-44`

These results suggest that campaign effectiveness varies across both campaign strategy and target audience age group.

## Visualizations
The notebook includes the following charts:
- Bar chart of average CPA by campaign
- Bar chart of CTR by campaign
- Bar chart of CPA by age group
- Bar chart of conversion rate by age group
- Bar chart of ROI by campaign

## Business Value
This project demonstrates how marketing data can be used to support better advertising decisions by:
- Identifying stronger and weaker campaigns
- Comparing cost efficiency across campaigns
- Evaluating profitability using ROI
- Understanding audience performance by age group
- Supporting smarter marketing budget allocation

## Repository Contents
- `marketing_analysis.ipynb` — notebook containing data cleaning, metric calculation, analysis, summary tables, and visualizations
- `README.md` — project documentation

## How to Run
1. Open the notebook in Jupyter Notebook or JupyterLab
2. Install the required Python libraries
3. Place `data.csv` in the same folder as the notebook
4. Run the notebook cells step by step

## Future Improvements
- Add chart screenshots to the repository
- Improve handling of zero-click and zero-conversion cases
- Add more segmentation dimensions such as gender or interest categories
- Build an interactive dashboard version of the analysis

## Author
Tanni
