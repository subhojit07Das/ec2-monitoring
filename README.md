# EC2 Monitoring Stack

Prometheus + Grafana + Node Exporter running on AWS EC2.

## Stack
- **Node Exporter** — collects CPU, RAM, disk metrics from the host
- **Prometheus** — scrapes and stores those metrics
- **Grafana** — visualizes everything with dashboards

## Ports
| Service       | Port |
|---------------|------|
| Grafana       | 3000 |
| Prometheus    | 9090 |
| Node Exporter | 9100 |

## Run
```
docker compose up -d
```

## Access
- Grafana: http://<your-ec2-ip>:3000 (admin / admin123)
- Prometheus: http://<your-ec2-ip>:9090