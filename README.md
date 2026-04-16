# 🛡️ API Security Risk Analysis

**🎯 API Tested:** [ReqRes Demo API](https://reqres.in)  

---

## 🛠️ Tools Used
* **Postman** (Web Version)
* **Browser DevTools**

## 🔎 Scope & Ethics
> **Note:** This assessment was restricted to read-only testing of public demo API endpoints. No exploitation, destructive testing, or access to private/production APIs occurred during this analysis.

## 📝 Methodology
1. **Documentation Review:** Analyzed standard API documentation to understand expected endpoint behaviors.
2. **Endpoint Testing:** Executed safe GET/POST requests via Postman.
3. **Traffic Inspection:** Evaluated authentication mechanisms, response payloads, and HTTP headers.
4. **Risk Identification:** Classified security risks based on standard Application Security (AppSec) principles.
5. **Reporting:** Documented findings and proposed actionable remediation steps.

## ⚠️ Risks Identified

| Risk ID | Vulnerability Description | Severity |
| :--- | :--- | :--- |
| **RISK-001** | Unauthenticated Access to Users | 🔴 **HIGH** |
| **RISK-002** | User PII Exposed Without Login | 🔴 **HIGH** |
| **RISK-003** | Missing Security Headers | 🟡 **MEDIUM** |
| **RISK-004** | Inconsistent Auth Model | 🟡 **MEDIUM** |
| **RISK-006** | Missing Rate Limiting | 🟡 **MEDIUM** |
| **RISK-005** | Excessive Data Exposure | 🟢 **LOW** |

> *Self-Correction Note for Report:* Make sure your final `.docx` report explains the context for **RISK-001** and **RISK-002**. In the screenshot you captured earlier, the API successfully blocked access with a `401 Unauthorized` error. If you found another endpoint that *did* allow unauthenticated access, make sure your screenshots clearly highlight that specific endpoint!

## 📂 Repository Contents
* 📄 `API_Security_TASK_03.docx` — Full security report including business impact and remediation steps.
* 📁 `/Screenshots` — Directory containing Postman test evidence and response validations.
