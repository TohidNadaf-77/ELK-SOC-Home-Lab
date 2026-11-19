# ELK SOC Home Lab – Centralized Log Monitoring and Threat Detection

## Project Overview
Designed and implemented a virtual Security Operations Center (SOC) home lab using the ELK Stack to collect, centralize, monitor, and analyze security logs from Windows and Kali Linux virtual machines.

## Lab Architecture
- **Ubuntu Server 24.04:** Hosted the ELK Stack.
- **Elasticsearch:** Stored and indexed security logs.
- **Logstash:** Received and processed incoming logs.
- **Kibana:** Used for log searching, monitoring, and investigation.
- **Windows VM:** Forwarded Windows Event Logs using Winlogbeat.
- **Kali Linux VM:** Forwarded Linux system and authentication logs using rsyslog.
- **Oracle VirtualBox:** Provided the virtual lab environment.

## Log Collection and Integration
- Configured Winlogbeat to forward Windows logs to Logstash through TCP port 5044.
- Configured rsyslog to forward Kali Linux logs through TCP port 5514.
- Configured Logstash pipelines to process incoming logs and forward them to Elasticsearch.
- Used Kibana Discover to search and investigate collected security events.

## Detection and Investigation Use Cases
- Monitored successful and failed Windows login events (Event IDs 4624 and 4625).
- Investigated Linux SSH authentication activity.
- Developed detection logic for repeated failed login attempts followed by a successful login.
- Practiced security event monitoring and authentication log investigation.

## Tools and Technologies
Elasticsearch | Logstash | Kibana | Winlogbeat | rsyslog | Ubuntu Server | Kali Linux | Windows | Oracle VirtualBox

## Learning Outcomes
- SIEM deployment and configuration.
- Centralized log collection and processing.
- Windows and Linux security log analysis.
- Authentication event investigation.
- Basic security detection engineering.

## Disclaimer
This project was developed in a controlled virtual lab environment for educational and cybersecurity learning purposes.
