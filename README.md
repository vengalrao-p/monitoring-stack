 README.md
markdown
Copy
Edit
# Monitoring Stack with Grafana, Prometheus, Loki, and InfluxDB

This project sets up a full DevOps monitoring stack using Docker Compose. It includes:

- **Prometheus** – for scraping and storing metrics
- **Grafana** – for visualizing metrics and logs
- **Loki** – for collecting and querying logs
- **InfluxDB** – a time-series database for storing custom metrics

> 📦 All services run as Docker containers for easy setup and deployment.

---

## 📁 Project Structure

monitoring-stack/
├── docker-compose.yml
└── prometheus/
└── prometheus.yml

yaml
Copy
Edit

---

## 🚀 Getting Started

### Prerequisites

- [Docker](https://www.docker.com/)
- [Docker Compose](https://docs.docker.com/compose/)

### Run the stack

```bash
git clone https://github.com/your-username/monitoring-stack.git
cd monitoring-stack
docker-compose up -d
🌐 Access Services
Service	URL	Default Port
Grafana	http://localhost:3000	3000
Prometheus	http://localhost:9090	9090
Loki	http://localhost:3100	3100
InfluxDB	http://localhost:8086	8086

🔐 Grafana login: admin / admin (you'll be prompted to change password on first login)

📊 Configure Grafana
Add Prometheus as a data source:

URL: http://prometheus:9090

Add Loki as a data source:

URL: http://loki:3100

Add InfluxDB as a data source:

URL: http://influxdb:8086

Auth: Disabled (unless configured)

Database: Create manually or configure later





👨‍💻 Author
Vengalarao Pasala
GitHub | Email: vengaldevops7@gmail.com

