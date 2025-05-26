🌍 Global Warming Trend Analysis - City Temperature Data

This project analyses long-term temperature trends across thousands of global cities using R.The goal is to identify patterns of climate warming, understand regional and hemispheric differences, and highlight the most affected areas.

📊 Objectives

🌡️ Analyse temperature trends in cities worldwide over time

🌍 Compare warming rates across regions and hemispheres

🚦 Classify cities into risk zones based on warming intensity

🔥 Identify cities with the fastest warming trends

📉 Examine areas with the lowest or slowest warming rates



🔍 Dataset

Source: GlobalLandTemperaturesByCity.csv

Data Period: 1743 to 2013

Columns Used: City, Country, Latitude, Longitude, AverageTemperature, dt

Processed Columns: Trend, RiskZone, Hemisphere, Region


🧪 Tools & Libraries Used

Language: R

IDE: RStudio

Libraries: tidyverse, lubridate, dplyr, ggplot2, broom, scales


📈 Key Insights

Global Average Warming Trend: 0.0067 °C/year

Trend vs. Latitude: Negative correlation (r = -0.507), indicating faster warming in lower latitudes (tropical zones)


Risk Levels:

🔴 Moderate/High Warming: 2,738 cities

🟢 Low Warming: 772 cities


By Region:

🧊 Temperate/Northern: 0.0060 °C/year

🌿 Temperate/Southern: 0.0081 °C/year

🔥 Tropics: 0.0077 °C/year


By Hemisphere:

🌎 Northern: 0.0064 °C/year

🌏 Southern: 0.0084 °C/year


🔥 Hottest Cities (Top 5 Trends)

| City     | Country | Trend (°C/year) |
| -------- | ------- | --------------- |
| Edmonton | Canada  | 0.0114          |
| Doha     | Qatar   | 0.0106          |
| Talara   | Peru    | 0.0106          |
| Bojnurd  | Iran    | 0.0105          |
| Kurgan   | Russia  | 0.0105          |


❄️ Least Warming Cities

| City      | Country | Trend (°C/year) |
| --------- | ------- | --------------- |
| Algeciras | Spain   | 0.00278         |
| Tangier   | Morocco | 0.00278         |
| Sevilla   | Spain   | 0.00287         |


🛠️ How to run, download or clone this repository

Place GlobalLandTemperaturesByCity.csv in your R working directory.

Run the R script city_warming_analysis.R to reproduce the analysis.

View tables and visualisations in the RStudio console and Plots pane.


📂 Project Structure

city_warming_analysis.R — Main analysis script

GlobalLandTemperaturesByCity.csv — Dataset used for analysis

README.md — Project overview and documentation

📌 Notes

The dataset contains over 3,500 cities with daily data processed into long-term warming trends.
Risk classification is based on the linear regression slope per city.
Code includes filtering, aggregation, correlation, and ranking of results.




