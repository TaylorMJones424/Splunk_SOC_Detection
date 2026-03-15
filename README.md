# Splunk_SOC_Detection
SOC detection lab using Splunk, Sysmon, Windows Event Logs, and Kali Linux attack simulation.
## Overview
This project demonstrates a SOC detection lab built using Splunk, Windows Event Logs, Sysmon, and Kali Linux attack simulation.

The lab simulates attacker behavior and builds SIEM detections for common threats.

## Lab Architecture

Kali Linux (Attacker)
      ↓
Windows VM (Target)
   ├─ Security Logs
   ├─ Sysmon
   └─ PowerShell Logging
      ↓
Splunk Universal Forwarder
      ↓
Splunk SIEM (Ubuntu)
      ↓
Detection Queries + Alerts + Dashboard

## Data Sources

- Windows Security Logs
- Sysmon Endpoint Telemetry
- PowerShell Script Block Logging

## Simulated Attacks

1. Brute Force Login Attempt (SMB)
2. Suspicious PowerShell Execution
3. Network Scanning using Nmap

## Detections

### Brute Force Detection
