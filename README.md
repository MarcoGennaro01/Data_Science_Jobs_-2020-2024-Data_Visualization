# data-science-salaries
## TL;DR
This data visualization project analyzes global **data science roles**, adjusting for **cost of living**, based on the [**Data Science Salaries 2024**](https://www.kaggle.com/datasets/sazidthe1/data-science-salaries) dataset from Kaggle (credits to [Sazidul Islam](https://www.kaggle.com/sazidthe1)).

- **Highest salaries** are found in countries like the **USA**, **Canada**, and the **UK**.
- However, European countries like **Italy**, **Spain**, and **Portugal** offer **more fully remote opportunities**.
- The project explores patterns by **country**, **role**, and **experience level**, with adjustments for **cost of living** to provide fairer comparisons.

The mission of the project is to help new data professionals to make informed decisions about their careers in a rapidly changing job market.

## Introduction
This notebook analyzes the 2024 Data Science Salary Survey dataset, which contains information about salaries, job titles, locations, and other relevant factors for data professionals worldwide. The goal is to provide insights into the current state of the data science job market, including salary trends, job demand, and regional differences. The results aim to help data professionals make informed decisions about their careers in a rapidly changing job market.

## Data cleaning
A good portion of the project revolves around cleaning the data. The dataset contains a lot of unclear and really specific roles. For the sake of simplicity, I kept just 4 roles: Data Scientist, Data Analyst, Machine Learning Engineer and Data Engineer, accounting for about 2 thirds of the dataset. Finally, I imported geographic data into a geopandas dataframe to be able to plot the results on a choropleth plot and PPP indexes per country to adjust salaries for cost of living using the [**World Bank PPP dataset**](https://ourworldindata.org/grapher/ppp-conversion-factor-for-private-consumption).

## Data visualization
The visualization part is done using the [**Plotnine**](https://plotnine.org/) library, a Python implementation of ggplot2. The visualizations are focused on the salaries distribution by role, by country, remote working percentages, their behavior in the 2020-2024 period, and the inequality in salaries per country and role. 
