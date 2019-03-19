# Week 5: Workflow Managment

## What will I learn?
Workflow Managment Layer - Airflow

## What should I learn in weekend?
1. Read
    [AirFlow Docs](https://airflow.apache.org)

2. Assignment
    [Please follow this tutorial](https://medium.com/@mozesr/basic-airflow-73361b62814f)

* Look at the DAG in the Batch data pipeline repo
    How are DAGs being scheduled?

* Create your own DAG that will 
    1. take data from a raw data directory 
    2. Transform it with daily driver
    3. Save it to a transformed data directory
    4. Read that data for Citibikes Transformation
    5. Run Citibikes Transformation on it
    6. Save it to a data mart directory

## What will we do in Guild?
1. Discussions on what we have learned so far...
2. Exercise
    * [Checkout](https://github.com/ThoughtWorksInc/batch-data-pipeline) and explore sample batch data pipeline in this codebase.
    * Discuss the architecture and each component.
    * [Run Spark submit locally](./running_spark_submit_locally.md).
    * [Setup Spark UI locally and explore](./running_spark_ui_locally.md).
    * Run airflow dags locally


## What if I want to know more!?
---

*Copyright (c) 2018 ThoughtWorks; for individual use for training purposes and not to be distributed or sublicensed without further authorisation by ThoughtWorks.*
