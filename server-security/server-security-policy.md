# Server Security Policy

## 1. Overview

Unsecured and vulnerable servers continue to be a major entry point for malicious threat actors. Consistent Server installation policies, ownership and configuration management are all about doing the basics well.

## 2. Purpose

The purpose of this policy is to establish standards for the base configuration of internal server equipment that is owned and/or operated by GetCraft. Effective implementation of this policy will minimize unauthorized access to GetCraft proprietary information and technology.

## 3. Scope

All employees, contractors, consultants, temporary and other workers at GetCraft and its subsidiaries must adhere to this policy. This policy applies to server equipment that is owned, operated, or leased by GetCraft or registered under a GetCraft-owned internal network domain.

## 4. Policy

### 4.1 General Requirements

4.1.1 All internal servers deployed at GetCraft must be owned by an operational group that is responsible for system administration. Approved server configuration guides must be established and maintained by each operational group, based on business needs and approved by DevSecOps. Operational groups should monitor configuration compliance and implement an exception policy tailored to their environment. Each operational group must establish a process for changing the configuration guides, which includes review and approval by DevSecOps. The following items must be met:

* Servers must be registered within the corporate enterprise management system. At a minimum, the following information is required to positively identify the point of contact:
  * Server contact\(s\) and location, and a backup contact
  * Hardware and Operating System/Version
  * Main functions and applications, if applicable
* Information in the corporate enterprise management system must be kept up-to-date.
* Configuration changes for production servers must follow the appropriate change management procedures

4.1.2 For security, compliance, and maintenance purposes, authorized personnel may monitor and audit equipment, systems, processes, and network traffic.

### 4.2 Configuration Requirements

1. Operating System configuration should be in accordance with approved DevSecOps guidelines.
2. Services and applications that will not be used must be disabled where practical.
3. Access to services should be logged and/or protected through access-control methods such as a web application firewall, if possible.
4. The most recent security patches must be installed on the system as soon as practical, the only exception being when immediate application would interfere with business requirements.
5. Trust relationships between systems are a security risk, and their use should be avoided. Do not use a trust relationship when some other method of communication is sufficient.
6. Always use standard security principles of least required access to perform a function. Do not use root when a non-privileged account will do.
7. If a methodology for secure channel connection is available \(i.e., technically feasible\), privileged access must be performed over secure channels, \(e.g., encrypted network connections using SSH or IPSec\).

### 4.3 Monitoring

4.3.1 All security-related events on critical or sensitive systems must be logged and audit trails saved as follows:

* All security related logs will be kept online for a minimum of 1 week.
* Daily incremental tape backups will be retained for at least 1 month.
* Weekly full tape backups of logs will be retained for at least 1 month.
* Monthly full backups will be retained for a minimum of 2 years.

4.3.2 Security-related events will be reported to DevSecOps, who will review logs and report incidents to IT management. Corrective measures will be prescribed as needed. Security-related events include, but are not limited to:

* Port-scan attacks
* Evidence of unauthorized access to privileged accounts
* Anomalous occurrences that are not related to specific applications on the host.

## 5. Policy Compliance

### 5.1 Compliance Measurement

The DevSecOps team will verify compliance to this policy through various methods, including but not limited to, periodic walk-thrus, video monitoring, business tool reports, internal and external audits, and feedback to the policy owner.

### 5.2 Exceptions

Any exception to the policy must be approved by the DevSecOps team in advance.

### 5.3 Non-Compliance

An employee found to have violated this policy may be subject to disciplinary action, up to and including termination of employment.

## 6. Related Standards, Policies and Processes

* None

## 7. Definitions and Terms

The following definition and terms can be found in the SANS Glossary located at: [https://www.sans.org/security-resources/glossary-of-terms](https://www.sans.org/security-resources/glossary-of-terms)

* De-militarized zone \(DMZ\)

## 8. Revision History

| **Date of Change** | **Responsible** | **Summary of Change** |
| :--- | :--- | :--- |
| October 2020 | GetCraft DevSecOps Team | Initial version |
|  |  |  |

