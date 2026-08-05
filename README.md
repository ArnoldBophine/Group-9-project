# Global Public Health Intelligence Dashboard

# Group Members
Susan Otieno - 670501


## Dataset Source

Source: Global Health Statistics Dataset

Platform: Kaggle

Dataset URL:
https://www.kaggle.com/datasets/malaiarasugraj/global-health-statistics?resource=download

## Dataset Description

The Global Health Statistics dataset contains health-related information collected from different countries between 2000 and 2024. It includes data on disease prevalence, incidence, mortality rates, recovery rates, healthcare access, treatment costs, population affected, demographic information, and socioeconomic indicators.

The dataset provides valuable insights into global health trends and helps identify patterns that can support better healthcare planning and decision-making.

## Business Problem
Public health organizations collect large amounts of health data every year, but making sense of this information can be difficult without the right tools. Decision-makers need a way to quickly identify disease trends, compare countries, monitor healthcare performance, and understand where resources are needed most.

For this project, our group developed a Global Public Health Intelligence Dashboard using Power BI. The dashboard transforms raw health data into interactive visualizations that help users analyze disease cases, mortality rates, healthcare access, treatment costs, and recovery outcomes across different countries from 2000 to 2024.

The goal is to support better decision-making by providing clear and interactive insights into global public health.

##Project Objectives

The dashboard was created to answer the following questions:

Which diseases affect the largest number of people?
Which countries have the highest mortality rates?
How have disease cases changed over time?
How does healthcare access affect recovery?
Which countries may require more healthcare resources?
What factors contribute most to disease burden?

##Power Query Transformations

The dataset was cleaned and prepared using Power Query before building the dashboard.

The main transformations included:

Removing duplicate records
Handling missing and invalid values
Renaming columns for consistency
Standardizing text values
Trimming unnecessary spaces
Correcting data types
Creating calculated columns where necessary
Creating dimension tables for:
Date
Country
Disease
Treatment
Demographics
Building a Star Schema data model to improve performance

These transformations improved the quality, consistency, and reliability of the data used for analysis.
