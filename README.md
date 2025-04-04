# 🌠 Stellar Command Insights (SCI)

**Stellar Command Insights (SCI)** is a real-time monitoring, visualization, and alerting system designed to help Stellar developers, system administrators, and blockchain enthusiasts gain deep insights into **Stellar CLI and RPC command executions**.

Built on the powerful **ELK Stack (Elasticsearch, Logstash, Kibana)**, SCI provides a user-friendly platform to capture, analyze, and visualize command data—bringing transparency, observability, and operational intelligence to Stellar-based development.

---

## 🚀 Features

- ⚙️ **Real-Time CLI & RPC Monitoring**  
  Capture and analyze both `soroban` CLI and Stellar RPC command outputs as they happen.

- 📊 **Interactive Dashboards**  
  Visualize command activity, transaction execution, and errors with Kibana dashboards.

- 🔔 **Real-Time Alerts via Telegram & Slack**  
  Receive immediate notifications for command failures, anomalies, or custom conditions.

- 📁 **Historical Log Tracking**  
  Store and search past command executions to streamline debugging and performance reviews.

- 🧠 **Extensible & Open Source**  
  Easily configurable and extendable for your custom Stellar workflow and infrastructure.

---

## 🧱 Architecture Overview

SCI is composed of the following components:

- **CLI & RPC Logger** – Captures `soroban` CLI and RPC command executions and logs them to `stellar.log`.
- **Filebeat** – Monitors the log file and forwards new entries to Logstash.
- **Logstash** – Parses and structures the logs before sending them to Elasticsearch.
- **Elasticsearch** – Indexes and stores log data for querying and analysis.
- **Kibana** – Provides a visual interface for dashboards, filtering, and reporting.
- **Alerting System** – Sends configurable alerts through Telegram or Slack.

---

## 📦 Installation

> SCI supports Linux/macOS and can be deployed with a single script (coming soon!).

```bash
# 1. Clone the repository:
git clone https://github.com/bytemaster333/Soroban-ELK.git
cd Soroban-ELK

# 2. Run the setup script:
./install.sh

# 3. Start using SCI:
# - Open Kibana on http://localhost:5601
# - Monitor CLI & RPC command logs in real time
# - Set up alerts under the "Alert Manager" dashboard
```

> ℹ️ Detailed installation instructions will be added soon.

---

## 📈 Demo & Screenshots

_🚧 Coming Soon: Live demo and dashboard examples_

---

## 📊 GitHub Release Stats

📥 Track SCI download stats here:  
[https://tooomm.github.io/github-release-stats/?username=bytemaster333&repository=Soroban-ELK](https://tooomm.github.io/github-release-stats/?username=bytemaster333&repository=Soroban-ELK)

---

## 🤝 Contributing

We welcome contributions! If you'd like to improve the CLI logger, expand RPC coverage, or enhance dashboard visualizations:

```bash
# 1. Fork the repo
# 2. Create your feature branch:
git checkout -b feature/new-feature

# 3. Commit your changes:
git commit -m 'Add new feature'

# 4. Push to the branch:
git push origin feature/new-feature

# 5. Submit a pull request
```

---

## 📬 Contact & Community

- 💬 Discuss the project on [Stellar Discord](https://discord.gg/stellar)
- 📫 Reach out via GitHub Issues or email: `salih@sci.dev` (example)

---

## 📜 License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.

---

> Created with ❤️ for the Stellar Developer Community
