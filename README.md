# Nmap Network Enumeration Lab

## Overview

This project documents my hands-on learning of network discovery and service enumeration using Nmap in a controlled lab environment.

The goal was to understand how hosts and network services can be identified, enumerated, and documented during a security assessment.

## Lab Objectives

- Discover active hosts on a network
- Identify open TCP ports
- Detect running services and versions
- Understand basic Nmap scan types
- Document findings clearly
- Practice security reconnaissance in an authorized lab environment

## Tools Used

- Kali Linux
- Nmap
- Linux terminal
- Virtual machines / controlled lab environment

## Nmap Techniques Practiced

### 1. Host Discovery

```bash
nmap -sn <target-network>/24
```

### 2. Service and Version Detection

```bash
nmap -sV <target>
```
### Example Lab Result

```text
Target: 192.168.43.106
Port: 5357/tcp
State: open
Service: HTTP
Version: Microsoft HTTPAPI 2.0
OS: Windows
```
### 3. Basic Port Scanning

```bash
nmap <target>
```
### Example Lab Result

```text
Target: 192.168.43.106
Port: 5357/tcp
State: open
Service: wsdapi
```

## Findings & Interpretation

The scan identified an active Windows host at `192.168.43.106`.

Port `5357/tcp` was discovered as open. Service and version detection identified the service as Microsoft HTTPAPI 2.0, while the basic Nmap scan identified the service as `wsdapi`.

This exercise demonstrated how Nmap can be used to:
- Discover active hosts
- Identify exposed ports
- Detect running services
- Gather basic service and operating system information
