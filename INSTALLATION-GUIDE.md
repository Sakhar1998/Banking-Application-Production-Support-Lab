# Installation Guide – Banking Application Production Support Lab

## 1. Introduction

This guide explains how to set up the local environment for the Banking Application – Production Support & Incident Management Lab.

The project is designed to provide hands-on experience with application support, production troubleshooting, database operations, API testing, Linux commands, log analysis, monitoring, and incident management.

Follow the installation steps in sequence.

---

## 2. System Requirements

Recommended minimum system configuration:

| Component | Requirement |
|---|---|
| Operating System | Windows 10/11 or Ubuntu Linux |
| RAM | 8 GB minimum; 16 GB recommended |
| Processor | Intel i5 / AMD equivalent |
| Storage | 20 GB free space |
| Internet | Required for downloading tools |
| GitHub Account | Required for project documentation |

### Recommended Development Environment

- Windows 11
- Ubuntu Linux through WSL2
- Visual Studio Code
- Java JDK 17 or later
- Maven
- Oracle Database or Oracle Free
- Postman
- Git and GitHub
---

## 3. Install Git

Git is used for source-code management and maintaining project documentation.

### Windows Installation

1. Visit https://git-scm.com/downloads
2. Download Git for Windows.
3. Run the installer.
4. Follow the default installation options.
5. Open Command Prompt or PowerShell.

Verify installation:

```bash
git --version
```

Configure your Git identity:

```bash
git config --global user.name "Your Name"
git config --global user.email "your-email@example.com"
```

---

## 4. Install Visual Studio Code

Visual Studio Code is used to edit Java code, SQL scripts, configuration files, and project documentation.

1. Visit https://code.visualstudio.com/
2. Download Visual Studio Code.
3. Install and launch the application.
4. Open the project folder.

Recommended extensions:

- Extension Pack for Java
- SQL Developer Extension (if compatible with your database workflow)
- REST Client
- GitLens
- Markdown All in One

---

## 5. Install Java JDK

Java is required to build and run the sample banking application.

1. Visit https://adoptium.net/
2. Download a suitable JDK 17 or later release.
3. Install the JDK.
4. Configure the JAVA_HOME environment variable if it is not configured automatically.
5. Add the JDK bin directory to your system PATH.

Verify installation:

```bash
java -version
javac -version
```

Expected result: Java version information should be displayed.

---

## 6. Install Apache Maven

Maven is used to manage Java project dependencies and build the application.

1. Visit https://maven.apache.org/download.cgi
2. Download the binary archive.
3. Extract it to a suitable folder.
4. Configure the MAVEN_HOME environment variable if needed.
5. Add the Maven bin directory to PATH.

Verify installation:

```bash
mvn -version
```

Expected result: Maven version and Java runtime information should be displayed.

---

## 7. Install Oracle Database

Oracle Database will be used to practise SQL queries, transaction monitoring, database troubleshooting, and data validation.

### Option A: Oracle Database Free

1. Visit https://www.oracle.com/database/free/
2. Review the supported operating systems and system requirements.
3. Download the appropriate Oracle Database Free package.
4. Follow Oracle's installation instructions.
5. Set up a database user for the project.

### Option B: Oracle Live SQL

If you do not want to install a database locally, use:

https://livesql.oracle.com/

Oracle Live SQL provides a browser-based environment for practising SQL.

### Verify Database Connectivity

Connect using SQL Developer or another Oracle-compatible client.

Example connection details:

```text
Hostname: localhost
Port: 1521
Service Name: <your-configured-service-name>
Username: <your-project-username>
Password: <your-configured-password>
```

The hostname, port, service name, username, and password depend on your installation. Do not assume these example values are already configured.

---

## 8. Install Postman

Postman is used to test REST APIs and troubleshoot application requests.

1. Visit https://www.postman.com/downloads/
2. Download Postman.
3. Install and launch the application.
4. Create a workspace named:

```text
Banking Application Support Lab
```

Create a sample API request:

```http
GET http://localhost:8080/health
```

This request will work only after the application and its health endpoint have been implemented and started.

---

## 9. Set Up Linux Using WSL2

Linux commands are important for application support and log analysis.

For Windows users, Ubuntu can be installed through Windows Subsystem for Linux.

Open PowerShell as Administrator:

```powershell
wsl --install
```

Restart the system if requested, then complete the Ubuntu setup.

Verify Linux:

```bash
uname -a
```

Update Ubuntu packages:

```bash
sudo apt update
sudo apt upgrade -y
```

Install useful support utilities:

```bash
sudo apt install curl wget net-tools dnsutils traceroute tree vim -y
```

Practise the following commands:

```bash
pwd
ls -la
cd
mkdir
touch
cat
less
grep
find
tail
ps
top
df -h
free -m
```

---

## 10. Install Windows Support Utilities

The project also covers basic Windows application and system troubleshooting.

Familiarise yourself with:

- Event Viewer
- Services
- Task Manager
- Resource Monitor
- Device Manager
- Windows Firewall
- PowerShell

Useful PowerShell commands:

```powershell
Get-Service
Get-Process
Get-EventLog -LogName System -Newest 20
ipconfig /all
nslookup example.com
Test-NetConnection example.com -Port 443
```

Some commands may require Administrator privileges. Use them only on systems you are authorised to manage.

---

## 11. Clone the GitHub Repository

Once your repository has been created, open Command Prompt, PowerShell, or the Linux terminal.

Run:

```bash
git clone https://github.com/YOUR-USERNAME/Banking-Application-Production-Support-Lab.git
```

Navigate into the project:

```bash
cd Banking-Application-Production-Support-Lab
```

Open the folder in Visual Studio Code:

```bash
code .
```

Replace `YOUR-USERNAME` with your actual GitHub username.

---

## 12. Configure the Project

Create the following folders if they do not already exist:

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
├── PROJECT-OVERVIEW.md
└── INSTALLATION-GUIDE.md
```

---

## 13. Verify Your Environment

Run the following commands to confirm that the main tools are installed:

```bash
git --version
java -version
javac -version
mvn -version
```

For Linux:

```bash
uname -a
df -h
free -m
curl --version
```

For network connectivity:

```bash
ping example.com
nslookup example.com
```

For Windows PowerShell:

```powershell
Get-Service
Get-Process
ipconfig
```

Confirm that you can also connect to your Oracle database and send a test request using Postman once the application is available.

---

## 14. Common Installation Issues

| Issue | Possible Cause | Troubleshooting |
|---|---|---|
| Java command not recognised | Incorrect PATH configuration | Check JAVA_HOME and PATH |
| Maven command not recognised | Maven not configured | Verify Maven installation and PATH |
| Oracle connection failed | Incorrect connection details or database not running | Check service status, hostname, port and service name |
| Port already in use | Another application is using the port | Identify the process and check its configuration |
| API connection refused | Application is not running | Check application status and logs |
| Git command not recognised | Git not installed or PATH missing | Reinstall or configure PATH |
| DNS resolution failed | DNS or network issue | Check DNS settings and use nslookup |

---

## 15. Security Guidelines

- Never upload passwords, API keys, or database credentials to GitHub.
- Do not use real customer information or banking data.
- Use dummy transaction records and test accounts.
- Store sensitive configuration in environment variables or an excluded local configuration file.
- Do not expose database ports or application services publicly.
- Use only systems and networks you are authorised to access.

---

## 16. Installation Completion Checklist

- [ ] Git installed and configured
- [ ] Visual Studio Code installed
- [ ] Java JDK installed
- [ ] Maven installed
- [ ] Oracle Database or Oracle Live SQL accessible
- [ ] Postman installed
- [ ] Ubuntu / WSL2 configured
- [ ] Windows troubleshooting utilities reviewed
- [ ] GitHub repository cloned
- [ ] Project folders created
- [ ] Basic connectivity verified

---

## 17. Next Steps

After completing the installation:

1. Create the banking database schema.
2. Insert sample customer and transaction records.
3. Develop a basic Java banking application.
4. Create and test REST API endpoints.
5. Practise Linux log analysis.
6. Simulate application failures.
7. Document incidents and root cause analysis.
8. Capture screenshots and publish your work on GitHub.

---

## Disclaimer

This is an educational project created to demonstrate practical application support and production troubleshooting skills. It is not a live banking application and does not connect to any real banking system.
