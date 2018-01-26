# Important Concepts:


## Datasets / Dataframes:
Blurb about ds/df


## Partitions:
In order to achieve parallel processing on a large dataset Spark will slice your dataset into row-wise sections and
parcel them out to executors to process.


The mechanism by which partitions are created can be as transparent as you like and we can gain really significant
performance improvements by defining partition keys.


When we define a partition key we tell spark to keep a given data set local on an executor.  This is specifically very
effective when we're joining diverse data sets.  Presumably both datasets share a common field that you'll be joining
on.  If that's the case we can realize significant performance improvements by defining a common partition key.

Executors operate on partitions at at time.

Executor != partitions.

df.mapPartitions why this is awesome and what pattern it assists.


## sadf