# Access Provisioning Automation & Centralized Log Correlation
### Security Engineering & SOC Case Study

This project demonstrates a complete security workflow combining **IAM automation**,  
**multi-OS log integration**, and **SIEM correlation logic** designed to improve  
visibility, auditability, and incident detection across a corporate environment.

The solution integrates **Google Workspace**, **Slack**, **Wazuh SIEM**, and a  
Python-based automated access workflow compliant with least-privilege and audit requirements.

---

## 🔐 1. Automated Access Provisioning Workflow

The proposed access workflow ensures:

- Manager approval (Slack or email)
- Automated provisioning via API (Python)
- Temporary access expiration
- Audit logging of every action (timestamp, approver, system, expiration)
- Full integration with the SIEM

Technologies involved:
- Python
- Google Workspace Admin SDK
- Slack Audit Logs API
- Wazuh SIEM ingestion
- AWS backend execution (serverless)

---

## 📊 2. Centralized Log Integration (Google Workspace + Slack)

### Google Workspace
- Admin Activity, Login Audit, Drive logs  
- Collected via Reports API (JSON)  
- OAuth-secured, TLS 1.2+  
- Normalized into Wazuh

### Slack
- Audit Logs API + Event Subscriptions  
- Real-time ingestion via webhook  
- Signed request validation (HMAC)

---

## ⚠️ 3. Correlation Rule: Account Takeover Detection

The SIEM rule identifies suspicious cross-system behavior:


Goal:
- Detect compromised accounts  
- Trigger automated SOC alerts  
- Reduce MTTR  

---

## 💻 4. Asset Management & Inventory Automation

Tools included:
- JumpCloud MDM
- Wazuh SIEM
- Jira Assets CMDB

Automations:
- Daily sync between SIEM → CMDB
- Unknown device detection
- Stale device detection (>30 days)
- Automated offboarding workflow

---

## 📄 5. Project Files

- **SIEM-report.pdf** → Full architecture documentation   

---

## 🏷️ Tags / Keywords
`Security Engineering`, `SOC`, `SIEM`, `Wazuh`, `Google Workspace`,  
`Slack Audit Logs`, `IAM`, `Automation`, `Python`, `Incident Detection`,  
`Access Provisioning`, `Log Correlation`, `MDM`, `JumpCloud`, `CMDB`,  
`Cybersecurity`, `Case Study`

---

## 👩‍💻 Author
**Nathalia Bertol**  
Cybersecurity Specialist — AppSec, SOC, Automation  
