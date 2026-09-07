# Networkwalks-B082-Week4-Penetation-Testing-Report
Authorized penetration testing assessment of the Mediroza web application, documenting identified vulnerabilities, security findings, supporting evidence, impact, and remediation recommendations.

# 🏥 Mediroza – Web Application Penetration Testing

> **Authorized Security Assessment | Penetration Testing Report**

[![Security Assessment](https://img.shields.io/badge/Assessment-Penetration%20Testing-red)]()
[![Platform](https://img.shields.io/badge/Platform-Web%20Application-blue)]()
[![Status](https://img.shields.io/badge/Status-Completed-success)]()

---

## 📋 Table of Contents

- [Executive Summary](#-executive-summary)
- [Scope & Methodology](#-scope--methodology)
- [Tools Used](#-tools-used)
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

# 🛠️ Tools Used

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



