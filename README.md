# Health-Subsidy-Optimization-Model
Maximizing uncompensated hospital care cost-avoidance in Sacramento (Rating Region 3) using a constrained state budget to subsidize commercial health insurance.
[Live Project Link](https://docs.google.com/spreadsheets/d/1oZzUwJHN-a5AjfPh4SHMomKkBjxNMKKCHfgr2KYhE3Q/edit?usp=sharing)

# Project Objective
Analyze existing patterns in uncompensated hospital care costs in the Sacramento area (Rating Region 3) using  using publically sourced data. Once patterns and trends have been identified, devise and assess various state-based solutions to reduce state spending and provide health benefits to the Sacramento area.

# Methodology and Adjustments

## Data Aquisition 
For this project, I used the U.S. Census Bureau's Small Area Health Insurance Estimates ([SAHIE] (https://www.census.gov/data/datasets/time-series/demo/sahie/estimates-acs.html)) program to get the respective rates of insurance and uninsurance for various demographic groups. By filtering the data to California, Sacramento, I focused the project to specifically the Sacramento area to build a more precise picture. Using this data, we can identify which populations are most prone to risk from both a personal and state perspective. 

To build a baseline estimate for the mean severity and frequency of uncompensated hospitalizations in the Sacramento area, I used California's Department of Health Care Access and Information database (HADR) on healthcare expenses to isolate and sum the total costs of uncompensated care across the area. I also used the database to get a count of the year's total instances uncompensated care. With the total count of uninsured individuals in the Sacramento area, we can build a rough estimate for the average frequency of uncompensated hospitalizations among uninsured individuals. 

## Adjustments
Since HADR does not disclose patient demographics for privacy purposes, it was not possible to organically build a distribution to model each demographic's relative risk and frequency. To compensate, I used less granular data with specific information to build a table of relative severity and frequency multipliers for each demographic. Once these multipliers were calculated, I applied them to the Sacramento's base frequency and severity to approximate the average cost and frequency of uncompensated hospital stays for each poplulation in Sacramento. 