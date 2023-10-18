# Node-Exporter

Node Exporter is an agent that collects metrics about the host machine and
sends them to Prometheus.

We can access the metrics collected by Node Exporter by going to
`http://localhost:9100/metrics` in our browser.

Node exporter exports a lot of metrics, some of them are easily understandable
and some of them are not. Even if we don't understand all the metrics, they can
still be useful to us.

Let's try to search for the number of allocated file descriptors in the metrics.

```sh
curl -s http://localhost:9100/metrics | grep node_filefd_allocated
```

The metric is not only composed of a name and a value, it also has labels that
give us more information about the metric:

The `help` label that gives us a description of the metric.

The `type` label that tells us that the metric is a `gauge`. A gauge is a metric
that can go up and down over time.
