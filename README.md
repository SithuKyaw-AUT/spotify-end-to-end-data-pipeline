# Spotify End-to-end Data Engineering Project
In this project, I build an ETL pipeline using Spotify API on AWS. I retrieve data from the Spotify API, transform it to a desired format, and then load it into an AWS data storage.

## Services Used
1. S3 (Simple Storage Service)
2. Lambda
3. Cloud Watch
4. Glue Crawler
5. Data Catalog
6. Athena

## About data/API
The Sportify API contains the information about music album, artists and songs. [Spotify API](https://developer.spotify.com/documentation)

## Dataflow
Extract data from API ==> Trigger extract lambda function (every 1 hour) ==> Extract data by the lambda function ==> Store data temporarily in Raw_data ==> Trigger transform lambda function ==> Transform and save data ==> Glue crawlers ==> Tables in Data Catelog ==> Query using Athena
