# 🛡️ Microsoft Sentinel SOC Automation Lab

This project demonstrates a functional **Cloud SIEM/SOAR** setup using **Microsoft Sentinel**. The goal was to detect SSH Brute Force attacks on a Linux VM and automate the incident response workflow using **Azure Logic Apps**.

---

## 🎨 Workflow Visualization
Below is the architectural flow of the automated response system I built. It shows how Sentinel triggers the Logic App to send real-time email notifications.

![Automation Visual Summary](Automate/2.png)


---

## 🚀 Project Overview
I implemented an end-to-end security monitoring solution in Azure to:
1. **Ingest Logs:** Connected a Linux VM to a Log Analytics Workspace.
2. **Detect Threats:** Created a custom Analytics Rule to flag Brute Force attempts.
3. **Automate Response:** Developed a Playbook to notify the security team via email.

---

## 🛠️ Tech Stack & Skills
- **SIEM:** Microsoft Sentinel
- **SOAR (Automation):** Azure Logic Apps (Playbooks)
- **Monitoring:** Log Analytics Workspace
- **Language:** Kusto Query Language (KQL)
- **Target:** Azure Linux Virtual Machine
- **Attack Tool:** Kali Linux (Hydra)

---

## 📊 Lab Execution & Evidence

### 1. Incident Detection
After simulating the attack from Kali Linux, Microsoft Sentinel successfully identified and created a medium-severity incident.

**Live Evidence: Sentinel Incident Dashboard**
![Sentinel Incident](Automate/incident.png)

### 2. Automated Notification
Upon incident creation, the automation rule triggered the email playbook, sending a real-time alert to my inbox.

**Live Evidence: Email Alert Received**
![Email Alert](Automate/output.png)

---

## 🧠 Key Learnings
- Deploying and managing **Microsoft Sentinel** in a cloud environment.
- Writing **KQL** queries for threat detection.
- Building **SOAR** workflows to automate repetitive security tasks.
- Reducing Mean Time to Respond (MTTR) through automation.

---
**Project completed by Amal** | [LinkedIn](https://www.linkedin.com/in/amal-udayanga-basnayake/)
