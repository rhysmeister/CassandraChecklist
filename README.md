# Cassandra Checklist

A checklist to ensure smooth operation of your Cassandra Clusters. Many of the checks here can, and should, be automated but will not be discussed in detail.

# Backups

For each node ensure the following according to your backup policy...

* Ensure recent snapshot exists and has been synced to an external location.
* Ensure incremental backups are running and files are synced to an external location.
* Ensure commitlog archive backups are running and files are synced to an external location.
* Ensure config backups are running and files are synced to an external location.
* Ensure schema backups are running and files are synced to an external location.
* Check for any recent errors in the backup process.
* Check snapshot syncronisation times are within expected limits.

# Cassandra Metrics

The following metrics should be checked daily at the cluster and node level...

TODO - Add Appropriate JMX Metrics for the below categories

* Errors -
* Throughput -
* Latency -
* Resource Saturation -
* Bottlenecks -
* Compactions -
* Flushes -
* Health -  
