# Street Team Placement Proposal for WTWY International
#### Manveer Sadhal
#### Sep 8, 2021

## Question/Need

WomenTechWomenYes (WTWY) International has approached Metis for help in gathering and analyzing data to help them position street teams for promotion of a gala scheduled for the beginning of summer. They are seeking guidance based primarily on MTA subway traffic data.

The goal of this analysis will be to recommend specific locations for placement of street teams to maximize gala attendance and contributions to WTWY International. We will be aiming to identify high traffic MTA turnstiles in New York City, ideally where future supporters of WTWY will pass through.

## Data Description

The primary data set that will be examined in this analysis is [MTA turnstile data](http://web.mta.info/developers/turnstile.html) in NYC which is freely available. Emphasis will be placed on data in the first half of the year (Jan-Jun) since the gala will be held at the beginning of summer. Data prior to and after the start of the COVID-19 pandemic will be explored in an effort to provide suitable options for different scenarios in the upcoming year depending on the trajectory of the spread of the virus and corresponding mitigation efforts.

Traffic patterns will be analyzed both on a weekly basis to determine the best days of the week as well as on a daily basis to determine the best time of day to target given turnstile locations.

Additional demographic data (e.g. census data) may be analyzed to further focus promotional efforts into areas where higher conversion rates are expected.

An individual sample from the MTA turnstile data will be the number of entries and exits from a specific turnstile on a given date, aggregated every four hours.

## Tools

A variety of tools including an assortment of Python packages will be used to complete the analysis required for this project. The Python tools will be used as part of a Jupyter Notebook.

- Data Ingestion and Storage
    - SQLite with DB Browser
    - SQLAlchemy to query imported data
- Data Cleaning
    - Pandas
- Exploratory Data Analysis
    - Pandas
    - DB Browser
- Data Visualization
    - Matplotlib
    - Seaborn

## Minimum Viable Product (MVP) Goal

The minimum viable product for this project would be determining which subway stations have the highest traffic through turnstiles as a starting point for where WTWY should place street teams.

This will be presented using visualizations and brief text to explain the conclusions of the analysis.