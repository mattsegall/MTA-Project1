# MTA analysis for WTWY

## Contributors
Michael Jehl, Matt Segall, Nathaniel Speiser

## Description

The goal of this project was to do EDA and data visualization on MTA turnstile data in order to make recommendations to WomenTechWomenYes about their street team allocation. We gave reccomendations based on weighted median ridership of MTA stations in June 2019, as the gala is in early summer and we wanted to avoid abnormal data from during the pandemic. The weighted ridership was calculated by taking the raw daily median ridership and multiplying it by z/n, where z is the median income of the zip code the station is located in and n is the median income of NYC as a whole. The graph below shows the busiest stations by this weighted ridership metric. The zip codes of the stations were found with the Google Maps API and were used to find the income in the area around each station.

![graph](https://github.com/nathaniel-speiser/MTA-Project1/blob/main/pics/median_ridership_weighted.png)

## Data

[MTA turnstile data](http://web.mta.info/developers/turnstile.html)

[Income data by zipcode](https://www.census.gov/)

## Tools

* pandas
* matplotlib
* seaborn
* Google Maps API


## Impacts

This project provides one way for WTWY (or any organization) to allocate street team resources to find potential wealthy donors. A number of other approaches are possible, including looking for areas around universities with STEM programs, tech campuses, or a variety of other locations. A possible future step would be to further refine the weighting process to include a coefficient that measures engagement at the station.
