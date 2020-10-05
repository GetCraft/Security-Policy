# Data Classification Policy

## 1. Purpose

The purpose of this policy is to establish a framework for classifying data based on its sensitivity, value and criticality to GetCraft, so sensitive corporate and customer data can be secured appropriately.

## 2. Scope

This policy applies to any form of data, including paper documents and digital data stored on any type of media. It applies to all of the GetCraft’s employees, as well as to third-party agents authorized to access the data.

## 3. Roles and Responsibilities

### 3.1 Data Owner

The person who is ultimately responsible for the data and information being collected and maintained by his or her department or division, usually a member of senior management.  The data owner shall address the following:

1. **Review and categorization** — Review and categorize data and information collected by his or her department or division
2. **Assignment of data classification labels**  — Assign data classification labels based on the data’s potential impact level
3. **Data compilation** — Ensure that data compiled from multiple sources is classified with at least the most secure classification level of any individually classified data
4. **Data classification coordination** — Ensure that data shared between departments is consistently classified and protected
5. **Data classification compliance** \(in conjunction with data custodians\) — Ensure that information with high and moderate impact level is secured in accordance with federal or state regulations and guidelines
6. **Data access** \(in conjunction with data custodians\) — Develop data access guidelines for each data classification label

### 3.2 **Data Custodians**

Technicians from the IT department or, in larger organizations, the Information Security office. Data custodians are responsible for maintaining and backing up the systems, databases and servers that store the GetCraft’s data. In addition, this role is responsible for the technical deployment of all of the rules set forth by data owners and for ensuring that the rules applied within systems are working. Some specific data custodian responsibilities include:

1. **Access control —** Ensure that proper access controls are implemented, monitored and audited in accordance with the data classification labels assigned by the data owner
2. **Audit reports —** Submit an annual report to the data owners that addresses availability, integrity and confidentiality of classified data
3. **Data backups —** Perform regular backups of state data
4. **Data validation —** Periodically validate data integrity
5. **Data restoration —** Restore data from backup media
6. **Compliance —** Fulfill the data requirements specified in the GetCraft’s security policies, standards and guidelines pertaining to information security and data protection
7. **Monitor activity** — Monitor and record data activity, including information on who accessed what data
8. **Secure storage** — Encrypt sensitive data at rest while in storage; audit storage area network \(SAN\) administrator activity and review access logs regularly
9. **Data classification compliance** \(in conjunction with data owners\) — Ensure that information with high and moderate impact level is secured in accordance with federal or state regulations and guidelines
10. **Data access** \(in conjunction with data owners\) — Develop data access guidelines for each data classification label

### **3.3 Data User**

Person, organization or entity that interacts with, accesses, uses or updates data for the purpose of performing a task authorized by the data owner. Data users must use data in a manner consistent with the purpose intended, and comply with this policy and all policies applicable to data use.

## **4. Data Classification Procedure**

1. Data owners review and assign each piece of data they own an information type based on the categories in [NIST 800-600 Volume 1](https://nvlpubs.nist.gov/nistpubs/Legacy/SP/nistspecialpublication800-60v1r1.pdf).
2. Data owners assign each piece of data a potential impact level for each of the security objectives \(confidentiality, integrity, availability\), using the guide in Section 5 of this document. The highest of the three is the overall impact level.
3. Data owners assign each piece of data a classification label based on the overall impact level:

   | **Overall impact level** | **Classification label** |
   | :--- | :--- |
   | High | Restricted |
   | Moderate | Confidential |
   | Low |  Public |

4. Data owners record the impact level and classification label for each piece of data in the data classification table.
5. Data custodians apply information security controls to each piece of data according to its classification label and overall impact level.

## **5. Impact Level Determination**

<table>
  <thead>
    <tr>
      <th style="text-align:left"><b>Security Objective</b>
      </th>
      <th style="text-align:left"><b>Potential Impact</b>
      </th>
      <th style="text-align:left"></th>
      <th style="text-align:left"></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">&lt;b&gt;&lt;/b&gt;</td>
      <td style="text-align:left"><b>Low</b>
      </td>
      <td style="text-align:left"><b>Moderate</b>
      </td>
      <td style="text-align:left"><b>High</b>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p><b>Confidentiality.</b>
        </p>
        <p>Restrict access to and disclosure of data to authorized users in order
          to protect personal privacy and secure proprietary information.</p>
      </td>
      <td style="text-align:left">Unauthorized disclosure of the information is expected to have <b>limited</b> adverse
        effects on operations, organizational assets, or individuals.</td>
      <td style="text-align:left">Unauthorized disclosure of the information is expected to have a <b>serious</b> adverse
        effect on operations, organizational assets, or individuals.</td>
      <td style="text-align:left">Unauthorized disclosure of the information is expected to have a <b>severe or catastrophic</b> adverse
        effect on operations, organizational assets, or individuals.</td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p><b>Integrity</b>.</p>
        <p>Guard against improper modification or destruction of data, which includes
          ensuring information nonrepudiation and authenticity.</p>
      </td>
      <td style="text-align:left">Unauthorized modification or destruction of the information is expected
        to have a <b>limited</b> adverse effect on operations, assets, or individuals.</td>
      <td
      style="text-align:left">Unauthorized modification or destruction of the information is expected
        to have a <b>serious</b> adverse effect on operations, assets, or individuals.</td>
        <td
        style="text-align:left">Unauthorized modification or destruction of the information is expected
          to have a <b>severe or catastrophic</b> adverse effect on operations, assets,
          or individuals.</td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p><b>Availability</b>.</p>
        <p>Ensure timely and reliable access to and use of information.</p>
      </td>
      <td style="text-align:left">Disruption of access to or use of the information or information system
        is expected to have a <b>limited</b> adverse effect on operations, assets,
        or individuals.</td>
      <td style="text-align:left">Disruption of access to or use of the information or information system
        is expected to have a <b>serious</b> adverse effect on operations, assets,
        or individuals.</td>
      <td style="text-align:left">Disruption of access to or use of the information or information system
        is expected to have <b>a severe or catastrophic</b> adverse effect on operations,
        assets, or individuals.</td>
    </tr>
  </tbody>
</table>

## **6. Information that Must be Classified as “Restricted”**

### **6.1 Authentication information**

Authentication information is data used to prove the identity of an individual, system or service. Examples include:

* Passwords
* Shared secrets
* Cryptographic private keys
* Hash tables

### **6.2 Electronic Protected Health Information \(ePHI\)**

ePHI is defined as any protected health information \(PHI\) that is stored in or transmitted by electronic media. Electronic media includes computer hard drives as well as removable or transportable media, such as a magnetic tape or disk, optical disk, or digital memory card.

Transmission is the movement or exchange of information in electronic form.  Transmission media includes the internet, an extranet, leased lines, dial-up lines, private networks, and the physical movement of removable or transportable electronic storage media.

### **6.3 Payment Card Information \(PCI\)**

Payment card information is defined as a credit card number in combination with one or more of the following data elements:

* Cardholder name
* Service code
* Expiration date
* CVC2, CVV2 or CID value
* PIN or PIN block
* Contents of a credit card’s magnetic stripe

### **6.4 Personally Identifiable Information \(PII\)**

PII is defined as a person’s first name or first initial and last name in combination with one or more of the following data elements:

* Social security number
* State-issued driver’s license number
* State-issued identification card number
* Financial account number in combination with a security code, access code or password that would permit access to the account
* Medical and/or health insurance information

## 7.  Related Standards, Policies and Processes

* [Data Protection Standard](../)

## 8. Definitions and Terms

None.

## 9. Revision History

| **Date of Change** | **Responsible** | **Summary of Change** |
| :--- | :--- | :--- |
| October 2020 | GetCraft DevSecOps Team | Initial version |
|  |  |  |

