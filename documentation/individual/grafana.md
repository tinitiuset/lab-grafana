# Grafana

Grafana is a visualization tool for metrics, logs, and traces.

Grafana by itself does not collect any data. It is a frontend that allows us to
visualize data collected by other tools.

In this lab, we will use Grafana to visualize metrics collected by Prometheus
and logs and traces collected by Loki.

With our observability stack deployed, we can access Grafana at
`http://localhost:3000`.

We will be greeted by the login page. The default username and password are
`admin` and `admin`.

Once logged in, we will be greeted by the home page. The home page
will guide us through the process of adding a data source and creating a
dashboard.

We will start by adding Prometheus as a data source. To do so, we can click on
the `Add data source` button.

In the data source configuration page, we can select `Prometheus` as the type
of data source. We can then configure the URL of the Prometheus server. In our
case, the URL is `http://prometheus:9090`. We can then click on the `Save &
Test` button to test the connection to the Prometheus server.

We should be able to add Loki as a data source in the same way. The URL of the
Loki server is `http://loki:3100`. We can then click on the `Save & Test`
button to test the connection to the Loki server.

Once we have our data sources configured, grafana is now able to query the data
collected by Prometheus and Loki.
