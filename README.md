# Chicago Taxi Trips Data Engineering ETL Project

This project is a comprehensive data engineering pipeline that processes and analyzes Chicago taxi trips data. 
It utilizes a variety of tools and services, primarily focusing on Python and AWS, to efficiently extract, transform, and load (ETL) data for further analysis.

## Data sources used:

- Chicago Taxi Trips Data: The primary dataset comes from the City of Chicago's open data portal ([https://data.cityofchicago.org/]), which provides detailed records of taxi trips within the city.
- Weather Data: Daily weather data relevant to the taxi trips is fetched from the Open-Meteo API ([https://open-meteo.com/])
- Community Area Information: Community area names, corresponding to the numeric IDs in the taxi trip data, were scraped from Wikipedia to enrich the dataset.
