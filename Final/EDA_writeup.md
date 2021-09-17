# Street Team Placement for WTWY, Inc. - Exploratory Data Analysis
Manveer Sadhal

## Abstract
The goal of this exploratory data analysis project was to offer guidance to WomenTechWomenYes, Inc. on the best locations to place their street teams for promotion of the next summer gala. The primary data source was [New York City Metropolitan Transportation Authority (MTA) turnstile data](http://web.mta.info/developers/turnstile.html).
Data was ingested from a SQL database into dataframes using the Python modules SQLAlchemy and Pandas and cleaned. After cleaning, data was plotted using Matplotlib and Seaborn, then analyzed to formulate specific recommendations to aid WTWY's promotion efforts. The primary period evaluated for turnstile data was January to June 2019. Additional periods from the spring of 2020 and 2021 were similarly evaluated.

## Design
The hypothetical scenario of providing data-driven insights to WTWY to help effectively promote their event was presented by the Metis team. The intent of the analysis was to determine locations and times where WTWY street teams could promote their upcoming summer gala with the most impact, leading to more sign ups to the organization's email list. This would in turn increase gala participation, and ultimately advance the organization towards their goal of increasing representation of women in technology.

## Data
Data used for this analysis was from the NYC MTA. Data is available by individual turnstile from all of the 472 stations, with cumulative counts typically updated every four hours.
January to June 2019 were chosen as the period to evaluate subway traffic. The gala is planned for the beginning of summer, so the first half of the year was selected since this is the period during which WTWY will promote the event. Due to the COVID-19 pandemic, subway ridership was drastically reduced during 12-week periods in the spring of 2020 and 2021, which were similarly evaluated as part of this analysis. 2019 is considered to be the most recent period which will be representative of the promotional period for the gala planned for summer 2022.


## Algorithms
### Cleaning
Cleaning was performed using the Python module Pandas. Duplicate data was first removed. Duplicate line names were also standardized to ensure accurate aggregation during analysis.
Erroneous values for the number of entries during a given date or time of day were removed, primarily occurring on the first or last day of the evaluated period. Other anomalies in the data caused by events such as counters reaching their maximum value and resetting were also removed by examining the distribution of entries and determining reasonable thresholds for the true number of entries. Data outside of this range was discarded.

### Visualization
Total entries over a given time span, monthly trends, weekly trends, and intraday trends were plotted using Matplotlib and Seaborn to evaluate the data and offer specific recommendations to the client.


## Tools
- Data Ingestion and Storage
    - SQLite with DB Browser
    - SQLAlchemy to query imported data
- Data Cleaning
    - Pandas
- Exploratory Data Analysis
    - Pandas
- Data Visualization
    - Matplotlib
    - Seaborn


## Communication
Findings and recommendations from the exploratory data analysis will be communicated during a 5-minute slide presentation.
