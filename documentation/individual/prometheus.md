# Prometheus

We can access the Prometheus web interface by going to `http://localhost:9090`
in our browser.

Under the `Status` menu, we can see the list of targets that Prometheus is
scraping. We can see that Prometheus is scraping itself and Node Exporter.
As per our configuration, Prometheus is scraping every 15 seconds.

Under the `Graph` menu, we can see the list of metrics that Prometheus is
collecting.

Let's try to search for the number of allocated file descriptors in the
metrics. To do so, we can search for the `node_filefd_allocated` metric.

The real time value of the metric should be displayed in the graph.
