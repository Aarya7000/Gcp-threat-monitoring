# 🔐 GCP Threat Monitoring and Incident Response System

This project demonstrates how to build a real-time cybersecurity alert system using Google Cloud.

---

## 🧠 What It Does
- Detects `ERROR` logs in GCP
- Triggers an alert via Cloud Logging
- Sends a POST request to a deployed Cloud Function
- Logs the event and simulates a response

---

## 🛠️ Tools Used
- Google Cloud Functions (2nd Gen)
- Cloud Logging
- Alert Policies
- IAM
- Python + Flask

---

📂 Files Included

| File | Description |
|------|-------------|
| `main.py` | The cloud function triggered via webhook |
| `requirements.txt` | Flask dependency for cloud function |
| `README.md` | Documentation |
| `screenshots/` | Folder with deployment & test screenshots |


 💡 Skills Gained

- Cloud automation using Google Cloud
- Real-time log-based threat monitoring
- IAM & Cloud Function deployments
- Webhook-based incident response
- Basic DevOps + Python integration

 📸 Screenshots

✅ 1. Cloud Function Deployed
![Function Deployed](screenshots/function-deployed.png)

✅ 2. Cloud Shell Deployment
![Shell Deploy](screenshots/cloud-shell-deploy.png)

✅ 3. Threat Logged Response
![Threat Log](screenshots/threat-logged-response.png)

✅ 4. Alert Policy
![Alert Policy](screenshots/alert-policy.png)

---
 🧪 Test Function via curl:

```bash
curl -X POST https://logthreatresponse-XXXXXX.a.run.app -H "Content-Type: application/json" -d '{"threat":"simulated"}'
