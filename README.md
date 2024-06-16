👋 Hi, I’m Loise

As a data analyst, my primary focus is on extracting insights from data to support informed decision-making. Here's a brief rundown of my toolkit and expertise:

- 💻**Languages**:Python & SQL
  
* Python:I leverage libraries like Pandas,NumPy,and Matplotlib to handle data manipulation,perform statistical analysis,and create informative visualizations.

* SQL:proficient in writing complex SQL queries to extract,filter,and aggregate data from relational databases, enabling me to uncover valuable insights and patterns.
- 🛠️**Tools**: Power BI,Python & Cognos
- 👷‍♀️**Workflow**:My workflow typically involves:
  
  - Data Collection:Gathering data from various sources, including databases, APIs, and flat files.
  
  - Data Cleaning:Preprocessing and cleaning data to ensure accuracy and consistency.
  
  - Analysis:Performing exploratory data analysis (EDA) to identify trends, outliers, and correlations.
  
  - Visualization:Creating informative charts,graphs,and dashboards to communicate insights effectively.
  
  - Interpretation:Deriving actionable insights and recommendations based on data analysis results.
  
  - Reporting:Presenting findings to stakeholders through reports, presentations, or interactive dashboards.
  
- 💞️ I’m looking to collaborate on teamwork and effective communication.I'm also open to feedback and continually strive to improve my analytical skills and deliver impactful insights.
- 📫 How to reach me via email at louisebaraza12@gmail.com.I'm excited to explore data-driven solutions together!

  ## 🚀 Current Focus
  - 🌱 I'm currently learning and exploring Tableau for data visualization and analysis.Excited to leverage its capabilities to enhance storytelling and create compelling visualizations.
 
   ## 👷‍♀️ Recent Projects
 
   ### [Data Collection Using APIs](https://github.com/lbaraza/Api)
  -  Collected job data from Jobs API
 
  -  Stored the collected data into an excel spreadsheet.
 
   ### [Web Scraping](https://github.com/lbaraza/Web-scrapping)
  - Extracted information from a given website
 
  - Wrote the scraped data into a csv file.
 
   ### [Data-wrangling](https://github.com/lbaraza/Data-wrangling)
 - Identified duplicated values in the dataset.

- Removed duplicated values from the dataset.

- Identified missing values in the dataset.

- Imputed the missing values in the dataset.

- Normalized data in the dataset.

 ### [Exploratory Data Analysis](https://github.com/lbaraza/Exploratory-Data-Analysis)
 - Identified the distribution of data in the dataset.

- Identified outliers in the dataset.

- Removed outliers from the dataset.

- Identified correlation between features in the dataset.

 ### [Data Visualization](https://github.com/lbaraza/Data-Visualization)
 - Visualized the distribution of data.

- Visualized the relationship between two features.

- Visualized composition of data.

- Visualized comparison of data.

 ### [Dataset Exploration](https://github.com/lbaraza/Survey-Dataset-Exploration)
- Loaded the dataset that will used thru the capstone project.

- Explored the dataset.

- Got familiar with the data types.

 ### [Building a Dashboard With IBM Cognos Analytics](https://github.com/lbaraza/Dashboards-on-Cognos)
  - Made a Dashboard of Current Technology Usage

  - Made a Dashboard of Future Technology Trend

  - Made a Dashboard of Demographcis

    ### [Building a Dashboard using SQL& Power BI](https://github.com/lbaraza/SQL-Power-BI)

# Toman Bike Share Analysis

## Project Overview

This project involves an analysis conducted for Toman Bike Share to determine if increasing prices next year is feasible.
As a data analyst,the focus was on examining current and historical data to provide insights for pricing decisions.

## Tools and Technologies

- **SQL**: Used for data extraction,transformation,and loading (ETL) processes.
- **Power BI**: Utilized for data visualization and dashboard creation to present findings.

## Objectives

1. Hourly revenue Analysis.
2. Profit and revenue trends.
3. Seasonal Revenue.  
4. Rider demographics.
5. Provide recommendations on raising prices next year.

## Key Findings
-  Conservative Increase: Considering the substantial increase last year,a more conservative increase might be prudent to avoid hitting a price ceiling where demand starts to drop.An increase in the range of 10-15% could test the market's response without risking a significant loss of customers.
-  Price Setting: If the price in 2022 was $4.99,a 10% increase would make the new price about $5.49, while a 15% increase would set the price at approximately $5.74.

## Data Sources
You can access the datasets through the following links:

-  https://github.com/lbaraza/SQL-Power-BI/blob/main/bike_share_yr_0.csv
-  https://github.com/lbaraza/SQL-Power-BI/blob/main/bike_share_yr_1.csv
-  https://github.com/lbaraza/SQL-Power-BI/blob/main/cost_table.csv

## Usage

1. **SQL Scripts**: Located in the `sql` directory, containing scripts used for data extraction and transformation.
2. **Power BI Dashboard**: Located in the `powerbi` directory, showcasing the interactive dashboard created for the analysis.

## Conclusion

The analysis provides a comprehensive overview of Toman Bike Share's current performance and 
supports informed decision-making regarding potential price adjustments.

## SQL Code


with cte as (
select * from bike_share_yr_0
union all
select * from bike_share_yr_1)


select
dteday,
season,
a.yr,
weekday,
hr,
rider_type,
riders,
price,
COGS,
riders*price as revenue,
riders*price -COGS as profit
from cte a
left join cost_table b
on a.yr =b.yr


    









<!---
lbaraza/lbaraza is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
