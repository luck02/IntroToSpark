# Intro to spark
## What is spark?


Spark is a distributed compute platform.


Great!  What's a distributed compute platform?


We call spark a distributed compute platform because it provides a
*relatively* (haha) simple way of scaling out a job across multiple units of execution.


We break a job in spark into the following architectural units:
* Driver:
  * Runs the actual script.
  * Contains the core logic and orchestration.
* Executor:
  * Executes the individual actions on a given set of partitions.


![spark-architecture](./markdown/cluster-overview.png)

source:

https://spark.apache.org/docs/latest/cluster-overview.html


What this roughly means is that when you write a spark program you are manipulating datasets, a dataset can be
partitioned across multiple executors and be executed on in parallel.

Note:
This will only display in the notes window.