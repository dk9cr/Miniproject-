# AI Driven Data Analytics: Y Combinator Startup Growth Dashboard

## 📌 Project Overview
This project analyzes the explosive growth of Artificial Intelligence startups using historical funding data from the Y Combinator startup directory. The objective of this mini-project was to extract a raw, unstructured web-scraped dataset, perform rigorous data pre-processing, and build an interactive business intelligence dashboard to visualize global AI investment trends.

## 🛠️ Tech Stack
* **Data Pre-Processing & Cleaning:** Microsoft Excel
* **Data Visualization & Modeling:** Microsoft Power BI

## 🧹 Phase 1: Data Pre-Processing (Excel)
**Raw Dataset:** 4,932 records | 16 features
**Cleaned Dataset:** 581 records | 10 features

The raw CSV file contained unstructured metadata and startups across all global industries. The following ETL (Extract, Transform, Load) steps were executed to prepare the data for modeling:
1. **Dimensionality Reduction:** Removed 6 non-essential web-scraping features (e.g., `slug`, `smallLogoUrl`, `longDescription`) to create a focused 10-feature business matrix.
2. **Precision Domain Filtering:** Applied strict conditional text filtering to the `tags` column, isolating exact matches for "Artificial Intelligence" to eliminate false positives and extract the 581 highly relevant AI startups.
3. **Data Imputation:** Handled missing/null values in the `teamSize` column by programmatically converting blanks to `0` to ensure mathematical accuracy in future aggregations.
4. **Data Integrity:** Executed deduplication protocols across all columns to guarantee each startup was represented by a single, unique row.
5. **Format Standardization:** Converted the finalized dataset from CSV to a structured `.xlsx` format for seamless Power BI integration.

## 📊 Phase 2: Data Visualization (Power BI)
Built a dynamic, interactive dashboard to allow stakeholders to explore the AI startup landscape. 

**Key Dashboard Features:**
* **KPI Card:** Displays the total count of verified AI startups funded.
* **Line Chart (Growth Timeline):** Visualizes the historical explosion of AI startup funding across Y Combinator batches/years.
* **Bar Chart (Geo-Location):** Ranks the top global tech hubs producing AI startups (e.g., San Francisco, New York).
* **Interactive Slicer (Industry Filter):** A responsive dropdown menu allowing users to filter the entire dashboard by specific sectors (e.g., Healthcare, Fintech, B2B SaaS).

## 📁 Repository Contents
* `ycombinator_companies.csv`: The original, raw dataset.
* `Cleaned_AI_Startups.xlsx`: The fully processed and cleaned dataset.
* `MiniProject_PowerBi.pbix`: The interactive Power BI dashboard file.
* `Dashboard_Overview.pdf`: Static export of the primary dashboard view.
* `Dashboard_Filtered_Healthcare.pdf`: Static export proving slicer interactivity.

## 🚀 How to Use
To interact with the dashboard, download the `.pbix` file and open it using Power BI Desktop. You can use the Industry Slicer in the top corner to dynamically filter the visual reports.
