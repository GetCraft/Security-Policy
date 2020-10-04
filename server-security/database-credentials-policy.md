# Database Credentials Coding Policy

## 1. Overview

Database authentication credentials are a necessary part of authorizing applications to connect to internal databases. However, incorrect use, storage and transmission of such credentials could lead to compromise of very sensitive assets and be a springboard to wider compromise within the organization.

## 2. Purpose

This policy states the requirements for securely storing and retrieving database usernames and passwords \(i.e., database credentials\) for use by a program that will access a database running on one of GetCraft's networks.

Software applications running on GetCraft's networks may require access to one of the many internal database servers. In order to access these databases, a program must authenticate to the database by presenting acceptable credentials. If the credentials are improperly stored, the credentials may be compromised leading to a compromise of the database.

## 3. Scope

This policy is directed at all system implementers and/or software engineers who may be coding applications that will access a production database server on the GetCraft Network. This policy applies to all software \(programs, modules, libraries or APIs\) that will access GetCraft's multi-user production database. It is recommended that similar requirements be in place for non-production servers and environments since they don’t always use sanitized information.

## 4. Policy

In order to maintain the security of GetCraft's internal databases, access by software programs must be granted only after authentication with credentials. The credentials used for this authentication must not reside in the main, executing body of the program's source code in clear text. Database credentials must not be stored in a location that can be accessed through a web server.

### 4.2 Storage of Database Usernames and Passwords

1. Database usernames and passwords may be stored in a file separate from the executing body of the program's code. This file must not be world readable or writable.
2. Database credentials may reside on the database server. In this case, a hash function number identifying the credentials may be stored in the executing body of the program's code.
3. Database credentials may be stored as part of an authentication server \(i.e., an entitlement directory\), such as an LDAP server used for user authentication. Database authentication may occur on behalf of a program as part of the user authentication process at the authentication server. In this case, there is no need for programmatic use of database credentials.
4. Database credentials may not reside in the documents tree of a web server.
5. Pass through authentication \(i.e., Oracle OPS$ authentication\) must not allow access to the database based solely upon a remote user's authentication on the remote host.
6. Passwords or passphrases used to access a database must adhere to the _Password Policy_.

### 4.3 Retrieval of Database User Names and Passwords

1. If stored in a file that is not source code, then database user names and passwords must be read from the file immediately prior to use. Immediately following database authentication, the memory containing the user name and password must be released or cleared.
2. The scope into which you may store database credentials must be physically separated from the other areas of your code, e.g., the credentials must be in a separate source file. The file that contains the credentials must contain no other code but the credentials \(i.e., the username and password\) and any functions, routines, or methods that will be used to access the credentials.
3. For languages that execute from source code, the credentials' source file must not reside in the same browseable or executable file directory tree in which the executing body of code resides.

### 4.4 Access to Database Usernames and Passwords

1. Every program or every collection of programs implementing a single business function must have unique database credentials. Sharing of credentials between programs is not allowed.
2. Database passwords used by programs are system-level passwords as defined by the _Password Policy_.
3. Developer groups must have a process in place to ensure that database passwords are controlled and changed in accordance with the _Password Policy_. This process must include a method for restricting knowledge of database passwords to a need-to-know basis.

### 4.5 Coding Techniques for implementing this policy

1. _\[Add references to your site-specific guidelines for the different coding languages such as Perl, JAVA, C and/or C++.\]_

## 5. Policy Compliance

### 5.1 Compliance Measurement

The DevSecOps team will verify compliance to this policy through various methods, including but not limited to, business tool reports, internal and external audits, and feedback to the policy owner.

### 5.2 Exceptions

Any exception to the policy must be approved by the DevSecOps team in advance.

### 5.3 Non-Compliance

An employee found to have violated this policy may be subject to disciplinary action, up to and including termination of employment.

A violation of this policy by a temporary worker, contractor or vendor may result in the termination of their contract or assignment with GetCraft.

Any program code or application that is found to violate this policy must be remediated within a 90 day period.

## 6. Related Standards, Policies and Processes

* [Password Policy](../general/password-protection-policy.md)

## 7. Definitions and Terms

* Credentials
* Executing Body
* Hash Function
* LDAP
* Module

## 8. Revision History

| Date of Change | Responsible | Summary of Change |
| :--- | :--- | :--- |
| October 2020 | GetCraft DevSecOps Team | Initial version |
|  |  |  |

