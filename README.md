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

The DAP architecture<br>
<img width="546" alt="image" src="https://github.com/user-attachments/assets/e03a5606-6f3f-4031-be5d-0f63ca888dea" />


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

<br>1.	Data Collection, Ingestion and Preparation: 
    <br>-	Load the dataset using Excel as the data analysis tool
    <br>-	Perform data cleaning to address missing values, correct data types, and remove duplicates using AWS Glue DataBrew

This includes understanding the following using AWS: 
    <br>•	Data structure: The number of columns, column names, column order and data type 
    <br>•	Content: The value distribution for the column, minimum, maximum, mean, average and others.
<img width="766" alt="image" src="https://github.com/user-attachments/assets/d1a9ba1b-afc8-4e62-8e75-f1bc1ab0e8d0" />


2.	Descriptive Statistics: 
<br> Business Question: What is the distribution of the four (4) mechanized system types used for water management in the Downtown City of Vancouver?
<br>How do we calculate the use of each Mechanized System distribution:
<br>•	Building Water = (# of Building Water systems / Total # of active mechanized systems) * 100
<br>•	Cooling Tower = (# of Cooling Tower systems / Total # of active mechanized systems) * 100
<br>•	Decorative Water = (# of Decorative Water systems / Total # of active mechanized systems) * 100
<br>•	Rainwater Harvesting = (# of building water systems / Total # of active mechanized systems) * 100

3. Design ETL Pipeline:
Started by creating the pipeline design using the following functions: 
<br>•	Extracting the data source from the S3 bucket through the Amazon S3 
<br>•	Dropped unwanted columns using the ‘Change Schema’ function 
<br>•	Counted the number of rows in the dataset using ‘Aggregate’ as a summarization function 
<br>•	Merged datasets using the ‘Join’ function •	‘Dynamic transformation’ to calculate the distribution ratio.
<img width="818" alt="image" src="https://github.com/user-attachments/assets/6625dba1-8ccc-4190-8d1b-2250a3eb26ec" />

**4. Highlights and Findings:**
![image](https://github.com/user-attachments/assets/bb1e3a2f-9876-461a-91f9-055be537998a)

<img width="634" alt="image" src="https://github.com/user-attachments/assets/a894ca83-f0ff-4496-beea-1fcebce81229" />

<br> 1. The cooling system is the dominant technology used for water system management in Downtown, representing 57% (276) of the total systems.
<br> 2.	The Decorative water feature is the second most used system, accounting for 19% of the total count.
<br> 3.	Rainwater harvesting has the lowest frequency. This suggests limited adoption.

**5. Recommendation:**
The City of Vancouver should do the following:
<br> **1. Focus on the Cooling Tower:** Being the most used system in the city (57%), the Agency should establish enhanced maintenance and monitoring protocols and inspection standards to avoid the risk of Legionella outbreaks.
<br> **2. Strengthen Monitoring for Decorative Water Features and Built Water Treatment Systems:** The city should drive awareness to ensure owners adhere to maintenance policies, as both systems represent 41% of the total type. 
<br> **3. Support Adoption of Rainwater Harvesting Systems:** The Agency should provide incentives or subsidies for installation and also run an awareness campaign on the environmental and economic benefits of harvesting rainwater
<br> **4. Allocate Resources Proportionally:** The Agency should provision its resources based on the respective proportion of the systems. 

**6. Tools and Technologies:**
<br> 1.	AWS Simple Storage Service (S3): Used to store the ingested data.
<br> 2.	AWS Data Brew: Helps in profiling (understanding) and transforming (cleaning) data for high quality and summarization. 
<b3> 3. AWS Data Glue: This AWS is used to Extract, Transform and Load (ETL) the dataset. This service helps to analyze the dataset to achieve the desired insight.
<br> 4.	Draw.io: This is used for the technical drawing that provides a graphical view of how the different systems and components interact.


# [Project 2: Explorative Analysis]

Project Description: Exploratory Data Analysis (EDA) on Fairview and Westend cities of Vancouver

Project Title: City of Vancouver Health Agency Water Management System Analysis: An Exploratory Data Analysis 

Objective: To compare the mechanized system distribution in two (2) locations in Vancouver (Fairview and West End) to examine whether any form of correlation, trends or pattern exists between them. 

Data Set Title: Issued operating permits – Water Systems 

Source: City of Vancouver Open Data Portal (Issued operating permits – water systems, 2024) 
<br> Geo Local Area: West End, Fairview 
<br> Current system status: Active 
<br> Record Count: 189 
<br> Last Processing Date: November 19, 2024, 9:52 AM 
<br> File Formats: .XLSX (Excel) 
<br> Data Team: Development, Buildings, and Licensing - Building Policy

Data Set: Fairview and Westend have the same similar data structure as indicated below:
<br>•	Operating Permit Number (ID): Unique identifier for each permit issued for each operator
<br>•	Address: Address where each mechanized system is situated
<br>•	Mechanized System Status: The status of each system if active or not
<br>•	Permit Renewal Date: When each operating permit is due for renewal
<br>•	Voluntary Participant: Indicator for each applicant if they willingly reported their system or not
<br>•	Marker Colour: Total price of the transaction 
<br>•	Turbidity: The nature of the mechanized system
<br>•	Legionella: A type of water infection

DAP System Architecture<br>
<img width="488" alt="image" src="https://github.com/user-attachments/assets/c64e6633-7d5d-447c-93f4-78dd255485d1" />

**Methodology:** 

<br>1.	Data Collection, Ingestion and Preparation: 
    <br>-	Load the dataset using Excel as the data analysis tool
    <br>-	Perform data cleaning to address missing values, correct data types, and remove duplicates using AWS Glue DataBrew

This includes understanding the following using AWS: 
    <br>•	Data structure: The number of columns, column names, column order and data type 
    <br>•	Content: The value distribution for the column, minimum, maximum, mean, average and others.
<img width="790" alt="image" src="https://github.com/user-attachments/assets/57106cfb-0922-40d9-918a-153063c0e19f" />

**2.	Explorative Statistics: **
<br> Business Question: What are the common trends, similarities or differences in the distribution of the four (4) mechanized system types used for water management in Fairview and Westfield locations at the City of Vancouver?
Step 1: Calculate the use of each Mechanized System distribution for each location:
<br>How do we calculate the use of each Mechanized System distribution:
<br>•	Building Water = (# of Building Water systems / Total # of active mechanized systems) * 100
<br>•	Cooling Tower = (# of Cooling Tower systems / Total # of active mechanized systems) * 100
<br>•	Decorative Water = (# of Decorative Water systems / Total # of active mechanized systems) * 100
<br>•	Rainwater Harvesting = (# of building water systems / Total # of active mechanized systems) * 100
Step 2: Compare and contrast the result of the outcome in step 1 above.

**3. Design ETL Pipeline:**
<br>•	Extracting the data source from the S3 bucket through the Amazon S3
<br>•	Dropped unwanted columns using the ‘Change Schema’ function
<br>•	Counted the number of rows in the dataset using ‘Aggregate’ as a summarization function
<br>•	Merged datasets using the ‘Join’ function
<br>•	‘Dynamic transformation’ to calculate the distribution ratio
<img width="897" alt="image" src="https://github.com/user-attachments/assets/3a6cfe65-07f8-47ea-918a-b70c215b5deb" />

**4. Highlights and Findings:**
<img width="634" alt="image" src="https://github.com/user-attachments/assets/a894ca83-f0ff-4496-beea-1fcebce81229" />

<br>**Insight/Deduction 1:** Mechanical System usage in Fairview and Westend 
<br>1.	Rainwater Harvesting/Alternative Water System: 
<br>        -	A common trend in both locations is that the Rainwater Harvesting/Alternative Water system is the least of all mechanized systems used with 2 in Fairview and 1 in Westend. 
<br>        -	This mechanized system represents the smallest portion of the overall system count with 2.04% in Fairview and 1.10% in Westend. 
<br>2.	Building Water Treatment System: 
<br>        -	Prominently used in both locations and ranked the second most used. 
<br>        -	Data indicates it is among the two most used systems in Westend. c.	A count of 36 (39.56%) in Westend compared to 28 (28.57%) in Fairview. 
<br>3.	Cooling Tower: 
<br>-	The Cooling Tower system appears to be the most used and dominant water system management technology in both locations. 
<br>-	Dominant in Fairview – 50 counts (51.02%) and equally significant in Westend but with 36 counts (39.6%). 
<br>4.	Decorative Water Feature: The trend indicates equal usage, with 18 counts in Fairview and Westend, which represent 19.78% and 18.37% respectively. 

<br>**Deduction 2:** Total Usage in both Locations 
<br>1.	Fairview has more mechanized systems compared to Westend - 98 vs 91 counts 
<br>2.	Despite the fewer counts in Westend, the Building Water Treatment System and Decorative Water Feature are higher in Westend compared to Fairview

**5. Recommendation:**
The City of Vancouver should do the following:
<br> 1. Focus on the Cooling Tower: Being the most used system in the city (57%), the Agency should establish enhanced maintenance and monitoring protocols and inspection standards to avoid the risk of Legionella outbreaks.
<br> 2. Strengthen Monitoring for Decorative Water Features and Built Water Treatment Systems: The city should drive awareness to ensure owners adhere to maintenance policies, as both systems represent 41% of the total type. 
<br> 3. Support Adoption of Rainwater Harvesting Systems: The Agency should provide incentives or subsidies for installation and also run an awareness campaign on the environmental and economic benefits of harvesting rainwater
<br> 4. Allocate Resources Proportionally: The Agency should provision its resources based on the respective proportion of the systems. 

6. Tools and Technologies:
<br> 1.	AWS Simple Storage Service (S3): Used to store the ingested data.
<br> 2.	AWS Data Brew: Helps in profiling (understanding) and transforming (cleaning) data for high quality and summarization. 
<b3> 3. AWS Data Glue: This AWS is used to Extract, Transform and Load (ETL) the dataset. This service helps to analyze the dataset to achieve the desired insight.
<br> 4.	Draw.io: This is used for the technical drawing that provides a graphical view of how the different systems and components interact.




