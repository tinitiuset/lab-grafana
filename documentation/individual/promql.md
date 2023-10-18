# PromQL

PromQL is the query language used to query Prometheus. It is a functional
language that allows us to select and aggregate metrics.

## Basic Queries

### Selecting a metric

To select a metric, we can use its name. For example, to select the `node_cpu`
metric, we can use the following query:

```promql
node_filefd_allocated
```

### Filtering by label

To filter a metric by label, we can use curly braces (`{}`) to specify the label

For example, to select the `node_cpu` metric with the `cpu` label set to `cpu0`,

```promql
node_filefd_allocated{job="node_exporter"}
```
