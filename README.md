#  Cloud Attack & Defense Lab (AWS)

## 📖 Project Overview
This repository serves as a technical demonstration of cloud security engineering and incident response. As a Network Systems Engineering student, I am building this lab to simulate real-world AWS breaches, analyze them using native security tools, and implement "Zero Trust" remediation strategies.

## Architecture Diagram
```mermaid
graph TD
    A[Internet] -->|Malicious Traffic| B(WAF / Load Balancer)
    B --> C{Vulnerable EC2}
    C -->|Lateral Movement| D[IAM Role Exploitation]
    D --> E[S3 Bucket - Sensitive Data]
    F[CloudTrail & GuardDuty] -.->|Monitoring| C
    F -.->|Monitoring| D
## 🛠️ Prerequisites & Tools
To replicate this lab, the following stack is utilized:
- **Cloud Provider:** AWS (Free Tier eligible services).
- **Operating System:** Ubuntu Server 22.04 LTS (for the vulnerable EC2).
- **Security Tools:** AWS GuardDuty, CloudTrail, and VPC Flow Logs.
- **Local Tools:** SSH, AWS CLI, and Wireshark (for packet analysis).

## 📈 Roadmap Alignment
This project is part of a multi-year specialized track (2026–2029) focusing on:
1. **Infrastructure Hardening** (Current Phase).
2. **Cloud Security Foundations**.
3. **Attack & Defense Engineering**.
