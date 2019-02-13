## Design and implement Data pipeline to find the top 10 origin stations and/or top 10 destination stations.

Data: 
We will use the [GoBike Bay Area Data](https://www.fordgobike.com/system-data) OR [CitiBike Data](https://s3.amazonaws.com/tripdata/index.html). 

It has below attributes: "tripduration","starttime","stoptime","start station id","start station name","start station latitude","start station longitude","end station id","end station name","end station latitude","end station longitude","bikeid","usertype","birth year","gender"

Steps for Data pipeline:
1. Download data from S3. 
2. Extract and upload data to HDFS. 
3. Clean and process the data. 
4. Create Parquet files of data using Spark. 
5. Store the top 10 results daily to ?? 

The pipeline should run daily using the Airflow\Oozie.

Tech:
1. HDFS Yarn for Storage of Parquet. 
2. Airflow for Orchestration 
3. Spark with Scala 
4. AWS SDK, S3cmd for interacting with AWS. 
5. ? as final data Storage


We can use data from https://www.kaggle.com/benhamner/sf-bay-area-bike-share/data. 

Detailed link for Citibike data: https://www.citibikenyc.com/system-data

——————————————————————————————————————————————————