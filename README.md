# Chicago Taxi Trips Data Engineering ETL Project

This project is a comprehensive data engineering pipeline that processes and analyzes Chicago taxi trips data. 
It utilizes a variety of tools and services, primarily focusing on Python and AWS, to efficiently extract, transform, and load (ETL) data for further analysis.

## Data sources used

- Chicago Taxi Trips Data: The primary dataset comes from the City of Chicago's open data portal (https://data.cityofchicago.org/), which provides detailed records of taxi trips within the city.
- Weather Data: Daily weather data relevant to the taxi trips is fetched from the Open-Meteo API (https://open-meteo.com/).
- Community Area Information: Community area names - corresponding to the numeric IDs in the taxi trip data - were scraped from Wikipedia.

## Project Components

### AWS Services

- AWS S3: The project uses S3 to store raw and processed data. The folder structure is designed to facilitate efficient data retrieval and management.
- AWS Lambda: Two Lambda functions are deployed:
  1. Data Extraction Function: Handles the continuous extraction of taxi trip data and weather information.
  2. Data Transformation Function: Processes and transforms the raw data, preparing it for analysis.
- Triggers: AWS Lambda functions are triggered automatically to ensure the data pipeline operates continuously.
- AWS Glue: Creating a  data catalog based on the data in S3 and crawling it for further usage.
- AWS Athena: Used for Exploratory Data Analysis (EDA) with SQL-based querying of the processed data.

### Data Processing

- Web Scraping: A web scraping script collects community area names from Wikipedia, replacing the numeric IDs provided in the original dataset.
- Dimension Tables: Separate dimension tables are created for dates, payment types and companies to normalize the data and improve query performance.

Consider below charts as results of the EDA:


