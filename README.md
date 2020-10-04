# Data Protection Standard

## 1. Overview

GetCraft create an access control data protection policy to make sure users can access only the assets they need to do their jobs — in other words, to enforce a least-privilege model. This policy is implemented with a combination of technical controls and training to educate users about their responsibilities for protection of data.

## 2. Purpose

GetCraft must restrict access to confidential and sensitive data to protect it from being lost or compromised in order to avoid adversely impacting our customers, incurring penalties for non-compliance and suffering damage to our reputation. At the same time, we must ensure users can access data as required for them to work effectively.

It is not anticipated that this policy can eliminate all malicious data theft. Rather, its primary objective is to increase user awareness and avoid accidental loss scenarios, so it outlines the requirements for data breach prevention.

## 3. Scope

This data security policy applies all customer data, personal data, or other GetCraft data defined as sensitive by the GetCraft's [data classification policy](general/data-classification-policy.md). Therefore, it applies to every server, database and IT system that handles such data, including any device that is regularly used for email, web access or other work-related tasks. Every user who interacts with GetCraft IT services is also subject to this policy.

## 4. Policy

### 4.1 Principles

GetCraft shall provide all employees and contracted third parties with access to the information they need to carry out their responsibilities as effectively and efficiently as possible.

### 4.2 General

1.  Each user shall be identified by a unique user ID so that individuals can be held accountable for their actions.
2. The use of shared identities is permitted only where they are suitable, such as training accounts or service accounts. 
3. Each user shall read this data security policy and the login and logoff guidelines, and sign a statement that they understand the conditions of access.
4. Records of user access may be used to provide evidence for security incident investigations.
5. Access shall be granted based on the principle of least privilege, which means that each program and user will be granted the fewest privileges necessary to complete their tasks.

### 4.3 **Access Control Authorization**

Access to GetCraft IT resources and services will be given through the provision of a unique user account and complex password. Accounts are provided by the IT department based on records in the HR department. 

Passwords are managed by the IT Service Desk. Requirements for password length, complexity and expiration are stated in the GetCraft's [Password Policy](general/password-protection-policy.md). 

Role-based access control \(RBAC\) will be used to secure access to all file-based resources in Active Directory domains. 

### **4.4 Network Access**

1. All employees and contractors shall be given network access in accordance with business access control procedures and the least-privilege principle.
2. All staff and contractors who have remote access to GetCraft networks shall be authenticated using the VPN authentication mechanism only.
3. Segregation of networks shall be implemented as recommended by the GetCraft's network security research. Network administrators shall group together information services, users and information systems as appropriate to achieve the required segregation.
4. Network routing controls shall be implemented to support the access control policy.

### 4.5 User Responsibilities

1. All users must lock their screens whenever they leave their desks to reduce the risk of unauthorized access.
2. All users must keep their workplace clear of any sensitive or confidential information when they leave.
3. All users must keep their passwords confidential and not share them.

### 4.6 **Application and Information Access**

1. All GetCraft staff and contractors shall be granted access to the data and applications required for their job roles.
2. All GetCraft staff and contractors shall access sensitive data and systems only if there is a business need to do so and they have approval from higher management.
3. Sensitive systems shall be physically or logically isolated in order to restrict access to authorized personnel only.

### 4.7 **Access to Confidential, Restricted information**

1.  Access to data classified as ‘Confidential’ or ‘Restricted’ shall be limited to authorized persons whose job responsibilities require it, as determined by the Data Security Policy or higher management.
2. The responsibility to implement access restrictions lies with the IT Security department. 

## **5. Technical Guidelines**

Access control methods to be used shall include:

* Auditing of attempts to log on to any device on the GetCraft network
* Windows NTFS permissions to files and folders
* Role-based access model
* Server access rights
* Firewall permissions
* Network zone and VLAN ACLs
* Web authentication rights
* Database access rights and ACLs
* Encryption at rest and in flight
* Network segregation

Access control applies to all networks, servers, workstations, laptops, mobile devices, web applications and websites, cloud storages, and services.

## 6. Reporting Requirements

1. Daily incident reports shall be produced and handled within the IT Security department or the incident response team.
2. Weekly reports detailing all incidents shall be produced by the IT Security department and sent to the IT manager or director.
3. High-priority incidents discovered by the IT Security department shall be immediately escalated; the IT manager should be contacted as soon as possible.
4. The IT Security department shall also product a monthly report showing the number of IT security incidents and the percentage that were resolved.

## 7. Ownership and Responsibilities

1. **Data owners** are employees who have primary responsibility for maintaining information that they own, such as an executive, department manager or team leader.
2. **Information Security Administrator** is an employee designated by the IT management who provides administrative support for the implementation, oversight and coordination of security procedures and systems with respect to specific information resources.
3. **Users** include everyone who has access to information resources, such as employees, trustees, contractors, consultants, temporary employees and volunteers.
4. **The Incident Response Team** shall be chaired by an executive and include employees from departments such as IT Infrastructure, IT Application Security, Legal, Financial Services and Human Resources.

## 8. Policy Compliance

### 8.1 Compliance Measurement

Each business unit must be able to demonstrate they have a written SRP in place, and that it is under version control and is available via the web. The policy should be reviewed annually.

### 8.2 Exceptions

Any exception to this policy must be approved by the DevSecOps Team in advance and have a written record.

### 8.3 Non-Compliance

Any user found in violation of this policy is subject to disciplinary action, up to and including termination of employment. Any third-party partner or contractor found in violation may have their network connection terminated.

## 9. Related Standards, Policies and Processes

* [Data Classification Policy](general/data-classification-policy.md)
* [Password Policy](general/password-protection-policy.md)
* [Encryption Policy](general/acceptable-encryption-policy.md)
* [Incident Response Policy](general/security-response-policy.md)

## 10. Definitions and Terms

* **Access control list \(ACL\)** — A list of access control entries \(ACEs\) or rules. Each ACE in an ACL identifies a trustee and specifies the access rights allowed, denied or audited for that trustee.
* **Database** — An organized collection of data, generally stored and accessed electronically from a computer system.
* **Encryption**—The process of encoding a message or other information so that only authorized parties can access it.
* **Firewall** — A technology used for isolating one network from another. Firewalls can be standalone systems or can be included in other devices, such as routers or servers.
* **Network segregation** — The separation of the network into logical or functional units called zones. For example, you might have a zone for sales, a zone for technical support and another zone for research, each of which has different technical needs.
* **Role-based access control \(RBAC\)** — A policy-neutral access-control mechanism defined around roles and privileges.
* **Server** — A computer program or a device that provides functionality for other programs or devices, called clients.
* **Virtual private network \(VPN\)** — A secure private network connection across a public network.
* **VLAN \(virtual LAN\)** — A logical grouping of devices in the same broadcast domain.

## 11. Revision History

| **Date of Change** | **Responsible** | **Summary of Change** |
| :--- | :--- | :--- |
| October 2020 | GetCraft DevSecOps Team | Initial version |

