# azure-threat-detection

# Azure Sentinel Brute Force Detection Lab

## Overview
This project demonstrates the implementation of a **cloud-based SIEM solution** using **Microsoft Sentinel** to detect and respond to brute force login attacks on a Windows virtual machine hosted in Azure.

The lab simulates a real-world attack scenario by generating multiple failed login attempts, detecting them using **Event ID 4625**, and triggering automated alerts and email notifications.

---

## Technologies Used
- Microsoft Azure
- Microsoft Sentinel (SIEM)
- Log Analytics Workspace
- Windows Virtual Machine
- KQL (Kusto Query Language)
- Azure Logic Apps
- Email Alerting

---

## Lab Architecture
1. Windows VM generates security logs
2. Logs are forwarded to Log Analytics
3. Microsoft Sentinel analyzes events
4. High-severity alert is triggered
5. Automated email notification is sent

---

## Detection Logic
The brute force attack was detected using **Event ID 4625**, which represents failed login attempts on Windows systems.

**Key Indicators:**
- Multiple failed logins from the same source
- High frequency of authentication failures
- Triggered high-severity Sentinel alert

---

## Evidence of Detection
Screenshots included in this repository show:
- Event ID 4625 logs in Sentinel
- High severity brute force alert
- Automated email alert sent upon detection

---

## Incident Response
When the alert condition was met:
- Microsoft Sentinel classified the activity as **High Severity**
- A Logic App workflow automatically sent an email alert
- The incident was logged for further investigation

---

## Skills Demonstrated
- SIEM deployment and configuration
- Cloud security monitoring
- KQL query creation
- Incident detection and response
- Azure security services
- Threat analysis and alert automation

---

## 📎 Disclaimer
This lab was conducted in a controlled environment for educational purposes only.
