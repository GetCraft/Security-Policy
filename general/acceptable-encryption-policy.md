# Acceptable Encryption Policy

## 1. Overview

See [Purpose](acceptable-encryption-policy.md#2-purpose).

## 2. Purpose

The purpose of this policy is to provide guidance that limits the use of encryption to those algorithms that have received substantial public review and have been proven to work effectively. Additionally, this policy provides direction to ensure that Federal regulations are followed, and legal authority is granted for the dissemination and use of encryption technologies outside of the United States.

## 3. Scope

This policy applies to all GetCraft employees and affiliates.

## 4. Policy

### **4.1 Algorithm Requirements**

1. Ciphers in use must meet or exceed the set defined as "AES-compatible" or "partially AES-compatible" according to the [IETF/IRTF Cipher Catalog](http://tools.ietf.org/html/draft-irtf-cfrg-cipher-catalog-01#section-3.1), or the set defined for use in the United States [National Institute of Standards and Technology \(NIST\) publication FIPS 140-2](http://csrc.nist.gov/groups/STM/cmvp/documents/140-1/1401val2010.htm), or any superseding documents according to the date of implementation. The use of the Advanced Encryption Standard \(AES\) is strongly recommended for symmetric encryption.
2. Algorithms in use must meet the standards defined for use in NIST publication [FIPS 140-2](http://csrc.nist.gov/groups/STM/cmvp/documents/140-1/1401val2010.htm) or any superseding document, according to date of implementation. The use of the RSA and Elliptic Curve Cryptography \(ECC\) algorithms is strongly recommended for asymmetric encryption.
3. Signature Algorithms

<table>
  <thead>
    <tr>
      <th style="text-align:left"><b>Algorithm</b>
      </th>
      <th style="text-align:left">
        <p><b>Key Length</b>
        </p>
        <p><b>(min)</b>
        </p>
      </th>
      <th style="text-align:left"><b>Additional Comment</b>
      </th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">ECDSA</td>
      <td style="text-align:left">P-256</td>
      <td style="text-align:left">Consider <a href="https://tools.ietf.org/html/rfc6090">RFC6090</a> to avoid
        patent infringement.</td>
    </tr>
    <tr>
      <td style="text-align:left">RSA</td>
      <td style="text-align:left">2048</td>
      <td style="text-align:left">Must use a secure padding scheme. <a href="http://tools.ietf.org/html/rfc3852#section-6.3">PKCS#7 padding scheme</a> is
        recommended. Message hashing required.</td>
    </tr>
    <tr>
      <td style="text-align:left">LDWM</td>
      <td style="text-align:left">SHA256</td>
      <td style="text-align:left">Refer to <a href="http://tools.ietf.org/html/draft-mcgrew-hash-sigs-00">LDWM Hash-based Signatures Draft</a>
      </td>
    </tr>
  </tbody>
</table>

### 4.2 Hash Function Requirements

In general, GetCraft adheres to the [NIST Policy on Hash Functions](http://csrc.nist.gov/groups/ST/hash/policy.html).

### 4.3 Key Agreement and Authentication

1. Key exchanges must use one of the following cryptographic protocols: Diffie-Hellman, IKE, or Elliptic curve Diffie-Hellman \(ECDH\).
2. End points must be authenticated prior to the exchange or derivation of session keys.
3. Public keys used to establish trust must be authenticated prior to use. Examples of authentication include transmission via cryptographically signed message or manual verification of the public key hash.
4. All servers used for authentication \(for example, RADIUS or TACACS\) must have installed a valid certificate signed by a known trusted provider.
5. All servers and applications using SSL or TLS must have the certificates signed by a known, trusted provider.

### 4.4 Key Generation

1. Cryptographic keys must be generated and stored in a secure manner that prevents loss, theft, or compromise.
2. Key generation must be seeded from an industry standard random number generator \(RNG\). For examples, see [NIST Annex C: Approved Random Number Generators for FIPS PUB 140-2](http://csrc.nist.gov/publications/fips/fips140-2/fips1402annexc.pdf).

## 5. Policy Compliance

### 5.1 Compliance Measurement

The DevSecOps team will verify compliance to this policy through various methods, including but not limited to, business tool reports, internal and external audits, and feedback to the policy owner.

### 5.2 Exceptions

Any exception to the policy must be approved by the DevSecOps team in advance.

### 5.3 Non-Compliance

An employee found to have violated this policy may be subject to disciplinary action, up to and including termination of employment.

## 6. Related Standards, Policies and Processes

* [National Institute of Standards and Technology \(NIST\) publication FIPS 140-2](http://csrc.nist.gov/groups/STM/cmvp/documents/140-1/1401val2010.htm)
* [NIST Policy on Hash Functions](http://csrc.nist.gov/groups/ST/hash/policy.html)

## 7. Definitions and Terms

The following definition and terms can be found in the SANS Glossary located at: https://www.sans.org/security-resources/glossary-of-terms/

* Proprietary Encryption

## 8. Revision History

| **Date of Change** | **Responsible** | **Summary of Change** |
| :--- | :--- | :--- |
| October 2020 | GetCraft DevSecOps Team | Initial version |
|  |  |  |

