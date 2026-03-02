# CS 305 Software Security Portfolio – Artemis Financial

## Artifact Included
This repository includes my completed **Artemis Financial Vulnerability Assessment Report (Project One)**.

---

## Brief Client Summary and Software Requirements
Artemis Financial is a financial services organization that develops a web application used to handle sensitive customer financial information and potentially personally identifiable information (PII). The client needed a vulnerability assessment to identify security risks and determine mitigations to protect confidentiality and integrity, enforce strong access controls, and ensure secure communications (TLS/HTTPS) end-to-end.

## What I Did Well and Why Secure Coding Matters
I did well at using a structured approach to identify vulnerabilities through manual code inspection and static dependency scanning. I documented clear findings and connected them to business risk. Secure coding matters because security failures can lead to data exposure, fraud, downtime, and loss of trust—especially in financial applications. Strong software security supports compliance expectations, reduces operational risk, and protects customers and the organization.

## Most Challenging or Helpful Part of the Assessment
The most challenging part was interpreting findings and deciding what was most critical to fix first (for example, separating code-level issues from dependency vulnerabilities). The most helpful part was pairing a manual review with dependency scanning because it revealed both “custom code” risks and known third-party library risks.

## Layers of Security Added and Future Approach
I increased security using a defense-in-depth mindset by recommending improvements such as: removing hard-coded secrets, enforcing authentication/authorization on endpoints, validating inputs, improving error handling to prevent information leakage, hardening file upload settings, and addressing vulnerable dependencies.  
In the future, I would continue using a combination of manual secure code review, SAST, and software composition analysis (dependency scanning), and I would choose mitigations based on severity, exploitability, and business impact.

## Ensuring the Application Stayed Functional and Secure
To ensure the application remained functional and secure after changes, I would confirm the project still builds and runs as expected, then re-run security checks (dependency scanning and static analysis) to verify issues are resolved and to confirm no new vulnerabilities were introduced. I would also add unit tests for boundary conditions (such as validation rules) and re-test key application workflows.

## Resources, Tools, and Practices Used
Key tools and practices I used include:
- OWASP Dependency-Check to identify known vulnerable third-party dependencies
- Secure coding practices such as input validation, least privilege, safe error handling/logging, and defense-in-depth
- Dependency/version management practices (upgrading to patched versions and tracking known CVEs)
- Following structured assessment guidance (Vulnerability Assessment Process Flow)

## What I Would Show Future Employers
For future employers, I would show my completed vulnerability assessment report as evidence that I can:
- identify vulnerabilities through code review and tooling,
- explain business/security impact,
- prioritize remediation,
- and propose realistic mitigation steps (including dependency upgrades and secure coding improvements).

---

## References

Iron-Clad Java. (n.d.). *Secure software development lifecycle*.

National Institute of Standards and Technology. (2015). *Secure hash standard (SHS) (FIPS PUB 180-4).* U.S. Department of Commerce.

National Institute of Standards and Technology. (2016). *CVE-2016-1000342 detail.* National Vulnerability Database.

National Institute of Standards and Technology. (2018). *CVE-2018-5382 detail.* National Vulnerability Database.

National Institute of Standards and Technology. (2020). *CVE-2020-26939 detail.* National Vulnerability Database.

National Institute of Standards and Technology. (2022). *CVE-2022-27772 detail.* National Vulnerability Database.

Oracle. (n.d.). *Secure coding guidelines for Java SE.* Oracle.

OWASP Foundation. (n.d.). *OWASP dependency-check.*

SNHU. (2026). *CS 305 vulnerability assessment process flow diagram.*

Spring. (2022). *CVE-2022-22950: Spring Expression DoS vulnerability.* Spring Security Advisories.

Spring. (2022). *CVE-2022-22965: Spring Framework RCE via data binding.* Spring Security Advisories.
