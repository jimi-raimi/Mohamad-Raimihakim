# Wireshark SQL Injection Traffic Analysis Lab

## Overview

This lab demonstrates the analysis of a SQL Injection attack using Wireshark and a captured PCAP file.

The objective was to investigate network traffic, identify malicious SQL Injection payloads, trace attacker activity, and understand how sensitive information can be exposed through vulnerable web applications.

---

## Lab Environment

### Analysis Platform

- CyberOps Workstation VM
- VMware Workstation

### Analysis Tool

- Wireshark

### Dataset

- SQL_Lab.pcap

---

## Objectives

- Analyze network traffic using Wireshark
- Identify SQL Injection attack patterns
- Follow HTTP streams
- Extract attacker activity
- Understand the impact of SQL Injection attacks

---

## Methodology

### Phase 1: PCAP Analysis

The captured network traffic file was loaded into Wireshark for inspection and analysis.

Activities Performed:

- Open PCAP file
- Review packet captures
- Identify suspicious HTTP traffic

Skills Demonstrated:

- Packet Analysis
- Traffic Inspection
- Wireshark Fundamentals

---

### Phase 2: HTTP Stream Investigation

Suspicious HTTP GET requests were identified and analyzed using the Follow HTTP Stream feature. The attack payloads were extracted from the captured traffic. 

Skills Demonstrated:

- HTTP Traffic Analysis
- Request Inspection
- Attack Identification

---

### Phase 3: SQL Injection Detection

Analysis revealed SQL Injection payloads designed to bypass application logic and retrieve unauthorized data from the backend database. 

Skills Demonstrated:

- SQL Injection Recognition
- Web Attack Analysis
- Threat Investigation

---

### Phase 4: Database Enumeration Analysis

The captured traffic showed attempts to retrieve:

- Database version information
- Table information
- User account information

through SQL Injection techniques. 

Skills Demonstrated:

- Database Enumeration Analysis
- Attack Progression Tracking
- Data Exposure Assessment

---

### Phase 5: Credential Exposure Investigation

The attack successfully exposed user credential information stored within the database. Password hashes were identified and analyzed as part of the investigation process.

Skills Demonstrated:

- Credential Analysis
- Incident Investigation
- Threat Analysis

---

## Key Findings

### Finding 01: SQL Injection Activity Detected

Malicious SQL Injection payloads were observed within HTTP requests targeting the web application.

### Finding 02: Database Information Disclosure

The attacker was able to retrieve database-related information through crafted SQL queries.

### Finding 03: User Credential Exposure

User account information and password hashes were exposed during the attack process.

### Finding 04: Weak Password Storage

The captured credentials demonstrated the risks associated with weak password hashing mechanisms.

---

## Security Impact

Successful SQL Injection attacks may result in:

- Unauthorized database access
- Sensitive data exposure
- Credential theft
- Privilege escalation
- Data manipulation
- Service disruption

These risks were observed throughout the analyzed attack sequence. 

---

## Mitigation Recommendations

- Implement parameterized queries
- Perform input validation and sanitization
- Use secure password hashing algorithms
- Conduct regular security testing
- Deploy Web Application Firewalls (WAF)
- Follow secure coding practices

---

## Key Learning Outcomes

- Wireshark Traffic Analysis
- HTTP Stream Investigation
- SQL Injection Detection
- Incident Investigation
- Threat Analysis
- Database Enumeration Analysis
- Credential Exposure Assessment

---

## Supporting Documentation

Detailed walkthrough and screenshots are available in:

`Wireshark-SQL-Lab.pdf`
