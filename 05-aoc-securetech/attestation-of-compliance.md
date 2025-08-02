# Attestation of Compliance (AOC)  
**Date:** 19/02/2025  
**Prepared by:** Emmanuel  
**Document Type:** For Service Providers Who Are PCI DSS Compliant  

---

## Part 1: Contact Information

- **Organization Name:** SecureTech Solutions  
- **Assessor Name:** Emmanuel  
- **Assessment Date:** 19/02/25  
- **Lead Contact Name:**  
- **Job Title:** GRC Team Lead  
- **Contact Phone/Email:**   

---

## Part 2: PCI DSS Assessment Information

- **Assessment Type:** On-Site  
- **Assessment Date(s):** 19/02/25  
- **Scope of Systems and Networks Assessed:**  
  - Cardholder Data Environment (CDE)  
  - Network Infrastructure  
  - Administrative Access Points  
  - Security Monitoring Systems  
  - Encryption Key Management Systems  
  - User Access Control Systems  

---

## Part 3: PCI DSS Validation

| Requirement | Status                         | Finding                                                                                 | Recommendation                                                             |
|------------|--------------------------------|------------------------------------------------------------------------------------------|----------------------------------------------------------------------------|
| 1          | In Place                       | Firewall and network segmentation isolate the CDE.                                      | Review and remove legacy firewall rules quarterly.                         |
| 2          | In Place with Compensating Controls | AES-256 encryption in use; key rotation delayed.                                   | Monitor access and rotate keys next month. Set annual schedule.           |
| 3          | In Place                       | Quarterly scans done; critical patches applied within 30 days.                         | Improve response time for medium-risk vulnerabilities.                    |
| 4          | Not Fully Compliant            | MFA in place, but shared accounts still used.                                           | Enforce unique IDs and extend MFA for high-risk functions.                |
| 5          | In Place                       | IDPS testing and SIEM monitoring in place.                                              | Add annual red teaming and threat simulations.                            |
| 6          | In Place                       | Updated security policy; 98% employee training completion.                             | Add bi-annual phishing/social engineering refreshers.                     |

---

## Part 4: Action Plan for Non-Compliant Requirements

- **Requirement:** Implement Strong Access Control Measures  
  - **Remediation Plan:** Eliminate shared admin accounts and enforce MFA across all critical systems.  
  - **Timeline:** Unique IDs by Q2 2024; full MFA rollout by Q3 2025. Status update in Q4 2025.  

- **Requirement:** Protect Cardholder Data  
  - **Remediation Plan:** Monitor access logs until key rotation.  
  - **Timeline:** Key rotation next month; follow-up audit in January 2026.  

---

## Part 5: Attestation and Sign-Off

By signing below, you attest that the information provided in this AOC is accurate and reflects the current state of PCI DSS compliance for the organization.

**Signature:** Emmanuel  
**Printed Name:** Emmanuel
**Job Title:** GRC analyst  
**Date:** 19/02/25  
