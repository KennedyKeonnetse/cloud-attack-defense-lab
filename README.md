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
