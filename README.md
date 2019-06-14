# Cassandra Checklist

A checklist to ensure smooth operation of your Cassandra Clusters. Many of the checks here can, and should, be automated but will not be discussed in detail.

# Backups

For each node ensure the following according to your backup policy...

* Ensure a recent snapshot exists and has been synced to an external location.
* Ensure incremental backups are running and files are synced to an external location.
* Ensure commitlog archive backups are running and files are synced to an external location.
* Ensure config backups are running and files are synced to an external location.
* Ensure schema backups are running and files are synced to an external location.
* Check for any recent errors in the backup process.
* Check snapshot syncronisation times are within expected limits.
* Check disk space used by snapshots on each node (see TrueDiskSpaceUsed in nodetool listsnpashots output)

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
* Caches -
* Data Size -

# Nagios

* Check number and type of service alerts issued by each cluster node.

# Cassandra Maintenance Tasks

Checklist for repair and other maintenance tasks.
