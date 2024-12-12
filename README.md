# Project Overview 

This repository describes the  end-to-end portfolio of the Data Analytics Platform I designed for the City of Vancouver Health Agency.

# [Project: Descriptive Analysis]

Project Title: Data Analytic Platform (DAP) Design and Implementation for City of Vancouver Issued Operating Permits – Water Systems.

**About the Client: **The City of Vancouver, as part of its continuous effort to retain its place as one of the world’s most livable cities due to its quality of life and clean environment, intends to understand (gain insight) into the water quality city, especially regarding how mechanized systems are used for existing cooling towers, decorative water features, building water treatment systems and rainwater harvesting/non-potable water systems in order to effectively mitigate health risks by pathogens through its operating permits for water systems.

**Data Set Title:** Issued operating permits – Water Systems 
<br> **Source:** The City of Vancouver Open Data Portal (Issued operating permits – water systems, 2024) 
<br> **Applied filters:** Geo Local Area: Downtown and	Current system status: 
<br> **Active Record Count:** 434 
<br> **Last Processing Date:** November 19, 2024, 9:52 AM 
<br> **File Formats:** CSV and XLSX (Excel) 

<img width="468" alt="image" src="https://github.com/user-attachments/assets/0eeeb856-06d5-4793-b7d6-2f2c94c1a4fd" />

**Dataset:** The dataset includes transactional data from XYZ Retail over the past year, containing the following key features: 
<br>•	Operating Permit Number (ID): Unique identifier for each permit issued for each operator
<br>•	Address: Address where each mechanized system is situated
<br>•	Mechanized System Status: The status of each system if active or not
<br>•	Permit Renewal Date: When each operating permit is due for renewal
<br>•	Voluntary Participant: Indicator for each applicant if they willingly reported their system or not
<br>•	Marker Colour: Total price of the transaction 
<br>•	Turbidity: The nature of the mechanized system
<br>•	Legionella: A type of water infection

**Methodology:** 
1-	Data Collection and Preparation: 
    o	Load the dataset using Excel as the data analysis tool
    o	Perform data cleaning to address missing values, correct data types, and remove duplicates using AWS Glue DataBrew

2-	Descriptive Statistics: o	Calculate summary statistics for key variables, including: 	Total sales and average transaction value 	Number of transactions per month 	Distribution of purchases by product category 	Average quantity purchased per transaction 3-	Data Visualization: o	Create visual representations to illustrate findings: 	Time series graphs showing sales trends over the year. 	Bar charts displaying the most popular product categories. 	Pie charts representing the share of different payment methods. 	Heatmaps of sales by location and time of day. 4-	Customer Segmentation: o	Segment customers based on their purchasing behavior (e.g., high-frequency vs. low-frequency buyers). o	Analyze the purchasing patterns of different segments. 5-	Insights and Findings: o	Summarize the insights derived from the analysis, highlighting: 	Peak shopping periods (e.g., holidays, weekends) 	Trends in product category sales over time 	Preferences in payment methods across customer segments 6-	Recommendations: o	Provide actionable recommendations based on the findings to inform inventory management, targeted marketing campaigns, and promotional strategies. Tools and Technologies: •	Python (Pandas, Matplotlib, Seaborn) or Excel for data analysis •	Data visualization tools (Tableau or Power BI) for creating dashboards Deliverables: •	A detailed report summarizing the methods, findings, and recommendations. •	Visualizations and dashboards to present key insights clearly. •	A presentation for stakeholders to communicate important findings and suggestions for future action. This descriptive analysis project aims to provide a comprehensive understanding of customer purchase behaviors, enabling XYZ Retail to optimize its operations and enhance customer satisfaction.
