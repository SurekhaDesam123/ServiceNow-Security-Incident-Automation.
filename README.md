
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
### 📊 System Dashboard
![Security Dashboard](image_338b65.png)

### ⚙️ Automation Logic (Flow Designer)
![Workflow Logic](Surekha_Security_Routing (1).png)
<h3 align="center">Security Command Center</h3>
<p align="center">
  <img src="image_338b65.png" width="800" title="Management Dashboard">
</p>

<h3 align="center">Flow Automation Logic</h3>
<p align="center">
  <img src="Surekha_Security_Routing (1).png" width="600" title="ServiceNow Flow Designer">
</p>
