# AI-Powered SOC Lab

**Detect threats in network and cloud environments using AI/ML with alerts, MITRE ATT&CK mapping, and interactive dashboards.**

## Project Description

This project is a **simulated Security Operations Center (SOC) lab** that uses Python, ML, and data visualization to detect and prioritize threats in network logs. It provides:

- Automated **data ingestion and cleaning**
- **Feature engineering** for ML models
- **Machine learning threat detection** (supervised + unsupervised)
- **Alert generation with severity levels**
- **MITRE ATT&CK tactic mapping**
- **Interactive dashboards** for monitoring and reporting

The project is fully runnable in **Google Colab** and includes a synthetic dataset for demonstration purposes.

## Project Features

1. **Data Ingestion & Cleaning**
   - Loads network logs
   - Normalizes columns (timestamp, source/destination IPs, protocol, action)
   - Maps threat severity
   - Handles missing or inconsistent data

2. **Feature Engineering**
   - Extracts time-based features (hour of day)
   - Creates protocol flags (`TCP`, `UDP`)
   - Calculates source and destination IP counts
   - Adds security-related flags (e.g., failed login attempts)

3. **ML-Based Threat Detection**
   - **Supervised ML**: Random Forest Classifier for known attacks
   - **Unsupervised ML**: Isolation Forest for anomaly detection
   - Combines results for accurate threat detection

4. **Alerts & MITRE Mapping**
   - Generates alerts with severity levels (`Low`, `Medium`, `High`, `Critical`)
   - Maps alerts to **MITRE ATT&CK tactics**
   - Prioritizes the most critical threats for SOC analysts

5. **Interactive Dashboard**
   - Visualizes alerts by severity
   - Pie charts for MITRE ATT&CK categories
   - Top source IPs generating alerts
   - Built with **Plotly** for interactivity

## Installation

Clone this repository:

```bash
git clone https://github.com/ThreatAnalyzer/AI-SOC-Lab.git
cd AI-SOC-Lab

pip install -r requirements.txt




