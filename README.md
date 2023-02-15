# Data-Engineering-for-Trending-Youtube-Video-Analysis in AWS

## Objective:

Develop a data pipeline in AWS to manage, streamline, and transform the structured and unstructured data containing 200+ trending youtube videos dataset to perform analysis based on categories and trending metrics. 

## Technology Stack
* Python 
* Spark
* AWS - S3, IAM, Glue, Athena, Lambda, Quicksight, AWS CLI

## AWS Services
* IAM (Identity Access Management): This allows to control access to AWS services and resources securely by assigning roles and attaching policies.
* Amazon S3: Used for storing raw and cleaned data in different buckets.
* AWS CLI: Used to ingest data from local to secure S3 buckets on AWS.
* AWS Glue: Created Data Catalogs by using crawlers in Glue for both raw and cleaned data.
            Also performed ETL operations in Glue to partition the data based on region, convert the format to parquet, perform joins and store it in S3 reporting.
* AWS Athena: Used for querying SQL commands, create databases and verify the outputs.
* AWS Lambda: Used to write and test the python script for converting the data in json format to parquet and storing the cleaned version in new S3 bucket.
              Also creating triggers on S3 buckets to automate the above ETL process on the data whenever there is any change in the bucket. 
* AWS Quicksight: Its a business intelligence (BI) service built for the cloud and was used to create interactive dashboards to visualiza and gain insights on various factors and features associated with trending videos.

## Dataset

https://www.kaggle.com/datasets/datasnaek/youtube-new

This dataset includes several months of data on daily trending YouTube videos. Data is included for the US, GB, DE, CA, FR, RU, MX, KR, JP and IN regions(USA, Great Britain, Germany, Canada, France, Russia, Mexico, South Korea, Japan and India respectively), with up to 200 listed trending videos per day.
Each region’s data is in a separate file. Data includes the video title, channel title, publish time, tags, views, likes and dislikes, description, and comment count.
The data also includes a category_id field, which varies between regions. To retrieve the categories for a specific video, find it in the associated JSON. One such file is included for each of the five regions in the dataset.

## Architecture


## Project Learnings
* Data Ingestion
* Data Lake 
* ETL Operations
* Cloud
* Reporting
