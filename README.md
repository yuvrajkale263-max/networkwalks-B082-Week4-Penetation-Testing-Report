# Networkwalks-B082-Week4-Penetation-Testing-Report
Authorized penetration testing assessment of the Mediroza web application, documenting identified vulnerabilities, security findings, supporting evidence, impact, and remediation recommendations.

# 🏥 Mediroza – Web Application Penetration Testing

> **Authorized Security Assessment | Penetration Testing Report**


---

## 📋 Table of Contents

- [Executive Summary](#-executive-summary)
- [Scope & Methodology](#-scope--methodology)
- [Tools Used](#tools-used)
- [Security Findings](#-security-findings)
- [Risk Rating Summary](#-risk-rating-summary)
- [Recommendations & Remediation](#-recommendations--remediation)
- [Evidence](#-evidence)
- [Lessons Learned](#-lessons-learned)
- [Final Deliverables](#-final-deliverables)
- [Disclaimer](#-disclaimer)

---

# 🎯 Executive Summary

## Assessment Overview

A security assessment was conducted against the **Mediroza web application** to identify vulnerabilities that could potentially allow unauthorized access, information disclosure, or compromise of sensitive organizational data.

The assessment followed a structured penetration testing methodology covering reconnaissance, enumeration, vulnerability identification, exploitation, data-access validation, evidence collection, and reporting.

| Category                 | Details                                                              |
| ------------------------ | -------------------------------------------------------------------- |
| 🏢 **Target**            | Mediroza Web Application                                             |
| 🌐 **Client**            | https://medirozahospital.com
| 🔐 **Assessment Type**   | Black box Web Application Penetration Test                           |
| 🎯 **Primary Objective** | Identify and validate security vulnerabilities                       |
| 🔎 **Testing Approach**  | Reconnaissance → Enumeration → Exploitation → Validation → Reporting |
| 📊 **Assessment Status** | Completed                                                            |
| 📄 **Deliverable**       | Detailed Penetration Testing Report                                  |

---

## 🚨 Executive Findings

The assessment identified security weaknesses that could lead to unauthorized access and exposure of sensitive information within the target environment.

A critical finding involved the exposure of **sensitive employee and shareholder information**. The exposed employee information included salary and employment-related details, while shareholder information included ownership and shareholding details.

This demonstrates a significant **confidentiality risk**, as unauthorized access to such information could expose sensitive personal and organizational data.

### 🔴 Critical Data Exposure

| Data Category                  | Information Exposed                                            |
| ------------------------------ | -------------------------------------------------------------- |
| 👤 **Employee Information**    | Names, job roles, departments, monthly salaries, joining dates |
| 📈 **Shareholder Information** | Names, ownership percentages, shares held, share classes       |

> **Impact:** Exposure of sensitive employee and organizational information may result in privacy violations, reputational damage, targeted attacks, and unauthorized disclosure of confidential business information.

---

## 🎯 Assessment Objectives

The assessment was performed with the following objectives:

* 🔎 Identify vulnerabilities within the target application.
* 🚪 Validate potential unauthorized access paths.
* 📂 Determine whether sensitive information could be accessed.
* 💥 Assess the practical impact of identified vulnerabilities.
* 📸 Collect evidence supporting each security finding.
* 🛡️ Provide remediation recommendations to reduce the identified risks.

---

# 🔍 Scope & Methodology

## 🎯 Scope

The penetration testing assessment was performed against the **Mediroza web application** within the authorized testing environment.

The assessment focused on identifying vulnerabilities that could allow unauthorized access, data extraction, or exposure of sensitive organizational information.

### 🌐 Target

| Category              | Details                                                   |
| --------------------- | --------------------------------------------------------- |
| **Target**            | Mediroza Web Application                                  |
| **Assessment Type**   | Authorized Penetration Testing                            |
| **Testing Objective** | Identify, validate, and document security vulnerabilities |

---

## 🧪 Methodology

The assessment followed a structured penetration testing methodology designed to identify vulnerabilities, safely validate their impact, and document sufficient evidence for remediation.

### 1. 🔎 Reconnaissance

Initial information was gathered about the target environment to identify accessible services, application components, and potential attack surfaces.

### 2. 🗺️ Enumeration

The discovered attack surface was examined to identify available endpoints, application functionality, parameters, services, and potentially exposed resources.

### 3. 🐛 Vulnerability Identification

The application and discovered resources were analyzed for security weaknesses that could potentially result in unauthorized access or information disclosure.

### 4. 💥 Exploitation & Validation

Identified vulnerabilities were safely validated within the authorized environment to determine whether the suspected weaknesses could be exploited and to assess their practical impact.

### 5. 📂 Data Access & Exposure Assessment

Following successful exploitation, accessible information was examined to determine whether sensitive or confidential organizational data could be obtained.

### 6. 📸 Evidence Collection

Screenshots and relevant technical evidence were collected throughout the assessment to demonstrate the identified vulnerabilities and their impact.

### 7. 📊 Risk Assessment

Each confirmed finding was evaluated based on its potential impact and security significance.

### 8. 📝 Reporting

The confirmed findings were documented with their description, impact, evidence, risk rating, and recommended remediation measures.

---

#  Tools Used

| Tool                       | Purpose                                          |
| -------------------------- | ------------------------------------------------ |
| **Kali Linux**             | Primary penetration testing environment          |
| **curl**                   | HTTP requests, header & endpoint analysis        |
| **Nmap**                   | Network and service discovery                    |
| **Burp Suite**             | Web application traffic interception and testing |
| **Web Browser**            | Application interaction and manual testing       |
| **Command-Line Utilities** | Supporting enumeration and analysis activities   |

> **Note:** Tools were selected based on the requirements of each testing phase. Not every tool was necessarily used for every finding.

---

# 🐛 Security Findings

The penetration testing assessment identified multiple security weaknesses within the Mediroza environment. The confirmed findings are summarized below.

## 📊 Findings Overview

| ID | Finding | Severity | Status |
|---|---|---|---|
| 🔴 **M1** | Initial Access | **High** | ✅ Confirmed |
| 🔴 **M2** | Data Extraction | **High** | ✅ Confirmed |
| 🔴 **M3** | Critical Data Exposure | **Critical** | ✅ Confirmed |

---

## 🔴 M1 – Initial Access

### Description

The assessment identified a vulnerability that allowed the tester to obtain initial access to the target environment.

The successful exploitation of this weakness established an initial foothold and enabled further security testing of the compromised environment.

### Impact

Successful initial access could allow an unauthorized attacker to continue reconnaissance, access application resources, and potentially reach sensitive information depending on the privileges available.

### Evidence

Supporting screenshots demonstrating the initial access are available in the [`Screenshots/`](./Screenshots/) directory.

---

## 🔴 M2 – Data Extraction

### Description

Following successful initial access, further testing was performed to determine what information could be accessed or extracted from the target environment.

The assessment demonstrated that data could be retrieved from the compromised environment.

### Impact

Unauthorized data extraction can result in the loss of confidentiality and may expose organizational information to unauthorized parties.

### Evidence

Supporting screenshots demonstrating the data extraction process are available in the [`Screenshots/`](./Screenshots/) directory.

---

## 🔴 M3 – Critical Data Exposure

### Description

A critical data exposure was identified during the assessment. Sensitive employee and shareholder information was accessible within the target environment.

The employee salary data contained records for **20 hospital employees**, including:

- Employee names
- Job roles
- Departments
- Monthly salaries
- Joining dates

The shareholder data contained:

- Shareholder names
- Ownership percentages
- Shares held
- Share classes

### Impact

The exposure of this information represents a significant **confidentiality risk** because sensitive employee and organizational information could be accessed by an unauthorized party.

Potential consequences include:

- Exposure of employee financial information
- Disclosure of confidential organizational information
- Privacy concerns for affected individuals
- Reputational damage
- Potential misuse of exposed information

### Evidence

Supporting screenshots demonstrating the exposed employee salary and shareholder information are available in the [`Screenshots/`](./Screenshots/) directory.

---

# ▥ Risk Rating Summary

The identified vulnerabilities were assessed according to their potential impact on the confidentiality, integrity, and availability of the Mediroza environment.

## Risk Overview

| Finding | Security Issue | Severity | Risk |
|---|---|---|---|
| **M1** | Initial Access | High | Significant |
| **M2** | Data Extraction | High | Significant |
| **M3** | Critical Data Exposure | **Critical** | **Critical** |

---

## Risk Classification

### 🔴 Critical

**M3 – Critical Data Exposure**

The exposure of sensitive employee salary information and shareholder information represents a critical confidentiality risk. The accessible information includes sensitive financial, employment, ownership, and organizational data.

### 🟠 High / Significant

**M1 - Initial Access**

The initial access and subsequent data extraction findings demonstrate that weaknesses in the target environment could be used to progress from unauthorized access toward access to sensitive information.

---

## Overall Risk Assessment

The assessment indicates that the identified vulnerabilities can have a significant impact on the confidentiality of sensitive Mediroza information.

The most significant risk identified during the assessment was the exposure of sensitive employee and shareholder data. Appropriate access controls, authorization mechanisms, and protection of sensitive information should therefore be prioritized.

> **Overall Priority:** Remediate the critical data exposure and address the vulnerabilities that enabled access to the affected information.

# ➜ Recommendations & Remediation

The following remediation actions are recommended based on the vulnerabilities confirmed during the Mediroza penetration testing assessment. Actions should be prioritized according to their potential impact and exploitability.

### Priority 1 — Immediate

- Remediate the confirmed **SQL Injection** vulnerability by implementing parameterized queries/prepared statements throughout the application.
- Remove the exposed **old database backup (`mediroza_db_backup_2019.sql`)** from the publicly accessible web directory immediately.
- Investigate the contents of the exposed database backup and determine whether any sensitive or outdated credentials/data could be abused.
- Investigate whether the exposed backup was accessed or downloaded by unauthorized parties.
- Disable unnecessary **directory listing/indexing** across the web server.
- Immediately restrict unauthorized access to sensitive employee and shareholder information.
- Review and secure all application endpoints that allow direct access to database-backed resources.
- Store future database backups outside the web root, encrypt them, and restrict access to authorized personnel only.

### Priority 2 — High

- Strengthen authentication mechanisms using secure password hashing and appropriate credential-management controls.
- Implement **Multi-Factor Authentication (MFA)** for sensitive accounts and administrative functionality where applicable.
- Implement **rate limiting and account lockout controls** to reduce the risk of brute-force attacks.
- Implement effective **CSRF protection** for state-changing requests.
- Replace static or weak PDF/document passwords with strong, securely managed secrets and enforce application-level authorization before allowing document access.
- Remove verbose database and application error messages from the production environment.
- Ensure database errors are logged securely on the server without exposing implementation details to users.

### Priority 3 — Medium / Low

- Use generic authentication error messages to reduce the possibility of username/account enumeration.
- Minimize technology and version disclosure through HTTP headers, server responses, and application-generated errors.
- Remove unnecessary information from headers such as `Server` and `X-Powered-By`.
- Implement security monitoring for failed authentication attempts, SQL injection patterns, suspicious requests, and unauthorized access to sensitive files.
- Store database backups outside the publicly accessible web root.
- Encrypt sensitive backups and restrict backup access to authorized personnel only.
- Conduct periodic security assessments and penetration tests to identify newly introduced vulnerabilities.
- Perform regression testing after remediation to confirm that the identified vulnerabilities have been fully resolved.

# ⊙ Evidence

Evidence was collected throughout the penetration testing assessment to validate the identified vulnerabilities and demonstrate their impact.

All screenshots published in this repository have been reviewed and redacted where sensitive information was present.

## Evidence Overview

| Milestone | Evidence | Description |
|---|---|---|
| **M1 – Initial Access** | [`M1 Evidence`](./Screenshots/M1-Initial-Access/) | Authentication bypass, patient portal access, and access to patient reports. |
| **M2 – Data Extraction** | [`M2 Evidence`](./Screenshots/M2-Data-Extraction/) | Access to three PDF reports and validation of their password protection. |
| **M3 – Critical Data Exposure** | [`M3 Evidence`](./Screenshots/M3-Critical-Data-Exposure/) | Exposure of the database backup, employee salary data, and shareholder information. |

---

## M1 – Initial Access

The M1 evidence demonstrates the initial access obtained during the assessment.

| Evidence | Description |
|---|---|
| [`Authentication Bypass`](./Screenshots/M1-Initial-Access/M1_01_Authentication_Bypass(Redacted).png) | Evidence of the identified authentication bypass. |
| [`Patient Portal`](./Screenshots/M1-Initial-Access/M1_02_Patient_Portal(Redacted).png) | Evidence of access to the patient portal. |
| [`Three Patient Reports`](./Screenshots/M1-Initial-Access/M1_03_Three_Patient_Reports.png) | Evidence showing three patient reports retrieved. |

---

## M2 – Data Extraction

The M2 evidence demonstrates access to the protected PDF documents and the password-cracking activity performed during the assessment.

| Evidence | Description |
|---|---|
| [`PDF 1 – Access`](./Screenshots/M2-Data-Extraction/M2_01_PDF1_Access(Redacted).png) | Evidence of access to the first PDF document. |
| [`PDF 1 – Password Crack`](./Screenshots/M2-Data-Extraction/M2_01_PDF1_Password_Crack(Redacted).png) | Evidence related to cracking the first PDF password. |
| [`PDF 2 – Access`](./Screenshots/M2-Data-Extraction/M2_02_PDF2_Access(Redacted).png) | Evidence of access to the second PDF document. |
| [`PDF 2 – Password Crack`](./Screenshots/M2-Data-Extraction/M2_02_PDF2_Password_Crack(Redacted).png) | Evidence related to cracking the second PDF password. |
| [`PDF 3 – Access`](./Screenshots/M2-Data-Extraction/M2_03_PDF3_Access(Redacted).png) | Evidence of access to the third PDF document. |
| [`PDF 3 – Password Crack`](./Screenshots/M2-Data-Extraction/M2_03_PDF3_Password_Crack(Redacted).png) | Evidence related to cracking the third PDF password. |

---

## M3 – Critical Data Exposure

The M3 evidence demonstrates the exposure of sensitive information through the accessible database backup and SQL output.

| Evidence | Description |
|---|---|
| [`Exposed Database Backup`](./Screenshots/M3-Critical-Data-Exposure/Database_Backup_Exposed(Redacted).png) | Evidence of the exposed database backup. |
| [`Employee Salary SQL Output`](./Screenshots/M3-Critical-Data-Exposure/Salary_SQL_Output(Redacted).png) | Evidence showing the extracted employee salary information. |
| [`Shareholder SQL Output`](./Screenshots/M3-Critical-Data-Exposure/Shareholders_SQL_Output(Redacted).png) | Evidence showing the extracted shareholder information. |


---

## 🔐 Evidence Handling

The screenshots included in this repository have been redacted where necessary to reduce unnecessary exposure of sensitive information.

The evidence is provided to demonstrate the vulnerabilities identified during the authorized assessment and to support the findings documented in the final penetration testing report.

# ✦ Lessons Learned

The Mediroza assessment provided practical insight into how multiple security weaknesses can contribute to broader security exposure when they are not adequately controlled.

### Key Takeaways

- **Authentication controls are critical:** Weaknesses in authentication can provide an attacker with an initial entry point into an application.
- **Access control must be enforced server-side:** Sensitive resources should never be accessible solely because an endpoint or resource can be discovered.
- **Sensitive documents require strong protection:** Password-protected documents should use strong, securely managed credentials and appropriate application-level authorization.
- **Exposed backups create significant risk:** Database backups should never be placed in publicly accessible web directories.
- **SQL Injection can expose large amounts of information:** Database-layer vulnerabilities can allow unauthorized access to sensitive records and should be addressed using secure query practices such as parameterized queries.
- **Sensitive data exposure should be minimized:** Employee, financial, ownership, and other confidential information should only be accessible to users with a legitimate business requirement.
- **Evidence-based validation is important:** Confirming vulnerabilities through controlled exploitation provides a clearer understanding of their actual security impact.
- **Security should be approached holistically:** Authentication, authorization, application security, database security, data protection, and monitoring should work together rather than being treated as isolated controls.

### Overall Lesson

The assessment demonstrated how an attacker can progress from an initial weakness toward access to increasingly sensitive resources. Effective security therefore requires not only fixing individual vulnerabilities, but also reviewing how weaknesses can be chained together to affect the overall security posture.

# ▰ Final deliverables

| Assessment Stage | Key Outcome | Completion |
|---|---|:---:|
| **Reconnaissance** | Target surface and accessible resources identified | 🟢 Complete |
| **Initial Access** | Authentication weakness validated and access established | 🟢 Complete |
| **Patient Portal** | Unauthorized portal access demonstrated | 🟢 Complete |
| **Document Retrieval** | Three patient reports successfully retrieved | 🟢 Complete |
| **Document Security** | Passwords recovered | 🟢 Complete |
| **Data Validation** | Recovered PDFs decrypted and verified | 🟢 Complete |
| **Database Exposure** | Publicly accessible database backup identified | 🟢 Complete |
| **Employee Data** | Salary information exposure validated | 🟢 Complete |
| **Shareholder Data** | Ownership information exposure validated | 🟢 Complete |
| **Evidence Collection** | Redacted screenshots and supporting evidence organized | 🟢 Complete |
| **Risk Assessment** | Findings evaluated and prioritized | 🟢 Complete |
| **Remediation** | Security recommendations documented | 🟢 Complete |
| **Final Documentation** | Professional penetration testing report completed | 🟢 Complete |

### Assessment Outcome

The assessment objectives were completed, with technical findings validated and supporting evidence organized for review.

# ! Disclaimer

This repository documents an **authorized penetration testing assessment** performed against the Mediroza environment.

The information presented, including technical findings, screenshots, and supporting evidence, is provided for **security assessment, documentation, and educational purposes**.

### Authorized Use

- All testing activities were performed within the defined assessment scope.
- Testing was conducted for the purpose of identifying and validating security weaknesses.
- Evidence has been redacted where necessary before being published publicly.
- The techniques documented in this repository should only be used against systems for which explicit authorization has been obtained.

### Responsible Disclosure

The vulnerabilities and security issues documented in this repository are intended to support remediation and security improvement. Unauthorized exploitation of these techniques against systems without permission is strictly prohibited.
