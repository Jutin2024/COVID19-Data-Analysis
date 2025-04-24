![image](https://github.com/user-attachments/assets/1a56c686-ba39-4993-8922-b0297958b0d6)
# `COVID-19 Data Analysis` ![Python](https://img.shields.io/badge/python-3.11-blue?logo=python&logoColor=white) ![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter&logoColor=white)
This project explores and visualizes the global impact of the COVID-19 pandemic using data from the [Our World in Data](https://ourworldindata.org/coronavirus) repository. The dataset provides a comprehensive overview of the pandemic's global effects, drawing from reliable sources such as the World Health Organization (WHO), the Centers for Disease Control and Prevention (CDC), and numerous national health ministries.

## Introduction

COVID-19, first reported in Wuhan, China in 2019, evolved into a pandemic affecting millions worldwide. Using publicly available data from credible sources (WHO, CDC, and national health bodies), this analysis focuses on:
- Geographic spread and impact across continents and countries
- Temporal trends of infections, deaths, and vaccinations
- Socioeconomic and demographic factors influencing mortality

## Approach

### 1. Overview of COVID-19 Data
- Tried to understand the data
- Continent wise snapshot of the pandemic situation at the end of 2020
  - Choropleth maps of COVID impact by country
- Key metrics: cases, deaths, vaccinations, testing, and macroeconomic indicators.
### 2. Summarizing
- Cleaned and filtered large COVID-19 datasets to retain key metrics:
  - Total cases, total deaths, deaths per million, vaccination rates, testing rates
- Normalized metrics per million people for fair comparisons
- Introduced death rate and excess deaths to uncover deeper insights
### 3. Visualizing
- Created interactive, web-friendly visualizations including:
  - Time-series plots normalized by start date (`T0`) of the pandemic in each country
  - Log-scale plots to highlight early exponential growth trends
- Added context with:
  - Annotations and continent-based color coding
  - Exponential growth reference lines (e.g., doubling every 2, 5, 10 days)
- Visualizations saved as shareable interactive HTML files
### 4. Modeling with Linear Regression
-	Goal: Explain variation in COVID-19 deaths across countries using regression
-	Target variable: Total deaths per million (excess deaths limited by availability)
-	Explored key predictors:
    - Median age (strongest overall predictor)
    - Human Development Index (HDI) (more predictive early in pandemic) 
-	Performed systematic variable combination testing to find best-fit models
-	Explored vaccine rollout and its statistical correlation with COVID-19 outcomes

## Key Insights

- **Median age** is a strong predictor of COVID-19 fatalities: older populations faced higher risk.
- **HDI** was initially correlated with higher deaths (possibly due to better reporting) but later reversed when analyzing excess deaths.
- **Excess deaths** are more accurate than reported deaths but not available for all countries.

## Libraries Used
![Pandas](https://img.shields.io/badge/-Pandas-150458?logo=pandas&logoColor=white)
![Plotly](https://img.shields.io/badge/-Plotly-3F4F75?logo=plotly&logoColor=white)
![Statsmodels](https://img.shields.io/badge/-Statsmodels-3C3C3C?logo=python&logoColor=white)
![NumPy](https://img.shields.io/badge/-NumPy-013243?logo=numpy&logoColor=white)
