Global Literacy & Education Progress Dashboard | 1980-2024

## Project Objective
To analyze global literacy trends 1980-2024 to identify regional disparities, track SDG 4 progress, and provide data-driven recommendations for education stakeholders.

## Dataset Description
Source: World Bank WDI. 2 tables - WDICountry (Region, Income Group) and WDICSV (11,204 rows after cleaning). Period 1980-2024, 6 World Bank regions, 4 indicators: Adult Literacy, Youth Literacy, Completion Rate, Enrollment Rate.
KPIs: Avg Literacy 76%, Completion 63.95%, Enrollment 86.27%.

## Data Cleaning Process
- Removed 4,217 nulls in Literacy Rate column (27% missing 1980-1995)
- Removed 124 duplicates on Country Code + Year + Indicator
- Fixed inconsistencies: Sub Saharan Africa → Sub-Saharan Africa, Indicator truncation
- Standardized formats: Year changed from Σ Sum to Don't Summarize (Text), Literacy Rate to Percentage 2 decimals, Trimmed spaces
- Created DAX Measures: Avg Literacy, Avg Youth Literacy, Literacy Gap, Year Group
- Documented in Power Query Applied Steps

## Analysis Methodology
Tools: Power BI, DAX, Power Query
- Time Series: Line chart Year vs Avg Literacy by Region (2000-2024) to show MDG impact
- Comparative: Bar charts for 6 regions ranking
- Geospatial: Bubble map for literacy by country
- Gap Analysis: Enrollment 86% vs Completion 63% vs Literacy 76%
- Filters: Summary visuals = 2023, Trend visual = 2000-2024 to avoid sparse data zigzag

## Key Findings
- Literacy increased 22.4% from ~58% (1980) to 76% (2024)
- Youth literacy 10% higher than adult literacy
- 40% gap: Europe & Central Asia 92.1% vs Sub-Saharan Africa 52.4%
- Completion is bottleneck: 86% enroll but only 63.95% complete

## Insights & Recommendations
- Target Sub-Saharan Africa & South Asia for funding
- Fix completion crisis with feeding programs
- Focus on quality not just access, close gender gap

## Dashboard Overview
- 3 KPI cards, Regional Bar, World Map Bubble, Trend Line, Completion Bar
- Colors: Page #F1F5F9, Visuals #FFFFFF + shadow, Blue #3B82F6, Coral #FB7185

## Repository Structure
- /power-bi/ - .pbix file
- /dashboard/screenshots/ - dashboard screenshot
- /data/ - Dataset info (full file on Drive due to size)
- /docs/ - Final Report PDF

## Links
- Power BI File: in /power-bi folder
- Dashboard Screenshots: in /dashboard/screenshots
- Final Report: in /docs

## Author
Bukola - AnalystLab Africa Internship
# AnalystLabAfrica
