# 🟡 Incident Report: Yellow RAT – Suspicious Network Activity

## Incident Overview
- **Case Name:** Yellow RAT
- **Platform:** CyberDefenders
- **Category:** Malware / Network Traffic Analysis
- **Severity:** High
- **Status:** Closed
- **Verdict:** <True Positive / False Positive>

---

## 1. Executive Summary
A security investigation was conducted after detecting abnormal network traffic originating from an internal host.
The analysis focused on identifying potential malware activity, determining command-and-control (C2) communication,
and confirming whether the behavior was associated with a Remote Access Trojan (RAT).

---

## 2. Trigger Event
The investigation was initiated due to suspicious network activity observed in captured network traffic (PCAP).
The traffic pattern indicated possible automated communication with an external system.

- **Detection Source:** Network Monitoring / PCAP Analysis
- **Initial Suspicion:** Possible malware-related communication

---

## 3. Investigation & Analysis

### 3.1 Network Traffic Analysis
The provided PCAP file was analyzed to identify abnormal traffic patterns and suspicious protocols.

- Observed repeated connections to an external IP address
- Traffic did not align with normal user browsing behavior
- Communication appeared consistent and automated

---

### 3.2 Identification of Rogue or Malicious Host
Internal IP addresses were reviewed to determine the source of the suspicious traffic.

- Internal source IP identified
- Behavior suggested compromise of the host
- Traffic characteristics were inconsistent with legitimate services

---

### 3.3 Malware Identification
Further analysis was performed to determine the malware family involved.

- Indicators suggested the presence of a Remote Access Trojan (RAT)
- Behavioral patterns aligned with known RAT activity
- Findings were correlated with known threat intelligence

---

### 3.4 Command and Control (C2) Communication
The suspicious traffic was evaluated to confirm command-and-control behavior.

- External destination identified as potential C2 server
- Communication pattern supported remote command execution capability
- This behavior increased confidence in malicious classification

---

## 4. Indicators of Compromise (IOCs)

| Type | Value | Description |
|-----|------|------------|
| Internal IP | <IP Address> | Compromised host |
| External IP | <IP Address> | Suspected C2 server |
| Protocol | <Protocol> | Used for C2 communication |

---

## 5. Verdict
Based on the network traffic analysis and behavior observed, the incident was classified as:

- **Verdict:** <True Positive / False Positive>

The evidence supported the presence of malware-related activity consistent with a Remote Access Trojan.

---

## 6. Containment & Recommendations
Recommended actions based on the investigation:

- Isolate the affected host from the network
- Block communication with identified external IPs
- Perform endpoint malware scanning and remediation
- Monitor for similar traffic patterns across the network

---

## 7. Analyst Notes
This case strengthened understanding of network-based malware detection,
PCAP analysis techniques, and identifying command-and-control communication
associated with Remote Access Trojans.
