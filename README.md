# Project Overview 

This repository describes the  end-to-end portfolio of the Data Analytics Platform I designed for the City of Vancouver Health Agency.

# [Project: Descriptive Analysis]

Project Title: Data Analytic Platform (DAP) Design and Implementation for City of Vancouver Issued Operating Permits – Water Systems (Team Member 3 – Samuel Ayodeji Omotayo)

About the Client:
The City of Vancouver, as part of its continuous effort to retain its place as one of the world’s most livable cities due to its quality of life and clean environment, intends to understand (gain insight) into the water quality city, especially regarding how mechanized systems are used for existing cooling towers, decorative water features, building water treatment systems and rainwater harvesting/non-potable water systems in order to effectively mitigate health risks by pathogens through its operating permits for water systems.

Data Set Title: Issued operating permits – Water Systems
Source: City of Vancouver Open Data Portal (Issued operating permits – water systems, 2024)

Applied filters: 
•	Geo Local Area: Downtown
•	Current system status: Active

Record Count: 434
Last Processing Date: November 19, 2024, 9:52 AM
File Formats: .CSV and .XLSX (Excel)
Data Team: Development, Buildings, and Licensing - Building Policy 

Licence Coverage:
•	Section 1 [2]: The Information Provider grants you a worldwide, royalty-free, perpetual, non-exclusive licence to use the Information, including for commercial purposes, subject to the terms below (Open Data Licence, n.d.).
•	Section 2 [3]: You are free to - copy, modify, publish, translate, adapt, distribute or otherwise use the Information in any medium, mode or format for any lawful purpose (Open Data, n.d.).
The bar graph below visually shows the frequency of use (count) of the four mechanized systems - building water treatment systems, cooling towers, decorative water features, and rainwater harvesting/non-potable water/alternative water systems.
![image](https://github.com/user-attachments/assets/ec378dda-d763-423c-8d1f-5819ea3521e4)

**Methodology:**
1-	Data Collection and Preparation:
    o	Loaded the source dataset using Microsoft Excel as the data analysis tool.
    o	Performed data profiling and data cleaning to address missing values, correct data types, and remove duplicates using AWS Glue DataBrew

2-	Descriptive Statistics:
    - Business Question: What is the distribution of the four (4) mechanized system types used for water management in the Downtown City of Vancouver?
    Calculated summary statistics for key variables, including:
    - How do we calculate the use of each Mechanized System distribution: 
    -	Building Water = (# of Building Water systems / Total # of active mechanized systems) * 100
    -	Cooling Tower = (# of Cooling Tower systems / Total # of active mechanized systems) * 100
    -	Decorative Water = (# of Decorative Water systems / Total # of active mechanized systems) * 100
    -	Rainwater Harvesting = (# of building water systems / Total # of active mechanized systems) * 100
![image](https://github.com/user-attachments/assets/c8e495f0-ba1a-4f72-81eb-ea400ab60d01)

3-	Data Visualization:
o	Create visual representations to illustrate findings:
	Time series graphs showing sales trends over the year.
	Bar charts displaying the most popular product categories.
	Pie charts representing the share of different payment methods.
	Heatmaps of sales by location and time of day.
4-	Customer Segmentation:
o	Segment customers based on their purchasing behavior (e.g., high-frequency vs. low-frequency buyers).
o	Analyze the purchasing patterns of different segments.
5-	Insights and Findings:
o	Summarize the insights derived from the analysis, highlighting:
	Peak shopping periods (e.g., holidays, weekends)
	Trends in product category sales over time
	Preferences in payment methods across customer segments
6-	Recommendations:
o	Provide actionable recommendations based on the findings to inform inventory management, targeted marketing campaigns, and promotional strategies.
Tools and Technologies:
•	Python (Pandas, Matplotlib, Seaborn) or Excel for data analysis
•	Data visualization tools (Tableau or Power BI) for creating dashboards
Deliverables:
•	A detailed report summarizing the methods, findings, and recommendations.
•	Visualizations and dashboards to present key insights clearly.
•	A presentation for stakeholders to communicate important findings and suggestions for future action.
This descriptive analysis project aims to provide a comprehensive understanding of customer purchase behaviors, enabling XYZ Retail to optimize its operations and enhance customer satisfaction.
![image](https://github.com/user-attachments/assets/7858a6a8-1123-4572-a651-6c0fef8e6407)

