# Introduction
The dataset used in this project is based on police recorded crime data and outcomes in England and Wales. It provides detailed insights into the number of crimes recorded by police forces, the outcomes of these cases, and the specifics of offences involving knives, hate crimes, and transferred/cancelled records. The goal of this analysis is to extract relevant information from the data, focusing on crime trends, outcomes, and discrepancies across various regions and crime types.
# Problem Statement
The primary aim of this project is to analyze police-recorded crime data to identify trends, outcomes, and regional differences. Key areas of interest include the effectiveness of police outcomes, the patterns of knife-related crimes, and the reporting and resolution of hate crimes. The analysis seeks to understand how crime statistics vary over time and by region, as well as how police recording practices impact the data.
# Data sourcing
The data was sourced from the Home Office's open data tables for police-recorded crime and outcomes. The crime tables cover various crime types, outcomes, and regions within England and Wales. Specific tables include data on general crimes, knife-related offences, hate crimes, and transferred or cancelled records, all provided in a structured format (.ods) for ease of analysis.
- [location data](https://docs.google.com/spreadsheets/d/12_rGg2I15b8fcCuI3-sa6s_ZFo_GO6ODY4_CmGzXqms/edit?usp=classroom_web&authuser=0)
- [Crime data](https://docs.google.com/spreadsheets/d/10tMLxKFBo_yIbFgpzbFul6xO9JhHG8yth8ZM2RXc6Gc/edit?usp=classroom_web&authuser=0)
- [Data dictionary](https://drive.google.com/file/d/1UanB-0CzhQIlMBdpBprS7t8d0W_L2jHx/view?usp=classroom_web&authuser=0)
- 
# Data transformation and cleaning
The data underwent several cleaning and transformation steps to ensure it was ready for analysis:<br>

Missing Data Handling: Rows with incomplete data, particularly missing outcomes or crime types, were either filled using appropriate methods or removed.<BR>

Data Formatting: The data was structured into consistent financial years and quarters, ensuring time-based comparisons were valid.<BR>

Categorization: Crime data was categorized based on offence types, regions, and outcomes, using reference tables to map codes to descriptive labels.<BR>

Outliers and Anomalies: Any outliers, especially negative values due to crime cancellations, were flagged and accounted for in the analysis to avoid skewing results.<BR>

These steps were necessary to prepare the dataset for accurate analysis and reporting.<BR>

![image](https://github.com/user-attachments/assets/3c583e4c-5f4a-4a1a-9186-0874c6fa22a5)

# Data modeling
 Data is organized by financial year, with a breakdown of various crime categories. It includes multiple levels such as offence codes, offence groups, and police force areas to ensure comprehensive crime coverage.Dimensions with which to break down the analysis were identified. Hence, new tables for identified dimensions were created. These included:
Location Dimension
Date Dimension Table
Offence Dim Table
Additional features were created to give more robustness to the analysis.
The data model was designed using the Star Schema where the different dimensions were connected to the Crime Fact table in a one-to-many relationship<br>

![image](https://github.com/user-attachments/assets/ef18b447-4935-4038-8e35-649eeedb7f31)

# Dashboard
![image](https://github.com/user-attachments/assets/ed08d311-b60c-4491-8604-9135604b0739)

# Insight
Total Crime committed during the year from 2012 to 2022 amounts to 60 Million.<br>

The crime rate trend  was on a steady rate at about 4million from 2012 to 2016. From 2017, the rate of crime increased from 4million plus to 5 million.<br>

In 2020, there was a decrease in the rate of crime<br>

Highest rate of crime was in 2021.<br>

Record shows that the highest Offence committed according to offfence group was Theft Offence follow by Violence.<br>

Records shows that South East has the highest no of crime based on region.

# Recommendation
Police should focus more on reducing crime offences of Theft and Violence because that is the most committed offence over the years.




