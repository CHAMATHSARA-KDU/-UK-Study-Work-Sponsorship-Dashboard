# -UK-Study-Work-Sponsorship-Dashboard
This project explores UK migration sponsorship trends for study and work visas, using real-world datasets from the Australian Government’s open data platform

It analyzes how sponsorship applications have evolved over time, across nationalities, regions, and industries — providing insights into how migration patterns reflect education, employment, and policy dynamics.

Built using Microsoft SQL Server and Power BI, this dashboard demonstrates advanced data modeling, cleaning, and visualization techniques through SQL queries and DAX expressions.

🧠 Objectives

Analyze UK study and work sponsorship application trends (2010–2023).

Identify top nationalities, regions, and industries driving sponsorships.

Compare year-over-year and quarter-based growth rates.

Visualize repeat and extension sponsorship patterns.

Demonstrate integration between SQL Server and Power BI for data analytics.

🧩 Methodology
1. Data Import

Downloaded datasets from data.gov.au
:

CAS_D01, CAS_D02 → Study Sponsorship

CoS_D01, CoS_D02 → Work Sponsorship

Imported datasets into SQL Server using “Import Flat File” wizard.

2. Data Cleaning

Removed commas and converted fields (e.g., Applications) into numeric types using T-SQL.

Replaced nulls with “Not Applicable”.

3. Merging Datasets

Combined study and work files into merge_study and merge_work tables using T-SQL UNION operations.

4. Power BI Integration

Connected to SQL Server and imported merged datasets.

Performed transformations and created relationships using Power Query.

Built DAX measures for:

Total and Year-over-Year applications

Repeat sponsorships

Extension rates

Regional and institutional aggregations

📈 Dashboard Visuals
Visualization	Description
Total Study & Work Applications by Year	Area chart showing long-term application trends.
Year-over-Year Growth by Quarter	Line chart comparing quarterly growth rates.
Top 10 Nationalities by Visa Type	Tornado chart comparing study vs work applications.
Repeat Sponsorship Applications by Region	Map visualizing recurring visa demand geographically.
Extension Rate of Applications	Decomposition tree breaking down extension behavior.
Applications by Institution & Industry	Waterfall chart illustrating sector-level contributions.
Card & Slicer Elements	Dynamic filters for year, region, and nationality.
🧮 Key Insights

Study sponsorships show strong seasonal patterns linked to academic calendars.

Work sponsorships are more consistent but vary with policy and economic shifts.

India leads in work sponsorships, while China dominates study sponsorships.

Asia and Europe have the highest repeat sponsorship rates.

Work visa holders have higher extension rates (0.30) than study visa holders (0.18).

🛠️ Tools & Technologies

SQL Server – Database creation, cleaning, and merging datasets

Power BI – Data modeling, DAX calculations, and dashboard visualization

T-SQL – Data transformation and query scripting

DAX (Data Analysis Expressions) – Custom measures and calculated tables
