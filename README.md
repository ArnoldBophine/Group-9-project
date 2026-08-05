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

## Project Objectives

The dashboard was created to answer the following questions:

Which diseases affect the largest number of people?

Which countries have the highest mortality rates?

How have disease cases changed over time?

How does healthcare access affect recovery?

Which countries may require more healthcare resources?

What factors contribute most to disease burden?

## Power Query Transformations

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

Recovery Rate Status

Cost Category

High Risk Indicator

These measures update automatically based on the filters selected by the user.

## Dashboard Pages
## Executive Summary

The Executive Summary provides a quick overview of the overall public health situation using key performance indicators and summary charts.

Visuals Used;

KPI Cards

Clustered Bar Chart

Line Chart

Interactive Slicers

Purpose

This page allows decision-makers to quickly understand the overall disease burden, mortality, recovery rates, and treatment costs before exploring the data in greater detail.

## Trend Analysis

This page focuses on how disease cases and health outcomes have changed over time.

Visuals Used
Multi-Line Chart
Ribbon Chart
Matrix with Conditional Formatting
Purpose

It helps users identify long-term disease trends, compare mortality and recovery rates over the years, and observe changes in disease rankings.

## Geographic Analysis

This page compares public health indicators across different countries and regions.

Visuals Used
Filled Map
Treemap
Scatter Plot
Purpose

It enables users to identify countries with the highest disease burden, compare healthcare access, and understand regional health inequalities.

## Drill-through Detail

## Toolpit

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
