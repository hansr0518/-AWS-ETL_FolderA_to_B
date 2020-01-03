# [AWS] ETL job using Glue 
Two types of ETL Process
1. ETL Job without Data Cleansing.
2. ETL job with Data Cleansing process.
> AWS Glue introduces the DynamicFrame.
>
> So for the Data Cleansing Process, I am going to convert DynamicFrames to DataFrames.

# Links
For the information about DynamicFrame & GlueContext

https://docs.aws.amazon.com/glue/latest/dg/aws-glue-api-crawler-pyspark-extensions-dynamic-frame.html

# Installation
```python
import sys
from awsglue.transforms import *
from awsglue.utils import getResolvedOptions
from pyspark.context import SparkContext
from awsglue.context import GlueContext
from awsglue.job import Job
from awsglue.dynamicframe import DynamicFrame
from pyspark.sql.functions import from_unixtime,col
```
