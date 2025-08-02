# Firewall Configuration Compliance Review – SecureTech

**Prepared by:** [Emmanuel Aka]  
 

## Overview

SecureTech is preparing for an upcoming PCI DSS audit. As part of the preparation, the GRC team is tasked with reviewing recent firewall configuration changes made by the IT department, specifically around the payment processing systems. This review evaluates compliance with PCI DSS firewall configuration standards.

---

## Firewall Rule Analyzed: `Allow-HTTP-to-Web`

**Rule Summary:**  
Allows HTTP traffic from an untrusted external zone to the web server located in the DMZ.

---

## PCI DSS Requirement Assessment

| **Requirement**                  | **Compliance Status** | **Notes**                                                                 |
|----------------------------------|------------------------|---------------------------------------------------------------------------|
| Encrypted Traffic (HTTPS)        | ❌ Not Compliant       | HTTP is unencrypted; PCI DSS requires encryption for sensitive data.     |
| Restriction of Access            | ❌ Not Compliant       | Traffic is allowed from an untrusted zone; this exposes systems to risk. |
| Access Logging                   | ⚠️ Incomplete           | No evidence of logging enabled for HTTP access.                           |

---

## Compliance Gaps

- **Use of Unencrypted Protocol**: HTTP is not secure and does not meet PCI DSS encryption standards.
- **Excessive Access Scope**: Permitting traffic from untrusted zones opens up potential vulnerabilities.
- **Lack of Logging**: Missing logging on firewall rules impedes accountability and threat detection.

---

## Recommendations

| **Gap**                        | **Recommended Action**                                                                 |
|-------------------------------|------------------------------------------------------------------------------------------|
| Unencrypted Protocol           | Replace HTTP with HTTPS (port 443) to ensure encrypted communication.                   |
| Unrestricted External Access   | Restrict access to a limited, trusted IP range only.                                     |
| Lack of Logging                | Enable detailed logging for this rule to aid in auditability and incident response.      |

---

## Importance of Compliance

Failure to meet PCI DSS firewall requirements could result in audit failure, data breaches, and potential fines. Encryption, restricted access, and logging are foundational controls for protecting payment environments.

---

