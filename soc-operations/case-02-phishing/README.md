# 📧 Incident Report: SOC140 – Phishing Email

## Incident Overview
- **Platform:** LetsDefend
- **Case ID:** SOC140
- **Category:** Phishing / Email Security
- **Severity:** Medium
- **Status:** Closed
- **Verdict:** <True Positive / False Positive>

---

## 1. Executive Summary
A suspicious email was reported and analyzed to determine whether it constituted a phishing attempt.
The investigation focused on validating the sender, analyzing the email content,
and assessing any associated attachments or links.
Based on the findings, an appropriate verdict and response action were determined.

---

## 2. Trigger Event
The investigation began after a phishing-related alert was generated.

- **Detection Source:** Email Security Gateway / User Report
- **Alert Type:** Suspicious Email
- **Target User:** <Username>
- **Sender Email:** <Sender Address>

---

## 3. Investigation & Analysis

### 3.1 Email Header Analysis
Email headers were reviewed to validate the authenticity of the sender.

- From / Reply-To comparison
- SPF, DKIM, and DMARC results
- Indicators of email spoofing or domain impersonation

![Email header analysis](images/email-headers.png)

---

### 3.2 Email Content Analysis
The email body was analyzed to identify social engineering techniques.

- Urgent language or pressure tactics
- Suspicious wording or formatting
- Requests for sensitive information or action

![Email body showing phishing indicators](images/email-body.png)

---

### 3.3 Attachment or URL Analysis
Any attachment or embedded link was analyzed for malicious intent.

- **Attachment Name / URL:** <Value>
- **File Hash (if applicable):** <Hash>

Threat intelligence tools were used to assess reputation.

![Attachment or URL reputation analysis](images/attachment-analysis.png)

---

### 3.4 Threat Intelligence Validation
External threat intelligence sources were consulted to confirm malicious indicators.

- URL or file reputation results
- Detection by multiple security vendors
- Correlation with known phishing campaigns

![Threat intelligence results](images/threat-intel.png)

---

## 4. Indicators of Compromise (IOCs)

| Type | Value | Description |
|------|------|------------|
| Sender Email | <Email Address> | Suspicious sender |
| URL | <URL> | Phishing link |
| File Hash | <Hash Value> | Malicious attachment |

---

## 5. Verdict
Based on header analysis, content inspection, and threat intelligence validation,
the email was classified as:

- **Verdict:** <True Positive / False Positive>

---

## 6. Response & Recommendations
The following actions were recommended or performed:

- Block sender domain or email address
- Remove the email from user mailbox
- Block malicious URLs or attachments
- Provide user awareness or training

---

## 7. Analyst Reflection
This case enhanced understanding of phishing investigation techniques,
including email header analysis, social engineering detection,
and validating threats using intelligence sources.
