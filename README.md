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

## 📦 Installation (macOS & Ubuntu)

You can install Soroban-ELK by downloading the appropriate installer script from the latest release.

### 🔗 Download

Go to the [release page](https://github.com/bytemaster333/Soroban-ELK/releases/tag/release-v1.0) and download the installation script that matches your system:

- [Download for macOS](https://github.com/bytemaster333/Soroban-ELK/releases/download/release-v1.0/MACOS_install.sh)
- [Download for Ubuntu](https://github.com/bytemaster333/Soroban-ELK/releases/download/release-v1.0/UBUNTU_install.sh)

---

### 🛠 Installation Steps

#### macOS
```bash
curl -LO https://github.com/bytemaster333/Soroban-ELK/releases/download/release-v1.0/MACOS_install.sh
chmod +x MACOS_install.sh
./MACOS_install.sh
```

#### Linux
```bash
curl -LO https://github.com/bytemaster333/Soroban-ELK/releases/download/release-v1.0/UBUNTU_install.sh
chmod +x UBUNTU_install.sh
./UBUNTU_install.sh
```

## 📊 GitHub Release Stats

📥 Track SCI download stats here:  
[https://tooomm.github.io/github-release-stats/?username=bytemaster333&repository=Soroban-ELK](https://tooomm.github.io/github-release-stats/?username=bytemaster333&repository=Soroban-ELK)

---

## 📬 Contact & Community

- 💬 Discuss the project on [Stellar Discord](https://discord.gg/stellar)
- 📫 Reach out via GitHub Issues or email: `salih@sci.dev` (example)

---

## 📜 License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.

---

> Created with ❤️ for the Stellar Developer Community
