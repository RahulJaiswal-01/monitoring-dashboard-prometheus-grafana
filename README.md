# 🖥 Real-Time Server Monitoring Dashboard (Prometheus + Grafana + Alertmanager)

This project implements a real-time monitoring and alerting system to track server performance metrics such as CPU, memory, disk, and network usage. It uses:

- **Prometheus** – metrics collection & time-series database  
- **Node Exporter** – host metrics (CPU, RAM, disk, network)  
- **Grafana** – interactive dashboards  
- **Alertmanager** – alert routing  
- **Slack** – notifications for high CPU / memory / node down  

---

## 🚀 Tech Stack

- RHEL Linux (VM)
- Docker & Docker Compose  
- Prometheus  
- Node Exporter  
- Grafana  
- Alertmanager  
- Slack Incoming Webhook (local, not committed)

---

## ⚙️ How to Run

```bash
git clone https://github.com/<your-username>/monitoring-dashboard-prometheus-grafana.git
cd monitoring-dashboard-prometheus-grafana
docker-compose up -d
Then open:

Prometheus: http://localhost:9090

Grafana: http://localhost:3000

Alertmanager: http://localhost:9093

📊 Grafana Dashboard

Import community dashboard ID:

1860


This shows CPU, memory, disk, and network usage visually.

🚨 Alerts

Prometheus is configured with alert rules, such as:

High CPU usage > 80%

High memory usage > 80%

Node Exporter down

Alerts are routed to Alertmanager, which sends notifications to Slack (configured locally via alertmanager.yml with your own webhook URL).

🔮 Future Enhancements

Container monitoring (cAdvisor)

Kubernetes cluster monitoring

Multi-channel alerting (Email / Telegram / Discord)

👨‍💻 Author

RJ
DevOps & Monitoring Enthusiast
