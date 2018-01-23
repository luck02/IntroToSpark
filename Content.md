1. What is spark
   1. What is a distributed compute framework
1. What is partitioning and why is it important.
1. When would you *need* spark vs. When you would *want* spark vs. when it's silly.
1. A quick background on our compute infra vis a vis spark
1. How to troubleshoot spark
1. How to ask for help and when to do it.
    1. How to troubleshoot spark here at UB
1. Common (sketchy) patterns.
    1. Subquery with non-sensical predicates in them.
        1. What is a subquery and what does it do?
    1. What is predicate pushdown and how does it work?
    1. Not partioning our reads and writes.
      1. How to partition reads and writes here at UB.
      1. DB query partioning.
      1. S3 file partitioning (Parquet)
      1. CSV partitioning (it can be done, but it won't compress / isn't columnar)
    1. Executing in the driver.
    1. Suboptimal for-each execution (optimize / minimize expensive external resources) 
      1. map.forEachPartition vs map.forEach
    1. What is a UDF
    1. Performance hit for pyspark
1. Uncommon good patterns:
   1. Testing your code, factoring for testing.
1. Telemetry and logging... Do it.
1. What is the Spark optimizer (catalyst).
1. What is 


Notes: https://www.qubole.com/blog/introducing-quboles-spark-tuning-tool/
