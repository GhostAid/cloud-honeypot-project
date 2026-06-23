# Cloud Honeypot Project 🍯

## Overview
This project demonstrates a cloud-based SSH honeypot using Cowrie deployed on AWS EC2.

## Architecture
- **Cloud Provider**: AWS EC2 (t3.micro, Ubuntu 24.04)
- **Honeypot**: Cowrie (Medium-interaction SSH honeypot)
- **Monitoring**: Real-time log monitoring

## What I Learned
- AWS EC2 provisioning and security groups
- SSH key management
- Linux system administration
- Honeypot deployment and configuration
- Threat intelligence gathering

## Results
- Successfully caught real attackers scanning the honeypot
- Logged attacker IP addresses and attempted credentials
- Gained hands-on experience with cloud security

## Sample Log
Here is a screenshot of a real hacker trying to break into my honeypot:
![Honeypot Log](WhatsApp Image 2026-06-20 at 14.28.03.jpeg)
## How to Deploy
1. Launch an AWS EC2 instance (Ubuntu 24.04, t3.micro)
2. Clone Cowrie: `git clone https://github.com/cowrie/cowrie`
3. Install dependencies and run Cowrie
4. Monitor logs for attack attempts

---

## Project 2: Serverless Phishing Simulation ☁️

### Overview
A serverless phishing simulation built on AWS using S3, Lambda, and CloudWatch.

### Architecture
- **Frontend**: S3 Static Website
- **Backend**: AWS Lambda (Python)
- **API**: Lambda Function URL
- **Monitoring**: CloudWatch Logs

### Skills Demonstrated
- AWS Serverless Architecture
- S3 Static Hosting
- Lambda Functions
- CloudWatch Logging
- Python Development

### Test Result
 Lambda function executed successfully with `Execution successful: Succeeded`

### CloudWatch Logging
 All login attempts were successfully logged to CloudWatch with timestamps, email addresses, and source IPs.

**Sample Log Entry:**
```json
{
    "timestamp": "2026-06-21T13:14:01.566732",
    "email": "test@example.com",
    "password_hash": "ecd71870d1963316a97e3ac3408c9835ad8cf0f3c1bc703527c30265534f75ae",
    "source_ip": "102.88.112.221"
}

## Project 3: Cloud SIEM (Wazuh) 

### Overview
Deployed a fully functional SIEM on AWS using Wazuh to monitor and detect security threats in real-time.

### Architecture
- **Wazuh Server**: AWS EC2 (Ubuntu 24.04)
- **Wazuh Agents**: Log collection from remote machines
- **Wazuh Dashboard**: Web-based monitoring and alerting

### Results
-  Successfully detected failed SSH login attempts
-  MITRE ATT&CK mapping for security events
-  Real-time alerting and monitoring

### Sample Alerts
- **Rule 5710**: Attempt to login using a non-existent user
- **Tactic**: Credential Access, Lateral Movement

###  Dashboard Screenshots

Here are screenshots of the Wazuh dashboard showing real security alerts:

![Wazuh SIEM Dashboard](Screenshot 2026-06-23 135514.png)

*Figure 1: Security alerts showing failed SSH login attempts*

![Wazuh SIEM Dashboard](Screenshot 2026-06-23 135621.png)

*Figure 2: Agent status and security events overview*
-  Real-time alerting for security events

