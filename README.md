# Hi, I'm Konstantina 👋

**Junior software engineer** (BSc Computer Science) building backend systems, data/ML pipelines and
security tooling, with tests, CI and the reasoning written down.

- 🛠️ **Core stack:** TypeScript · Node.js / Express · Python · PostgreSQL · React / Next.js · Docker · GitHub Actions
- 🔍 **Also comfortable with:** Kafka · Spark · scikit-learn / XGBoost · Redis · Laravel · Suricata / Wazuh · Modbus/TCP


[Portfolio](https://kgiannopoulou.github.io/website-portfolio/) ·
[LinkedIn](https://www.linkedin.com/in/konstantina-giannopoulou-464668281) ·
[CV (PDF)](https://github.com/user-attachments/files/33810795/myCV.pdf) .


---

## ⭐ Featured projects

| Project | What it is | Evidence |
|---|---|---|
| **[Fireline — Incident Response Platform](https://github.com/kgiannopoulou/incident-response-platform)** *(flagship)* | PagerDuty-style platform: alert ingestion and deduplication, an incident state machine, escalations, real-time updates over SSE, and an AI investigator that cites its evidence | 367 tests · 93% coverage · ~340 alerts/s per process · threat model · v1.0.0 |
| **[Real-Time Fraud Detection](https://github.com/kgiannopoulou/real-time-fraud-detection-platform)** | Kafka → Spark Structured Streaming → XGBoost from an MLflow registry, with SHAP explanations, Airflow retraining and drift monitoring | PR-AUC 0.795 · ~450 tx/s on a laptop · p95 4.2 s · 13-service `docker compose up` |
| **[OT/ICS Cybersecurity Lab](https://github.com/kgiannopoulou/ot-ics-cybersecurity-lab)** | Simulated PLC water-tank process over Modbus/TCP, IT/DMZ/OT zones, Suricata + Wazuh detections, and red/blue validation | 13 allow-list IDS rules · 0 false positives on the baseline · IEC 62443 / ATT&CK for ICS |
| **[IoT Security Monitor](https://github.com/kgiannopoulou/iot-security-monitor)** | Passive IoT/OT network monitor: device inventory, per-device baselines, MQTT/Modbus decoding, SOC triage dashboard | 163 tests · ATT&CK mapping · ECS/CEF/syslog SIEM output |
| **[Full-Stack E-Commerce](https://github.com/kgiannopoulou/fullstack-ecommerce)** | Next.js + Express/TypeScript + PostgreSQL + Stripe. Stock can't be oversold, and a payment can't be processed twice | 62 race/replay tests against real Postgres · CI · Docker |
| **[Road Network Simulator](https://github.com/kgiannopoulou/road-network-simulator)** | City traffic and self-driving-car lab in plain JS: physics, sensors, a neural network + genetic algorithm, A* routing | [▶ Live demo](https://kgiannopoulou.github.io/road-network-simulator/) · 180 tests · zero dependencies |

## 🧭 Pick a path

<table>
<tr>
<th>💻 Software Engineering</th>
<th>📊 Data &amp; AI</th>
<th>🛡️ Cybersecurity</th>
</tr>
<tr valign="top">
<td>

**[Fireline](https://github.com/kgiannopoulou/incident-response-platform)**: concurrency-safe dedup, Postgres triggers, BullMQ workers, SSE, OpenAPI

**[E-Commerce](https://github.com/kgiannopoulou/fullstack-ecommerce)**: transactional stock reservation, idempotent Stripe webhooks

**[Home Helper API](https://github.com/kgiannopoulou/home-helper-api)**: Laravel/MySQL sync API, 294 tests, OpenAPI, ER diagrams

</td>
<td>

**[Fraud Detection](https://github.com/kgiannopoulou/real-time-fraud-detection-platform)**: streaming features, model comparison on PR-AUC, MLflow, drift (PSI)

**[Road Network Simulator](https://github.com/kgiannopoulou/road-network-simulator)**: neural network and genetic algorithm written from scratch, reproducible training

**[Personal Home Helper](https://github.com/kgiannopoulou/personal-home-helper)**: React Native app with an AI hub (Claude API) and on-device predictions

</td>
<td>

**[OT/ICS Lab](https://github.com/kgiannopoulou/ot-ics-cybersecurity-lab)**: segmentation, Modbus detection, attack → detect → block validation

**[IoT Security Monitor](https://github.com/kgiannopoulou/iot-security-monitor)**: passive detection engine, baselines, SOC analyst view

**[Smart Factory Threat Assessment](https://github.com/kgiannopoulou/smart-factory-threat-assessment)**: STRIDE threat model and OT risk assessment

Also: [websec-scanner](https://github.com/kgiannopoulou/websec-scanner) · [PortSwigger write-ups](https://github.com/kgiannopoulou/PortSwigger-Web-Security-Academy)

</td>
</tr>
</table>

## 📝 Technical write-ups

- **[Alert deduplication under concurrency](https://github.com/kgiannopoulou/incident-response-platform#deduplication-strategy)**: why "one open incident per key" is a unique index, not application logic, and the bug a load test found
- **[Event time in a real-time fraud pipeline](https://github.com/kgiannopoulou/real-time-fraud-detection-platform/blob/main/docs/event-time.md)**: watermarks, late events and avoiding train/serve skew with Kafka and Spark
- **[Threat-modelling an industrial water-tank process](https://github.com/kgiannopoulou/ot-ics-cybersecurity-lab/blob/main/docs/threat-model.md)**: Modbus has no authentication, so what actually protects the process?
- **[Design decisions for a passive IoT monitor](https://github.com/kgiannopoulou/iot-security-monitor/blob/main/docs/design-decisions.md)**: per-device baselines, MAC keys, and why it never sends a packet

## 🔧 How I work

Every serious project here has automated tests and CI. Each README covers the architecture, the design
decisions and trade-offs, failure scenarios, and honest limitations. Simulated data is labelled as
simulated, and benchmarks say what machine they ran on. Right now I'm going deeper on existing systems
(load tests, observability, deployment) rather than starting new ones.

<sub>Smaller and older experiments (Java games, early web projects) are archived. They're still public, just not the focus.</sub>
