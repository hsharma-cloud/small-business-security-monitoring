# Small Business Security Monitoring Environment

## Overview

This project demonstrates the design and deployment of a centralized security monitoring environment for a small business infrastructure.

The environment simulates common enterprise systems such as web applications, database servers, storage systems, domain services, and endpoint devices. Security telemetry from these systems is aggregated into a centralized monitoring platform to provide visibility into authentication activity, system events, and potential security threats.

The goal of this project is to demonstrate practical experience with infrastructure monitoring, host-based intrusion detection, and security event analysis.

---

## Infrastructure Architecture

The environment represents a small business network with centralized monitoring capabilities. Multiple infrastructure systems forward security telemetry to a centralized monitoring server.

```
                     Internet
                        │
                        ▼
                     fw01
                    Firewall
                        │
                        ▼
                Internal Network
                        │
        ┌───────────────┼───────────────┐
        ▼               ▼               ▼
      web01            db01         storage01
   Web Server      Database Server  Storage Server
                        │
                        ▼
                     siem01
              Security Monitoring Server

        ┌───────────────┴───────────────┐
        ▼                               ▼
      dc01                         Client Systems
  Domain Controller             winclient01
                                linclient01
                                kali01
```
---

## Infrastructure Components

| Hostname | Role |
|---------|------|
| fw01 | Network firewall |
| siem01 | Centralized security monitoring server |
| web01 | Web application server |
| db01 | Database server |
| storage01 | File storage server |
| dc01 | Domain controller |
| winclient01 | Windows workstation |
| linclient01 | Linux workstation |
| kali01 | Security testing host |

---

## Security Monitoring

Security telemetry from multiple systems is collected and analyzed by the centralized monitoring platform. The monitoring system provides visibility into system activity, authentication events, and potential security incidents across the environment.

Monitoring capabilities include:

- system log collection  
- authentication monitoring  
- file integrity monitoring  
- web server activity monitoring  
- centralized alerting  

---

## Detection Scenarios

The monitoring environment allows simulation and detection of several types of security events:

- brute force authentication attempts  
- suspicious web requests  
- unauthorized file modifications  
- abnormal system activity  
- privilege escalation attempts  

These events are aggregated and analyzed by the monitoring platform to generate security alerts.

---

## Technology Stack

- Security Monitoring Platform: Wazuh  
- Firewall Platform: pfSense  
- Web Server: Apache  
- Operating Systems: Ubuntu Server, Windows Server  
- Virtualization Platform: VMware Workstation  
- Security Testing Tools: Kali Linux  

---

## Project Highlights

- Designed a centralized security monitoring architecture  
- Implemented host-based intrusion detection across multiple systems  
- Aggregated system and security telemetry into a SIEM platform  
- Simulated attack scenarios using a security testing host  
- Demonstrated detection of suspicious activity through monitoring alerts  

---

## Future Enhancements

Potential improvements to this environment include:

- custom detection rules  
- automated attack simulations  
- threat intelligence integration  
- additional endpoint monitoring  
- advanced alert correlation  

---

## Screenshots

Screenshots of the monitoring dashboard and system components will be added in a future update.
