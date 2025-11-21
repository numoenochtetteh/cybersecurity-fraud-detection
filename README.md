# Cybersecurity & Fraud Detection Analysis using UNSW-NB15 Dataset

## Project Overview
Cyberattacks and digital fraud continue to increase, posing serious risks to businesses and individuals. This project analyzes network traffic data using the **UNSW-NB15 dataset** to detect anomalous behavior and potential cyberattacks. The goal is to provide actionable insights to cybersecurity teams and highlight suspicious activity in network traffic.

---

## Problem Statement
- Cyberattacks and digital fraud are becoming more frequent and sophisticated.  
- Organizations need **early warning systems** to identify high-risk activities in real-time.  
- Manual monitoring is inefficient due to the large volume of network traffic.  

---

## Solution / What This Project Achieves
- Analyzed network traffic logs to identify unusual patterns.  
- Built visualizations to understand attack distribution by type, protocol, hour, and source IP.  
- Implemented **anomaly detection** using Isolation Forest to automatically flag suspicious traffic.  
- Helped prioritize high-risk areas for cybersecurity monitoring using **data-driven insights**.  

---

## Dataset
- **Name:** Custom version of UNSW-NB15  
- **Rows:** 5,000 sample entries  
- **Columns include:**  
  - `src_ip`, `dst_ip` — Source and destination IP addresses  
  - `src_port`, `dst_port` — Source and destination ports  
  - `protocol` — Network protocol (TCP, UDP, ICMP)  
  - `packet_size` — Size of the packet in bytes  
  - `timestamp` — Time of the network traffic  
  - `attack_type` — Type of traffic/attack  
  - `label` — 0 = Normal, 1 = Attack  

---

## Tools & Libraries Used
- **Python 3** — Main programming language  
- **Jupyter / Google Colab** — Notebook environment  
- **Pandas & NumPy** — Data manipulation and analysis  
- **Matplotlib & Seaborn** — Visualization of trends and patterns  
- **Scikit-Learn** — Machine learning for anomaly detection  

---

## Steps Taken

1. **Data Cleaning & Feature Engineering**
   - Converted `timestamp` to datetime format  
   - Created additional features: `hour` and `day`  

2. **Exploratory Data Analysis (EDA)**
   - Analyzed distribution of normal vs attack traffic  
   - Explored attack types, traffic by hour, and protocols  

3. **Visualization**
   - Count plots for normal vs suspicious traffic  
   - Bar charts for top attack types and source IPs  
   - Hourly traffic trends and protocol usage  

4. **Anomaly Detection**
   - Applied Isolation Forest to detect suspicious network activity  
   - Flagged anomalies for further investigation  

5. **Insights**
   - Most attacks occur during specific hours of the day  
   - Certain protocols (TCP/UDP) are more frequently targeted  
   - Top source IPs triggering anomalies identified  

---

## How to Run

1. Clone this repository:
   ```bash
   git clone https://github.com/YourUsername/cybersecurity-fraud-detection.git

