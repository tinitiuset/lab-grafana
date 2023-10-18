# What makes an observability stack?

An observability stack is a set of tools that allows us to monitor and
understand the state of our systems and applications. 

The main components of an observability stack are:

- Metrics: A metric is a measurement of a system's state. Metrics are usually
collected at regular intervals and are used to understand the behavior of the
system over time. 

- Logs: Logs are records of events that happened in a system. Logs are usually
used to understand the behavior of the system at a specific point in time.

- Traces: Traces are records of the path of a request through a system. Traces
are usually used to understand the behavior of the system when handling a
request.

The observability stack we will be using in this lab is composed of the
following components:

- Grafana: A visualization tool for metrics and logs.

- Prometheus: A metrics database and a metrics collection and aggregation engine.
- Node Exporter: An agent that collects metrics about the host machine and sends
  them to Prometheus.
- cAdvisor: An agent that collects metrics about the containers running on the
  host machine and sends them to Prometheus.

- Loki: A logs database and a logs collection and aggregation engine.
- Promtail: An agent that collects logs and sends them to Loki.








