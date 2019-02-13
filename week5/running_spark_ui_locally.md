## Monitoring Performance
To understanding implications of different code on performance, we first need to understand how to monitor performance locally.  Here we are going to use the example of the batch-data-pipeline repo to analyze performance.


## Things to note:
[Good document on monitoring Spark](https://spark.apache.org/docs/2.3.0/monitoring.html)

## Use the above documentation to set up Spark monitoring locally. Note that Spark requires that a directory /tmp/spark-events be created beforehand. 
Run your citibike solution
Note how long it took in compute time
Rewrite the solution without using UDF
Note how long this new code took in compute time

## Lesson Learned:
Note that in Spark it’s really important to do your research to learn which functions are already built in spark.  When you use these functions then spark can better optimize them with the catalyst. 
