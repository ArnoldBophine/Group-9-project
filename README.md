# Global Public Health Intelligence Dashboard

## Group Members
Susan Otieno - 670501

Lavender Achieng' - 671809

Movine ouma rading - 670351

Arnold Bophine - 668821

Angela Mwanzia - 663887

Reana Auma - 669255


## Dataset Source

Source: Global Health Statistics Dataset

Platform: Kaggle

Dataset URL:
https://www.kaggle.com/datasets/malaiarasugraj/global-health-statistics?resource=download
<img width="1600" height="892" alt="image" src="https://github.com/user-attachments/assets/7448b89c-4a4f-402b-b743-6474e56ac34a" />

## Dataset Description

The Global Health Statistics dataset contains health-related information collected from different countries between 2000 and 2024. It includes data on disease prevalence, incidence, mortality rates, recovery rates, healthcare access, treatment costs, population affected, demographic information, and socioeconomic indicators.

The dataset provides valuable insights into global health trends and helps identify patterns that can support better healthcare planning and decision-making.

## Business Problem
Public health organizations collect large amounts of health data every year, but turning this data into meaningful insights can be challenging without the right analytical tools. Decision-makers need a reliable way to identify disease trends, compare healthcare performance across countries, monitor mortality and recovery rates, and understand where healthcare resources are needed most.

For this project, our group developed a Global Public Health Intelligence Dashboard using Microsoft Power BI. The dashboard transforms raw health data into interactive visualizations that allow users to explore disease cases, mortality rates, recovery outcomes, healthcare access, treatment costs, and other key public health indicators across different countries between 2000 and 2024.

Using interactive filters, drill-through analysis, maps, and other Business Intelligence features, the dashboard enables users to identify patterns, compare countries, and gain deeper insights into global health trends.

The goal of this project is to support evidence-based decision-making by presenting complex health data in a clear, interactive, and easy-to-understand format that can assist healthcare organizations, policymakers, and researchers in planning and allocating healthcare resources more effectively.

## Project Objectives

The dashboard was created to answer the following questions:

- Which diseases affect the largest number of people?

- Which countries have the highest mortality rates?

- How have disease cases changed over time?

- How does healthcare access affect recovery?

- Which countries may require more healthcare resources?

- What factors contribute most to disease burden?

## Power Query Transformations

The dataset was cleaned and prepared using Power Query before building the dashboard.

The main transformations included:

- Removing duplicate records

- Handling missing and invalid values

- Renaming columns for consistency

- Standardizing text values

- Trimming unnecessary spaces

- Correcting data types

- Creating calculated columns where necessary
<img width="1600" height="902" alt="WhatsApp Image 2026-08-05 at 6 29 26 PM" src="https://github.com/user-attachments/assets/5fe7b38a-e188-4672-aaa9-089867eb4c61" />


Creating dimension tables for:

- Date
<img width="1600" height="899" alt="WhatsApp Image 2026-08-05 at 6 31 55 PM" src="https://github.com/user-attachments/assets/0ecc563f-397f-4252-b481-b9ac95e47967" />

- Country
  <img width="1600" height="887" alt="image" src="https://github.com/user-attachments/assets/30b87197-7700-45c8-9b6a-aef702881f4e" />


- Disease
<img width="1600" height="899" alt="image" src="https://github.com/user-attachments/assets/8498978e-c2a9-4679-97c2-ad5e1033c9ea" />


- Treatment
<img width="1600" height="899" alt="image" src="https://github.com/user-attachments/assets/fff1438a-9e75-4f67-9cde-ada757e235ba" />


- Demographics
<img width="1600" height="898" alt="image" src="https://github.com/user-attachments/assets/dd66cc85-6d22-409f-bdf7-f9cf995ae25f" />

Building a Star Schema data model to improve performance
<img width="1600" height="898" alt="image" src="https://github.com/user-attachments/assets/f84ba535-c4c7-4bd6-9da7-56ab22442312" />

These transformations improved the quality, consistency, and reliability of the data used for analysis.
## Data Model

The dashboard follows a Star Schema, which is commonly used in Business Intelligence because it improves performance and simplifies data analysis.

Fact Table

Fact_HealthRecords

Dimension Tables

Dim_Date

Dim_Country

Dim_Disease

Dim_Treatment

Dim_Demographics
<img width="1600" height="905" alt="image" src="https://github.com/user-attachments/assets/99fdea7b-8a35-4919-8944-bca1caaeb997" />

The fact table stores the health records, while the dimension tables provide descriptive information that allows users to filter and analyze the data from different perspectives.

## DAX Measures Created

Several DAX measures were created to support calculations and interactive analysis within the dashboard.

These include:

Total Cases

Average Mortality Rate

Average Recovery Rate

Total Treatment Cost

Total Population Affected

Average Healthcare Access

Dynamic Dashboard Title

Recovery rate status

Cost Category

High Risk Indicator

These measures update automatically based on the filters selected by the user.
<img width="1600" height="901" alt="image" src="https://github.com/user-attachments/assets/25cabd6e-1270-4785-928e-ff54b0fbe007" />

## Dashboard Pages
## Executive Summary

The Executive Summary provides a high-level overview of global public health performance through key performance indicators (KPIs) and summary visualizations. It allows users to quickly assess disease burden, treatment costs, mortality, and recovery rates before exploring the dashboard in more detail.
Visuals Used;

KPI Cards (Total Cases, Average Mortality Rate, Average Recovery Rate, Total Treatment Cost)

Clustered Bar Chart (Disease Cases by Category)

Line Chart (Total Disease Cases Over Time)

Interactive Slicers (Country, Disease Category, and Year)

Purpose

This page allows decision-makers to quickly understand the overall disease burden, mortality, recovery rates, and treatment costs before exploring the data in greater detail.

![alt text](<Screenshot 2026-08-05 154211.png>)

## Trend Analysis

The Trend Analysis page examines changes in disease burden and health outcomes over time. It enables users to identify long-term trends, compare mortality and recovery rates, and observe how disease categories have changed throughout the years.

Line Chart (Mortality vs Recovery Rate Trends)

Ribbon Chart (Disease Category Ranking Over Time)

Matrix (Country Mortality Rate by Year with Conditional Formatting)
Purpose

It helps users identify long-term disease trends, compare mortality and recovery rates over the years, and observe changes in disease rankings.

![alt text](<Screenshot 2026-08-05 154507.png>) 

## Geographic Analysis

This page compares public health indicators across different countries and regions.

Visuals Used
Filled Map (Disease Burden by Country)

Treemap (Disease Cases by Category and Disease)

Scatter Plot (Healthcare Access vs Per Capita Income)

Purpose

It enables users to identify countries with the highest disease burden, compare healthcare access, and understand regional health inequalities.

![alt text](<Screenshot 2026-08-05 154624.png>)

## Detailed Analysis 
The Detailed Analysis page provides users with an interactive drill-through experience that allows them to explore health records at a more detailed level for individual countries and diseases.

Visuals Used
Drill-through Table (Disease Records)

Decomposition Tree (Factors Influencing Disease Burden)

Back Navigation Button

Custom Report Tooltip
Purpose

Enables users to investigate specific countries and diseases, identify the factors contributing to disease burden, and gain additional context through drill-through and tooltip interactions.

![alt text](<Screenshot 2026-08-05 154724.png>)

## Key Insights
The dashboard provides several important insights into global public health.

1. Disease burden varies significantly across countries.

Some countries consistently report higher disease cases than others, indicating the need for targeted healthcare interventions and better resource allocation.

2. Healthcare access has a positive impact on recovery rates.

Countries with higher healthcare access generally achieve better recovery outcomes, highlighting the importance of investing in healthcare infrastructure.

3. Mortality rates differ even among countries with similar disease prevalence.

This suggests that healthcare quality, early diagnosis, and access to treatment play an important role in reducing deaths.

4. Disease trends have changed over time.

Trend analysis shows that while some diseases have remained stable, others have increased over the years, emphasizing the importance of continuous monitoring.

5. High treatment costs do not always lead to lower disease burden.

Some countries continue to experience high disease prevalence despite increased treatment spending, suggesting that preventive healthcare strategies should receive greater attention.

## Recommendations

Based on the dashboard findings, we recommend the following:

Increase investment in healthcare infrastructure in countries with high disease burden.

Strengthen preventive healthcare programs such as vaccination, awareness campaigns, and early disease screening.

Allocate healthcare resources based on disease burden and regional health needs.

Improve access to quality healthcare services in underserved regions.

Continue using data-driven dashboards to monitor disease trends and support evidence-based decision-making.

## Storytelling

The dashboard follows a logical flow that allows users to move from a broad overview of global health to more detailed analysis.

The Executive Summary introduces the overall health situation through KPIs and summary charts, giving decision-makers a quick understanding of disease burden, mortality, recovery, and treatment costs.

The Trend Analysis then explores how disease cases and health outcomes have changed between 2000 and 2024, helping users identify long-term trends and changes in disease rankings.

The Geographic Analysis shifts the focus to regional comparisons by showing how disease burden, healthcare access, and economic factors vary across countries. These visuals make it easier to identify health inequalities and regions that may require additional healthcare investment.

Finally, the Detailed Analysis allows users to drill down into individual countries and diseases. Through the decomposition tree and detailed records, users can investigate the factors influencing disease burden and make more informed decisions based on specific health indicators.

Together, the dashboard transforms complex health data into meaningful insights that support evidence-based public health planning and resource allocation.
