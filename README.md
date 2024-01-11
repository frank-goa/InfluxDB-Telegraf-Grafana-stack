
![Logo](https://user-images.githubusercontent.com/64506580/159311466-f720a877-6c76-403a-904d-134addbd6a86.png)


# Telegraf, InfluxDB, Grafana (TIG) Stack

Gain the ability to analyze and monitor telemetry data by deploying the TIG stack within minutes using [Docker](https://docs.docker.com/engine/install/) and [Docker Compose](https://docs.docker.com/compose/install/).




## ⚡️ Getting Started


Change the environment variables define in `.env` that are used to setup and deploy the stack
```bash
├── telegraf/
├── .env         <---
├── docker-compose.yml
├── entrypoint.sh
└── ...
```

Customize the `telegraf.conf` file which will be mounted to the container as a persistent volume

```bash
├── telegraf/
│   ├── telegraf.conf <---
├── .env
├── docker-compose.yml
├── entrypoint.sh
└── ...
```

Start the services
```bash
docker-compose up -d
```
<img width="1386" alt="Screenshot 2024-01-11 at 22 31 33" src="https://github.com/frank-goa/InfluxDB-Telegraf-Grafana-stack/assets/137857643/d5c6ae64-a47b-4f2b-951c-592ee7e321f7">

<img width="1398" alt="Screenshot 2024-01-11 at 22 33 43" src="https://github.com/frank-goa/InfluxDB-Telegraf-Grafana-stack/assets/137857643/08137484-2d61-4def-a0da-ab068a86f254">

<img width="1509" alt="Screenshot 2024-01-11 at 22 34 44" src="https://github.com/frank-goa/InfluxDB-Telegraf-Grafana-stack/assets/137857643/a1f3edb2-b8b9-40f6-992c-0c814eb200c9">

<img width="1403" alt="Screenshot 2024-01-11 at 22 36 41" src="https://github.com/frank-goa/InfluxDB-Telegraf-Grafana-stack/assets/137857643/378d2722-9dc6-4bd9-92fc-30005b0609fc">

<img width="1506" alt="Screenshot 2024-01-11 at 22 39 26" src="https://github.com/frank-goa/InfluxDB-Telegraf-Grafana-stack/assets/137857643/1a8d07a6-882f-4c9b-b8b4-2fb66e1c708d">

<img width="1487" alt="Screenshot 2024-01-11 at 22 41 53" src="https://github.com/frank-goa/InfluxDB-Telegraf-Grafana-stack/assets/137857643/a0b5188a-21af-4f93-985d-289a31978ea3">

<img width="1496" alt="Screenshot 2024-01-11 at 22 43 33" src="https://github.com/frank-goa/InfluxDB-Telegraf-Grafana-stack/assets/137857643/e87499bd-0338-467d-b3f0-af09a3265e50">

<img width="1498" alt="Screenshot 2024-01-11 at 22 44 38" src="https://github.com/frank-goa/InfluxDB-Telegraf-Grafana-stack/assets/137857643/5a1ac66c-459b-49d4-a774-91a4d0bd4bc6">

<img width="1492" alt="Screenshot 2024-01-11 at 22 46 23" src="https://github.com/frank-goa/InfluxDB-Telegraf-Grafana-stack/assets/137857643/c3a55a16-0ef9-48eb-8031-b200bc1413ba">

<img width="1493" alt="Screenshot 2024-01-11 at 22 47 44" src="https://github.com/frank-goa/InfluxDB-Telegraf-Grafana-stack/assets/137857643/77f81eda-3e0c-46f3-b296-4cf2024f0b8d">

<img width="1501" alt="Screenshot 2024-01-11 at 22 51 42" src="https://github.com/frank-goa/InfluxDB-Telegraf-Grafana-stack/assets/137857643/7dec8343-ddc5-4205-ab0c-0447c2ea0763">


## Docker Images Used (Official & Verified)

[**Telegraf**](https://hub.docker.com/_/telegraf) / `1.19`

[**InfluxDB**](https://hub.docker.com/_/influxdb) / `2.1.1`

[**Grafana-OSS**](https://hub.docker.com/r/grafana/grafana-oss) / `8.4.3`

### Important links
- https://docs.influxdata.com/influxdb/v2/reference/cli/influx/setup/
- https://grafana.com/grafana/dashboards/
- https://docs.influxdata.com/telegraf/v1/
