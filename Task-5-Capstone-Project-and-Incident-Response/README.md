# Task 5 – Capstone Project

## Vulnerability Assessment of Test Network

## Overview

This capstone project demonstrates a complete vulnerability assessment of a controlled test network.

The assessment was performed using Kali Linux as the security testing system and Metasploitable 2 as the intentionally vulnerable target.

The project covers network reconnaissance, vulnerability assessment, controlled exploitation, incident response, log analysis, findings, and security recommendations.

## Lab Environment

### Attacker

* Kali Linux

### Target

* Metasploitable 2

### Virtualization

* Oracle VirtualBox

### Network

* Host-Only Network
* Kali Linux ↔ Metasploitable 2

## Tools Used

* Oracle VirtualBox
* Kali Linux
* Metasploitable 2
* Nmap
* OpenVAS / Greenbone
* Metasploit Framework
* John the Ripper
* Wireshark
* iptables

## Project Phases

### 00 – Lab Setup

Contains documentation for:

* VirtualBox configuration
* Kali Linux setup
* Metasploitable 2 setup
* Network configuration
* Lab screenshots

### 01 – Project Planning

Contains:

* Project objectives
* Project scope
* Tools used
* Project timeline

### 02 – Network Diagram

Contains the network diagram showing the relationship between the host system, Kali Linux, and Metasploitable 2.

### 03 – Reconnaissance

Nmap was used to identify:

* Open ports
* Running services
* Service versions
* Operating system information
* Network details

### 04 – Vulnerability Assessment

OpenVAS / Greenbone was used to identify vulnerabilities on the target system.

The assessment includes:

* Scan configuration
* Vulnerability findings
* Severity information
* Vulnerability details
* OpenVAS report
* Screenshots

### 05 – Controlled Exploitation

Selected vulnerabilities were tested in the controlled lab using the Metasploit Framework and password-security tools.

The purpose was to demonstrate the potential impact of identified vulnerabilities without targeting real systems.

### 06 – Incident Response

The project includes:

* Detection
* Containment
* Incident analysis
* Post-incident documentation
* Log analysis

System logs such as authentication, system, and Apache logs were reviewed to identify relevant security events.

### 07 – Final Report

Contains the consolidated vulnerability assessment report, including:

* Executive Summary
* Methodology
* Findings
* Risk analysis
* Mitigations
* Conclusion

### 08 – Presentation

Contains presentation material and supporting content for the project demonstration.

### 09 – Video

Contains the capstone project demonstration video showing the assessment process and findings.

### 10 – Screenshots

Contains supporting screenshots collected throughout the project.

## Key Findings

The assessment demonstrated that an intentionally vulnerable system can expose multiple security weaknesses through outdated services, vulnerable configurations, and weak authentication practices.

The findings were analyzed and documented with recommended security mitigations.

## Recommended Mitigations

* Apply security patches and updates.
* Remove or disable unnecessary services.
* Restrict network exposure.
* Use strong authentication.
* Protect password hashes.
* Configure firewall rules.
* Monitor authentication and system logs.
* Regularly perform vulnerability assessments.
* Keep security tools and operating systems updated.

## Project Evidence

The repository contains:

* Planning documents
* Network diagram
* Nmap scan results
* OpenVAS vulnerability report
* Metasploit evidence
* Password-security testing evidence
* Incident-response documentation
* Log-analysis documentation
* Screenshots
* Final report
* Demonstration video

## Disclaimer

This project was performed exclusively in a controlled lab environment using intentionally vulnerable systems for educational and cybersecurity training purposes.

No unauthorized systems or networks were targeted.

## Author

**Vanam Chenchu Puneeth**

Cyber Security & Ethical Hacking Internship
ApexPlanet Software Pvt. Ltd.

