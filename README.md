# Monitoring Stack 🚀

[![Docker](https://img.shields.io/badge/Docker-24.0.1-blue?logo=docker)](https://www.docker.com/)
[![Prometheus](https://img.shields.io/badge/Prometheus-2.50.0-orange?logo=prometheus)](https://prometheus.io/)
[![Grafana](https://img.shields.io/badge/Grafana-10.3.0-red?logo=grafana)](https://grafana.com/)
[![Loki](https://img.shields.io/badge/Loki-2.9.0-lightgrey?logo=loki)](https://grafana.com/oss/loki/)
[![Alertmanager](https://img.shields.io/badge/Alertmanager-0.25.0-yellowgreen?logo=prometheus)](https://prometheus.io/docs/alerting/alertmanager/)

A complete monitoring stack for metrics, logs, and alerts using **Prometheus**, **Grafana**, **Loki**, **Promtail**, and **Alertmanager**.

---

## 🛠 Services Included

- **Prometheus** → Metrics collection  
- **Grafana** → Dashboards and visualization  
- **Loki** → Centralized log aggregation  
- **Promtail** → Log collection agent  
- **Alertmanager** → Alert notifications  
- **Alert Rules** → CPU, memory, disk, and custom alerts  

---

## 🚀 Quick Setup

1. Clone repository:

```bash
git clone git@github.com:yourusername/monitoring-stack.git
cd monitoring-stack
Edit configurations (replace placeholders):

docker-compose.yml → domains, SMTP credentials

prometheus/prometheus.yml → target servers

loki/local-config.yaml → storage paths

promtail/promtail-config.yml → log paths

Start services:

bash
Copy code
docker-compose up -d
Access services:

Grafana → http://localhost:13000 (admin/admin)

Prometheus → http://localhost:19090

Alertmanager → http://localhost:19093

📂 Repository Structure
arduino
Copy code
monitoring-stack/
├── docker-compose.yml
├── prometheus/
│   └── prometheus.yml
├── alertmanager/
│   └── alertmanager.yml
├── rules/
│   └── alert.rules.yml
├── grafana/
│   └── dashboards/
├── loki/
│   └── local-config.yaml
├── promtail/
│   └── promtail-config.yml
└── README.md
⚙ Features
Real-time metrics and log monitoring

4xx/5xx HTTP logs visualization

System resource alerts (CPU, memory, disk)

Email notifications via Alertmanager

Ready-to-use Grafana dashboards

📧 Maintainer
Name: Your Name

Email: youremail@example.com
