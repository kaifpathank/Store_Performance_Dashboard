# Store Performance Executive Suite Dashboard

> **Project type:** Data Analytics Portfolio Project  
> **Status:** Learning project — validate units, formulas, and source data before treating results as a business report.

## Project Overview
This project explores store-level performance using a dataset containing 898 store records. The analysis focuses on sales, customer traffic, available items, and store area. The dashboard is intended to help a reader compare store performance and identify records for further investigation.

## Business Questions
- What are the total and average store sales in the dataset?
- Which stores have the highest and lowest recorded sales?
- How does daily customer count vary across stores?
- How can sales, customer traffic, available items, and store area be compared?
- Which stores should be investigated further based on clearly stated thresholds?

## Dataset
The working sheet contains these fields:
- `Store ID`
- `Store_Area`
- `Items_Available`
- `Daily_Customer_Count`
- `Store_Sales`

**Dataset size:** 898 store records (verify against the source file before publishing).  
**Source:** Add the original dataset URL/name here. Do not claim a source you cannot verify.  
**Important:** The dataset fields do not, by themselves, establish currency or area units. Keep labels neutral unless the source documentation confirms them.

## Tools
- Google Sheets / Excel for data inspection and summary checks
- Gemini AI as an assistant for exploration and dashboard support (AI-generated output must be verified)
- Dashboard canvas used to present KPIs, comparisons, and a selected-store detail view

> Only list tools you personally used. If you recreate the dashboard in Power BI, add Power BI here and include the `.pbix` file if you can share it.

## Key Results (from the current working analysis)
- **Total recorded Store_Sales:** 53,298,770
- **Average Store_Sales:** approximately 59,352.75
- **Minimum Store_Sales:** 14,920
- **Maximum Store_Sales:** 116,320
- **Total Daily_Customer_Count across records:** 706,070
- **Average Daily_Customer_Count:** approximately 786.27
- **Average Items_Available:** approximately 1,781.94
- **Average Store_Area:** approximately 1,485.33
- **Highest-sales record identified:** Store ID 610, with recorded sales of 116,320

These values are preliminary and should be independently recalculated from the source file before publication. Do not add a currency symbol unless the source confirms the currency.

## Insights and Interpretation
1. **Store #610 is the highest-sales record in the current analysis.** Its recorded sales are 116,320. This identifies a record worth studying, but it does not explain why sales are high.
2. **Average recorded sales are about 59,352.75 per store.** This is a baseline for comparison, not a target or proof of good/bad performance.
3. **Average daily customer count is about 786.27 across the store records.** Store-level differences should be explored before drawing conclusions.
4. **Sales and customer traffic should be compared visually and statistically.** A scatter plot can reveal patterns, but correlation should be calculated and reported before claiming a strong relationship.
5. **Threshold flags are exploratory.** If the dashboard flags sales below 40,000 or above 75,000, document that these are analyst-selected thresholds—not externally validated definitions of poor or excellent performance.

## Metric and Data-Quality Notes
- `Store_Sales` has no confirmed currency in the field name. Use **Recorded Sales** or **Store_Sales** until the source defines its unit.
- `Store_Area` has no confirmed area unit. Do not label it square feet without source confirmation.
- A ratio of recorded sales to daily customer count is only a rough proxy if the periods and definitions are not aligned. Do not call it “average basket size” without transaction-level evidence.
- Verify the store ID uniqueness, missing values, duplicates, data types, and any outliers.
- Verify the row count and all summary values directly from the original CSV.
- Document that Gemini was used for assistance if you used it, and manually verify the results.

## Screenshots to Add
Create a folder named `images` in the repository and save the screenshots below. Use these exact relative paths in this README.

### 1. Full Dashboard
**File:** `images/store-comparison.png`  
**Place here:** Immediately below this heading.  
**Capture:** Full dashboard showing the title, KPI cards, main chart, and selected-store panel. Zoom the browser so the important text is readable. Hide unrelated browser tabs or personal information.

![Store Performance Dashboard](./Screenshot%202026-10-23%20003142.png)

### 2. KPI Cards
**File:** `images/dashboard-kpis.png`  
**Place here:** Below this heading.  
**Capture:** Crop showing the KPI cards clearly. Ensure unit labels are correct or neutral.

![Dashboard KPI cards](Screenshot 2026-10-23%010535.png)

### 3. Main Chart / Store Comparison
**File:** `images/store-comparison.png`  
**Place here:** Below this heading.  
**Capture:** The traffic-versus-sales chart or Top/Bottom 10 view. If showing correlation, include the actual calculated coefficient only if you have verified it.

![Store comparison](images/store-comparison.png)

### 4. Selected Store Detail
**File:** `images/store-610-detail.png`  
**Place here:** Below this heading.  
**Capture:** Store #610 details. Avoid showing unsupported currency or area units.

![Selected store detail](images/store-610-detail.png)

## Repository Structure
```text
store-performance-dashboard/
├── README.md
├── data/
│   └── Stores.csv                 # Include only if redistribution is permitted
├── images/
│   ├── dashboard-overview.png
│   ├── dashboard-kpis.png
│   ├── store-comparison.png
│   └── store-610-detail.png
└── report/
    └── Store_Performance_Project_Report.pdf
```

## How to Reproduce
1. Download the dataset from its verified original source.
2. Inspect column names, data types, missing values, duplicates, and store ID uniqueness.
3. Recalculate totals, averages, minimums, and maximums.
4. Build the charts and dashboard from the checked data.
5. Compare dashboard values against the calculations.
6. Add screenshots and the final report to the repository.

## Limitations
- The source and units must be documented before publishing.
- Summary statistics alone do not establish causes for high or low sales.
- Sales/customer ratios are not transaction-level average order values.
- The dashboard's thresholds are exploratory and should not be presented as company policy.
- AI-assisted results require independent verification.

## Author
**Kaif Khan**  
Aspiring Data Analyst | Excel / Google Sheets | SQL | Power BI | Python

Update this section to match the tools you have actually used and can explain confidently.
