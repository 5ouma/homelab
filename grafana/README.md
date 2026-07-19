<!-- name: 🟠 Grafana -->
<h1 align="center"><a href="https://grafana.com">Grafana</a></h1>

<div align="center">

**🟠 OpenTelemetry Collector distribution with programmable pipelines**

</div>

<br /><br />

## 🔧 Setup

1. 🏔️ Copy the [`.env.tmpl`](./.env.tmpl) file to `.env` and Edit it

   |          Name           |         Value         |
   | :---------------------: | :-------------------: |
   | `GRAFANA_CLOUD_API_KEY` | Grafana Cloud API Key |
   |    `PROMETHEUS_URL`     |    Prometheus URL     |
   |  `PROMETHEUS_USERNAME`  |  Prometheus Username  |
   |       `LOKI_URL`        |       Loki URL        |
   |     `LOKI_USERNAME`     |     Loki Username     |

2. 🚀 Start the Docker Compose

   ```sh
   docker compose up -d
   ```
