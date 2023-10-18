# Loki

Loki is a logs database and a logs collection and aggregation engine. It is
designed to be used as a companion to Prometheus.

For Loki to be able to collect logs, we need to configure our applications to
send their logs to Loki. We will use Promtail to do so.

We can query Loki using PromQL. We can also use Grafana to visualize the logs
collected by Loki.