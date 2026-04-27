# Japan's Aviation Industry During Covid-19 (2020-2021)

## Overview
This project analyzes Japan's domestic and international 
air traffic patterns during the COVID-19 pandemic using 
flight data from the OpenSky Network. The goal was to 
understand how COVID-19 impacted different routes, airports, 
and airlines across Japan between 2020 and 2021.

## Why PySpark
The dataset contains 51 million rows across 2020-2021. 
PySpark was chosen over Pandas due to memory constraints 
at this scale. All heavy filtering, aggregation, and 
window function calculations are performed in Spark. 
Aggregated results are converted to Pandas for 
visualization.

## Tech Stack
- PySpark — large-scale data processing
- Pandas — post-aggregation analysis and plotting
- Matplotlib — exploratory visualization
- Tableau — interactive dashboard

## Key Analysis
- Monthly flight volume trends with month-over-month 
  percentage change
- Domestic vs international flight breakdown
- Inbound and outbound traffic by airport (RJAA, RJTT, 
  RJBB, RJFF, RJOO, RJCC)
- Airline-level traffic analysis (JAL, ANA, Peach, 
  Skymark, Jetstar Japan)
- Correlation between COVID-19 case counts and flight 
  activity
- Least busiest day identification (May 4, 2020 — 
  117 flights)

## Key Findings
- April 2020 saw the sharpest decline at -52% 
  month-over-month, coinciding with Japan's first 
  state of emergency
- International inbound flights dropped more severely 
  than domestic routes
- 2021 showed a 58.9% year-over-year recovery compared 
  to 2020

## Dashboard
Interactive Tableau dashboard visualizing airport and 
airline recovery trends:
https://public.tableau.com/app/profile/alexander.aryasena/viz/japanflight_analysis/Dashboard1

## Data Source
OpenSky Network — worldwide flight observations from 
2,500+ network members
