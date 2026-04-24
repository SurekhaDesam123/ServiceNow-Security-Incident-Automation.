
# Security Incident Routing & Automation (ServiceNow)

## 📌 Project Overview
A custom ServiceNow application designed to automate the lifecycle of security incidents. The system handles ingestion, intelligent routing, SLA-based escalations, and management reporting.

## ⚙️ Technical Implementation

### 1. Data Modeling
* Created a custom table `u_surekha_security_incident` extending from the Task architecture.
* Implemented an auto-numbering system (`SEC0001000`).
* Configured choice lists for Categories (Phishing, Malware, Unauthorized Access).

### 2. Workflow Automation (Flow Designer)
* **Conditional Routing:** Developed logic to auto-assign incidents to specific analysts based on the threat category.
* **SLA Escalation:** Built a 2-minute "Wait" timer that checks the record status.
* **Automated Updates:** If the record remains "Not Resolved," the flow automatically upgrades the Severity to **Critical** and appends "[OVERDUE]" to the short description.

### 3. Analytics & Visualization
* Developed a **Platform Analytics Dashboard** featuring:
    * Pie charts for incident distribution.
    * Bar charts for workload balancing.
    * Real-time list monitoring for Critical incidents.

## 📸 Visuals

### 📊 Management Command Center
![Dashboard](Screenshot%202026-04-23%20185640.png)

### ⚙️ Automation Logic (Flow Designer)
![Flow Diagram](Surekha_Security_Routing%20\(1\).png)

