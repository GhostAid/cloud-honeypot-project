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
![Honeypot Log] (WhatsApp Image 2026-06-20 at 14.28.03.jpeg)
## How to Deploy
1. Launch an AWS EC2 instance (Ubuntu 24.04, t3.micro)
2. Clone Cowrie: `git clone https://github.com/cowrie/cowrie`
3. Install dependencies and run Cowrie
4. Monitor logs for attack attempts
