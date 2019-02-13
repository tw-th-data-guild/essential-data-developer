
## Pre-requisite
apache-spark, sbt

## Steps
First some things to notice:
Spark Submit Details - [here is some useful documentation](https://spark.apache.org/docs/latest/submitting-applications.html).
Test files like big.txt are located in the sample-data folder
We need to use a config.jar for the spark submit job that is located at the root folder
Brew install apache-spark if you haven’t done so already

Update application.conf in the TW-pipeline > src > main > resources folder should be updated with input and output paths that work for you.  
For me this looks like:
WordCount{
 input="/Users/keyadesai/batch-data-pipeline/sample-data/big.txt"
 output="/Users/keyadesai/transformedData"
}

Run sbt package
Take a look at the build.sbt file in tw-pipeline to understand more about what we have configured

cd to the tw-pipeline folder and run the following spark-submit command
spark-submit --jars ../config-1.3.2.jar --class com.thoughtworks.ca.de.batch.wordcount.WordCount --master local target/scala-2.11/tw-pipeline_2.11-0.1.0-SNAPSHOT.jar 

Take a look at your results
