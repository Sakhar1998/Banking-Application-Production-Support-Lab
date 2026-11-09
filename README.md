# Banking-Application-Production-Support-Lab
A hands-on banking application production support project covering Java, REST APIs, Oracle SQL, Linux, Windows, log analysis, monitoring, networking, incident management and root cause analysis.

## Project Overview

The Banking Application – Production Support & Incident Management Lab is a hands-on technical project designed to simulate real-world IT production support and application troubleshooting scenarios within a banking environment.

The project focuses on understanding how banking applications operate, how different technical components communicate, and how Technical Support Engineers investigate, troubleshoot, resolve and document production incidents.

The lab combines Java application fundamentals, REST API testing, Oracle SQL database operations, Linux and Windows administration, log analysis, application monitoring, networking and incident management.

The primary objective is to develop practical L1/L2 Application Support skills and gain experience with the tools and troubleshooting methodologies commonly used in enterprise IT environments.

**Project Type:** Personal Hands-on Technical Project  
**Domain:** Banking / Financial Technology  
**Target Role:** Technical Support Engineer / Application Support Analyst  
**Focus:** Application Troubleshooting, Production Support and Incident Management

## Project Objectives

- Understand the architecture and transaction flow of a banking application.
- Build and troubleshoot a sample Java-based banking application.
- Test REST APIs and investigate HTTP errors using Postman.
- Perform database operations and transaction investigations using Oracle SQL.
- Practise Linux server administration and command-line troubleshooting.
- Investigate Windows application and system events.
- Analyse application logs to identify errors and failures.
- Understand application performance monitoring using Grafana and Dynatrace.
- Troubleshoot DNS, TCP/IP, port connectivity and SSL/TLS certificate issues.
- Simulate production incidents and prepare Root Cause Analysis (RCA) reports.
- Develop incident management, escalation and technical documentation skills.

## Technology Stack

| Category | Tools / Technologies |
|---|---|
| Programming | Java, Spring Boot |
| API Testing | Postman, REST API, JSON |
| Database | Oracle Database, SQL Developer |
| SQL | DDL, DML, TCL, Constraints, Joins |
| Operating Systems | Linux, Ubuntu, Windows |
| Linux Commands | grep, tail, ps, top, df, du, systemctl |
| Windows | Event Viewer, Windows Services |
| Monitoring | Grafana, Dynatrace |
| Networking | TCP/IP, DNS, HTTP, HTTPS, Ports |
| Certificates | SSL/TLS, OpenSSL |
| Version Control | Git, GitHub |
| ITSM Concepts | Incident Management, Priority, Escalation, RCA |

## Application Architecture

The simulated banking application follows this transaction flow:

1. Customer initiates a payment request.
2. REST API receives the request.
3. Java application validates the transaction.
4. Oracle database stores transaction information.
5. Application processes the payment request.
6. Application logs capture transaction activities and errors.
7. Monitoring tools help identify performance and availability issues.
8. Technical Support Engineer investigates incidents and coordinates resolution.

## Key Technical Modules

### 1. Java Application Support
- Understand Java application execution.
- Investigate application exceptions.
- Analyse application failures.
- Understand service availability and dependencies.

### 2. API Troubleshooting
- Test APIs using Postman.
- Understand HTTP methods and status codes.
- Analyse JSON request and response payloads.
- Investigate 400, 401, 403, 404, 500 and 503 errors.

### 3. Oracle Database Support
- Create and manage database tables.
- Perform SQL queries and data manipulation.
- Understand DDL, DML and TCL.
- Investigate pending and failed transactions.
- Troubleshoot database connectivity.

### 4. Linux Administration
- Monitor CPU and memory utilisation.
- Investigate disk space issues.
- Monitor running processes.
- Check application services.
- Analyse application and system logs.

### 5. Windows Administration
- Investigate application errors through Event Viewer.
- Monitor Windows Services.
- Understand user permissions and account management.
- Learn Active Directory fundamentals.

### 6. Log Analysis and Monitoring
- Analyse application logs.
- Identify exceptions and error patterns.
- Understand INFO, DEBUG, WARN and ERROR log levels.
- Monitor application health and performance.
- Explore Grafana and Dynatrace.

### 7. Networking and Infrastructure
- Troubleshoot DNS resolution.
- Check server connectivity.
- Investigate port connectivity issues.
- Understand TCP/IP and HTTP/HTTPS.
- Inspect SSL/TLS certificates.

### 8. Incident Management
- Create and classify incident tickets.
- Understand incident priorities P1, P2, P3 and P4.
- Document troubleshooting steps.
- Prepare technical escalation notes.
- Perform Root Cause Analysis.
- Verify service recovery and document incident closure.

## Production Support Scenarios

The project will simulate the following real-world incidents:

| Incident | Troubleshooting Tools |
|---|---|
| Payment API returning HTTP 500 | Postman, Java Logs |
| API authentication failure | Postman, Authentication |
| Transaction stuck in pending status | Oracle SQL, Logs |
| Database connection failure | Oracle SQL, Application Logs |
| Application performance degradation | Linux, Monitoring |
| Application service unavailable | Linux, systemctl |
| Server disk space issue | Linux, df, du |
| High CPU utilisation | Linux, top, ps |
| DNS resolution failure | nslookup, dig |
| Port connectivity issue | curl, nc, ss |
| SSL certificate expiry | OpenSSL |
| Windows application crash | Event Viewer |
| User login failure | Active Directory concepts |

## Repository Structure

```text
Banking-Application-Production-Support-Lab/
│
├── Application/
│   ├── Java-Code/
│   └── API-Documentation/
│
├── Database/
│   ├── Schema.sql
│   ├── Transactions.sql
│   └── Troubleshooting.sql
│
├── Linux/
│   └── Commands.md
│
├── Windows/
│   └── Event-Logs.md
│
├── Monitoring/
│   └── Dashboard-Screenshots/
│
├── Incidents/
│   ├── INC001.md
│   ├── INC002.md
│   └── INC003.md
│
├── RCA/
│   └── Root-Cause-Analysis.md
│
└── README.md
```

## Learning Outcomes

By completing this project, the expected learning outcomes are:

- Practical understanding of application support workflows.
- Ability to investigate API and database-related issues.
- Experience with Linux and Windows troubleshooting.
- Understanding of application logs and monitoring.
- Ability to investigate infrastructure and connectivity issues.
- Knowledge of incident prioritisation and escalation.
- Ability to document technical findings and prepare RCA reports.

## Project Progress

This repository is being developed as a structured hands-on learning lab.

The implementation, incident simulations, screenshots and documentation will be updated as each module is completed.

## Disclaimer

This is an independent educational project using simulated banking scenarios and sample data. It is not affiliated with any bank, financial institution or commercial banking platform.

No real customer information, banking credentials or confidential production data should be used.

## Author

**Sakhar Thakur**

Technical Support Engineer | Application Support | Production Support
