# SOC Lab: ELK Stack Log Monitoring & Threat Detection

##  Overview
This project demonstrates a basic Security Operations Center (SOC) lab using the ELK Stack (Elasticsearch, Kibana, Filebeat) to monitor and detect suspicious activities on a Linux system.

---

##  Architecture
Filebeat → Elasticsearch → Kibana

- Filebeat collects logs from `/var/log`
- Elasticsearch stores and indexes logs
- Kibana visualizes and analyzes logs

---

##  Technologies Used
- Elasticsearch
- Kibana
- Filebeat
- Ubuntu Server

---

##  Setup Summary
1. Installed Elasticsearch and enabled security
2. Installed Kibana and connected to Elasticsearch
3. Installed Filebeat and configured log ingestion
4. Loaded dashboards into Kibana
5. Verified logs in Discover

---

##  Log Monitoring
Logs were collected from:
- `/var/log/auth.log`
- `/var/log/syslog`

---

## Simulated Attacks

### 1. Failed SSH Login (Brute Force Simulation)
```bash
ssh fakeuser@localhost
