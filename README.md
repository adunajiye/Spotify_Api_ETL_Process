# Spotify_Api_ETL_Process
Key points of this Project 
1. Extracts DData from API
2. Build an automated trigger to run data pipelines (EventBridge Trigger)
3. Extracts and transform jobs (Lambda) and store raw data (s3)
4. Build the correct bucket structure  for data storage
5. Automate transformation job (s3) for a new data
6. Build analytics layer for SQL queries and business intelligence (Athena)

# Architecture
![WhatsApp Image 2023-06-22 at 6 26 59 PM](https://github.com/adunajiye/Spotify_Api_ETL_Process/assets/80220180/79be9dcd-9cf2-459f-ad4a-dde2b35cc1fe)

# Tools Used
Python, AWS Services( CloudWatch,Lambda,s3,Glue,Athena)
Brief Overview of each services used:
1. S3(Simple Storage Service): Easily stores and retrieve large amount of data. Each file is called an object and data is stored in buckets
2. Lambda: Serverless compute service to run code with managing servers. we will use lambda to deploy the python code to perfrom data extraction and transformation
3. EventBridge: Creates and manage events, scehdule them based on a defined pattern or crom expression
4. CloudWatch: Monitor and collect metrics from AWS resources. itcan be used to monitor log fie and set alarms
