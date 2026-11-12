# Project Overview
## Banking Application – Production Support & Incident Management Lab
---

## 1. Introduction

The **Banking Application – Production Support & Incident Management Lab** is an independent, hands-on technical project designed to simulate real-world application support and production troubleshooting scenarios in the banking and financial technology domain.

The project focuses on understanding how enterprise banking applications operate, how different technical components interact, and how Technical Support Engineers investigate, troubleshoot, resolve and document application-related incidents.

It provides practical exposure to multiple technologies commonly used in IT support environments, including Java, Oracle SQL, REST APIs, Linux, Windows, application logs, monitoring tools, networking and incident management.

The project simulates the responsibilities of an **L1/L2 Technical Support Engineer or Application Support Analyst** working in a banking application support environment and any other environment.

## 2. Project Objectives

The primary objectives of this project are:

- Understand the architecture and transaction lifecycle of a banking application.
- Develop and troubleshoot a basic Java-based banking application.
- Test and investigate REST APIs using Postman.
- Perform database operations and transaction investigations using Oracle SQL.
- Understand Linux server administration and command-line troubleshooting.
- Investigate Windows application and system errors.
- Analyse application logs to identify technical failures.
- Monitor application health and performance.
- Troubleshoot networking, DNS, connectivity and SSL/TLS certificate issues.
- Simulate real-world production incidents.
- Prepare incident reports, escalation notes and Root Cause Analysis (RCA).
- Develop practical troubleshooting and technical documentation skills.

## 3. Project Scope

The project covers the following technical areas:

| Technical Area | Scope |
|---|---|
| Application Support | Java application troubleshooting |
| API Support | REST API testing and error investigation |
| Database Support | Oracle SQL and transaction investigation |
| Linux Administration | Processes, services, disk and memory |
| Windows Support | Event Viewer and Windows Services |
| Log Analysis | Application and system log investigation |
| Monitoring | Application health and performance monitoring |
| Networking | DNS, TCP/IP, ports and connectivity |
| Security | SSL/TLS certificate fundamentals |
| Incident Management | Ticket handling and prioritisation |
| Problem Management | Root Cause Analysis and prevention |
| Documentation | Troubleshooting guides and technical reports |

## 4. Application Architecture

The simulated banking application follows a simplified transaction-processing architecture.

### Transaction Flow

1. A customer initiates a payment request.
2. The request reaches the application through a REST API.
3. The Java application validates the request.
4. The application communicates with the database.
5. Oracle Database stores customer and transaction information.
6. The application processes the payment request and updates its status.
7. Application logs capture transaction activities, warnings and errors.
8. Monitoring tools help identify application performance and availability issues.
9. The Technical Support Engineer investigates and documents any reported incident.

### Architecture Components

| Component | Responsibility |
|---|---|
| Customer Interface | Initiates banking transactions |
| REST API | Receives and processes application requests |
| Java Application | Handles business logic and validation |
| Oracle Database | Stores customer and transaction records |
| Linux Server | Hosts the application environment |
| Windows Environment | Provides administrative and troubleshooting practice |
| Logging System | Records application events and errors |
| Monitoring Tools | Tracks availability and performance |
| Support Engineer | Investigates incidents and coordinates resolution |

## 5. Technology Stack

The following technologies and tools are included in the project.

### Programming and Application
- Java
- Spring Boot
- REST APIs
- JSON

### API Testing
- Postman
- HTTP methods
- HTTP status codes
- Request and response analysis

### Database
- Oracle Database Free
- Oracle SQL Developer
- SQL queries
- DDL and DML
- TCL commands
- Constraints and joins

### Operating Systems
- Ubuntu Linux
- Windows 10/11
- Linux command-line utilities
- Windows Event Viewer
- Windows Services

### Monitoring and Log Analysis
- Grafana
- Dynatrace (where trial or learning access is available)
- Application logs
- System logs
- Log-level analysis

### Networking and Security
- TCP/IP
- DNS
- HTTP/HTTPS
- Port connectivity
- SSL/TLS
- OpenSSL

### Version Control and Documentation
- Git
- GitHub
- Markdown
- Incident documentation
- RCA reports

## 6. Technical Support Responsibilities

Within this simulated environment, the Technical Support Engineer performs the following responsibilities:

1. Receive and understand reported application issues.
2. Identify the affected service, functionality and users.
3. Assess business impact and incident priority.
4. Investigate application errors using logs and monitoring tools.
5. Execute database queries to validate transaction records.
6. Troubleshoot API responses and application connectivity.
7. Check Linux processes, services and server resources.
8. Investigate Windows application and system events.
9. Identify the probable root cause using collected evidence.
10. Resolve issues within authorised scope or escalate them to the appropriate technical team.
11. Verify application recovery and functionality.
12. Document the investigation and final resolution.

## 7. Production Support Scenarios

The project will simulate common banking application incidents.

| Incident ID | Scenario | Primary Tools |
|---|---|---|
| INC001 | Payment API returning HTTP 500 | Postman, Java Logs |
| INC002 | API authentication failure | Postman |
| INC003 | Transaction stuck in pending status | Oracle SQL |
| INC004 | Database connection failure | Oracle SQL, Java Logs |
| INC005 | Application response time degradation | Linux, Monitoring |
| INC006 | Application service unavailable | Linux, systemctl |
| INC007 | Server disk space issue | Linux, df, du |
| INC008 | High CPU utilisation | Linux, top, ps |
| INC009 | DNS resolution failure | nslookup, dig |
| INC010 | Application port connectivity failure | curl, nc, ss |
| INC011 | SSL certificate validation failure | OpenSSL |
| INC012 | Windows application crash | Event Viewer |
| INC013 | User account login failure | Active Directory concepts |
| INC014 | Application log error investigation | grep, tail, less |
| INC015 | Multiple transaction failures | SQL, Logs, Incident Management |

Each incident will include:

- Incident description
- Reported symptoms
- Business impact
- Priority classification
- Investigation steps
- Commands and tools used
- Technical findings
- Root cause
- Resolution or escalation
- Verification and closure notes

## 8. Incident Management and RCA

Incident management is an important part of this project.

Each simulated incident will be documented using a structured support process.

### Incident Priority Classification

| Priority | Description | Example |
|---|---|---|
| P1 - Critical | Major service outage or widespread business impact | Banking payment service unavailable |
| P2 - High | Significant functionality affected | Multiple payment transactions failing |
| P3 - Medium | Limited functionality or users affected | Individual transaction processing issue |
| P4 - Low | Minor issue or service request | General application information request |

Actual priority assignment should follow business impact and urgency, along with the organisation's incident policy.

### Root Cause Analysis

For every resolved incident, an RCA document will contain:

- Incident summary
- Timeline of events
- Customer or business impact
- Technical investigation
- Identified root cause
- Resolution implemented
- Recovery verification
- Preventive and corrective actions

## 9. Project Development Approach

The project will be implemented in six stages.

| Phase | Focus Area | Expected Deliverable |
|---|---|---|
| Phase 1 | Linux and Windows | OS troubleshooting documentation |
| Phase 2 | Oracle SQL | Banking database and SQL scripts |
| Phase 3 | Java and REST APIs | Sample payment application |
| Phase 4 | Logs and Monitoring | Log analysis and monitoring dashboard |
| Phase 5 | Networking and Security | Network and certificate troubleshooting guide |
| Phase 6 | Production Support | Incident reports and RCA documentation |

## 10. Expected Learning Outcomes

Upon completing the project, the expected learning outcomes include:

- Understanding application support and production support workflows.
- Practical knowledge of Java application troubleshooting.
- Ability to test and investigate REST APIs.
- Ability to perform database queries and transaction investigations.
- Familiarity with Linux and Windows troubleshooting.
- Understanding application logs and monitoring.
- Ability to investigate common networking issues.
- Understanding SSL/TLS certificate validation.
- Knowledge of incident prioritisation and escalation.
- Ability to prepare technical documentation and RCA reports.

## 11. Repository Structure

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
├── README.md
└── PROJECT-OVERVIEW.md
```

## 12. Project Status

**Current Status:** In Progress

This repository is being developed as a practical learning environment. Application modules, SQL scripts, troubleshooting exercises, monitoring dashboards and incident documentation will be added progressively.

The project will be updated as each development and troubleshooting phase is completed.

## 13. Disclaimer

This project is independently developed for educational and professional skill-development purposes.

It uses simulated banking scenarios and sample data. It is not affiliated with any bank, financial institution or commercial banking platform.

No real customer information, banking credentials or confidential production data should be used.

## 14. Author

**Sakhar Thakur**

Aspiring Technical Support Engineer | Application Support | Production Support

---

**Project Focus:** Learn by building, troubleshoot by investigating, and improve by documenting.
