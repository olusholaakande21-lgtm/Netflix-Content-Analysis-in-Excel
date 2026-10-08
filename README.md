This project presents an end-to-end analysis of 8,807 Netflix titles using Microsoft Excel. The analysis explores Netflix's content catalog to identify patterns in content growth, content type, ratings, genres, and geographical distribution.

The project demonstrates a structured analytical workflow using Excel Power Query, Pivot Tables, Pivot Charts, Slicers, and an interactive dashboard to transform raw data into meaningful business insights.

The analysis is structured around five key business questions and concludes with actionable recommendations for content strategy and catalog diversification.

<img width="1317" height="583" alt="NETFLIX Dashboard" src="https://github.com/user-attachments/assets/33012d6b-8d3f-49d3-a322-22716f9a62d9" />


🎯 Business Questions

The analysis seeks to answer the following questions:
How has Netflix's content catalog grown over time?
Which genres or content categories dominate the catalog?
What is the distribution between Movies and TV Shows?
Which content rating is most prevalent?
Which countries contribute the most titles to the Netflix catalog?

📊 Dataset
Source: Public Netflix Titles Dataset — Kaggle
Records: 8,807 titles
Columns: 12
Granularity: One row per Netflix title
Key Fields

show_id · type · title · director · cast · country · date_added · release_year · rating · duration · listed_in · description

🛠️ Tools & Technologies
Purpose	Tool
Data Cleaning & Transformation	Excel Power Query
Data Analysis	Excel Pivot Tables
Data Visualization	Pivot Charts
Dashboard Interactivity	Excel Slicers
Reporting & Presentation	Excel Dashboard

🔎 Analytical Approach
The project follows a three-stage analytical framework:

1. Pre-Analysis
Before building the analysis, each business question was translated into an analytical plan covering:

Objective
Required data fields
Analytical approach
Expected business insight
Potential value to decision-making

2. In-Analysis

Pivot Tables and Pivot Charts were used to investigate each business question.

For every analysis, the results were evaluated to identify:
Key observations
Trends and patterns
Significant differences
Potential business implications

3. Post-Analysis

The findings were further evaluated through the interactive dashboard using slicers for:

Content Type
Rating
Year Added

This stage focused on validating the findings across different segments and converting observations into actionable insights and recommendations.

🧹 Data Cleaning & Preparation

The raw dataset contained missing values across several fields:

Column	Missing Values
Director	2,634
Country	831
Cast	825
Date Added	10
Rating	4
Duration	3
Power Query Transformation Steps

The following data preparation steps were performed:

Replaced missing values with "Unknown" instead of removing records
Preserved all 8,807 titles for analysis
Converted date_added into a proper date format
Created year_added and month_added fields for time-based analysis
Loaded the cleaned dataset into a structured netflix_titles table
Preserved the original dataset separately on the Raw Data sheet
Checked show_id for duplicate records; no duplicates were identified

📈 Key Findings
Analysis Area	Key Finding
Content Growth	2019 recorded the highest number of titles added, with 2,016 titles — 1,424 Movies and 592 TV Shows.
Catalog Concentration	Titles added between 2017 and 2020 account for approximately 76% of the catalog in the dataset.
Content Type	6,131 Movies (69.6%) compared with 2,676 TV Shows (30.4%).
Content Rating	TV-MA was the most common rating, with 3,207 titles (36.4%), followed by TV-14 with 2,160 titles (24.5%).
Country	The United States contributed the most titles at 2,818, followed by India (972) and the United Kingdom (419).
Top Categories	Dramas, International Movies, Documentaries, and Stand-Up Comedy were among the leading content labels.

💡 Business Insights
1. Netflix's catalog expansion was concentrated in recent years

The strongest period of catalog growth occurred between 2017 and 2020, with 2019 representing the peak year.
This suggests a period of aggressive content acquisition and expansion within the dataset.

2. Movies dominate the catalog

Movies represent approximately 70% of the titles, significantly exceeding TV Shows.
This indicates that the Netflix catalog in this dataset is heavily weighted toward movie content.

3. Mature-audience content represents a significant share

TV-MA is the largest rating category, accounting for approximately 36% of all titles.
This suggests a strong presence of content targeted toward mature audiences.

4. The catalog is geographically concentrated

The United States contributes the largest number of titles, with India representing the second-largest contributor.
This highlights the importance of both established and emerging regional content markets.

🎯 Recommendations

Based on the analysis, the following recommendations can be considered:

Maintain strong movie investments while continuing to monitor the changing balance between Movies and TV Shows.
Expand TV Show offerings in high-performing categories to improve catalog balance.
Increase genre and audience diversity, particularly family-friendly and children's programming.
Strengthen regional content production beyond the United States and India to improve geographical diversity.
Use audience engagement data alongside catalog data in future analysis to determine whether the largest content categories also generate the strongest viewer demand.

⚠️ Analysis Limitations

Several limitations should be considered when interpreting the findings:

The dataset measures titles rather than viewing activity, so it describes Netflix's catalog rather than audience behavior.
date_added represents when a title was added to Netflix, not when the title was originally released.
The dataset appears to end partway through 2021; therefore, the apparent decline in 2021 should not necessarily be interpreted as a genuine reduction in content additions.
listed_in and country contain multiple values within individual cells. Consequently, some Pivot Table results may underrepresent individual genres or countries.
Splitting multi-value fields into separate records would provide more granular analysis. For example, counting each country individually increases the United States total to approximately 3,690 titles.
Missing or "Unknown" values, particularly for director and country, limit the reliability of some categorical comparisons.

📌 Skills Demonstrated

This project demonstrates practical experience in:

Excel Data Analysis
Power Query
Data Cleaning
Data Transformation
Pivot Tables
Pivot Charts
Dashboard Development
Data Visualization
Exploratory Data Analysis
Business Question Formulation
Insight Generation
Analytical Storytelling
Business Recommendations
