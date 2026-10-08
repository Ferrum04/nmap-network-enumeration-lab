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

