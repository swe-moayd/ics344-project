# ICS-344 DVSA Security Project

This repository contains the course project work for ICS-344. It documents the discovery, exploitation, mitigation, and verification of vulnerabilities in the OWASP DVSA cloud application.

---

## Project Team

| Team Member | Student ID |
| --- | --- |
| Moayd shahat| 202277460 |
| Osama alghamdi |  202172210|
| Abdullah Alzahrani| 202265440|
| RAMI ALMATHANI| 201946290 |

---

## Project Summary

This project analyzes the OWASP DVSA, a deliberately vulnerable serverless application deployed on AWS. The goal is to perform practical cloud security testing by identifying vulnerabilities, demonstrating exploitation, proposing mitigations, documenting fixes, and verifying the results after remediation.

The DVSA system uses Amazon S3, Amazon API Gateway, AWS Lambda, Amazon DynamoDB, Amazon Cognito, and Amazon CloudWatch. Each lesson follows a structured report format covering the vulnerability summary, root cause, environment setup, reproduction steps, evidence, mitigation strategy, implementation changes, verification, analysis, and lessons learned.

---

## Repository Layout

```text
ics344-Moayd-Shahat-sec1/
|-- Lesson#01/
|   `-- README.md
|-- Lesson#02/
|   `-- README.md
|-- Lesson#03/
|   `-- README.md
|-- Lesson#04/
|   `-- README.md
|-- Lesson#05/
|   |-- README.md
|   `-- images/
|-- Lesson#06/
|   `-- README.md
|-- Lesson#07/
|   |-- README.md
|   `-- images/
|-- Lesson#08/
|   |-- README.md
|   `-- images/
|-- Lesson#09/
|   `-- README.md
|-- Lesson#10/
|   `-- README.md
`-- README.md
```

Every lesson folder contains a README for that vulnerability. Folders with completed reports also include screenshot evidence under an `images/` directory.

---

## Vulnerability 


| # | Lesson Folder | Vulnerability Topic | Short Description |
| --- | --- | --- | --- |
| 1 | [Lesson#01](Lesson%2301/README.md) | Event Injection | User-supplied event data can be manipulated to alter how backend functions execute, leading to unintended behavior. |
| 2 | [Lesson#02](Lesson%2302/README.md) | Broken Authentication | Weak validation of authentication tokens may allow attackers to modify or misuse identity information. |
| 3 | [Lesson#03](Lesson%2303/README.md) | Sensitive Data Exposure | Features related to receipts may unintentionally reveal protected data or access links belonging to other users. |
| 4 | [Lesson#04](Lesson%2304/README.md) | Insecure Cloud Configuration | Misconfigured cloud resources or permissions can enable unauthorized uploads or trigger unintended processes. |
| 5 | [Lesson#05](Lesson%2305/README.md) | Broken Access Control | Internal backend operations can be accessed by regular users, allowing unauthorized modification of order states. |
| 6 | [Lesson#06](Lesson%2306/README.md) | Denial of Service | Excessive or repeated requests can overwhelm system resources and disrupt normal application functionality. |
| 7 | [Lesson#07](Lesson%2307/README.md) | Over-Privileged Function | A Lambda function is granted more permissions than necessary, increasing risk if it is exploited. |
| 8 | [Lesson#08](Lesson%2308/README.md) | Logic Vulnerability | A timing issue between billing and order updates can lead to inconsistent or incorrect order results. |
| 9 | [Lesson#09](Lesson%2309/README.md) | Vulnerable Dependencies | Using insecure or outdated libraries may introduce serious risks such as code execution or unsafe data handling. |
| 10 | [Lesson#10](Lesson%2310/README.md) | Unhandled Exceptions | Improper error handling can expose sensitive internal details such as file paths or system information. |

---
##
DEMO link = 
## Report Format

Each lesson README is organized to show:

- the vulnerability objective and expected behavior
- the technical reason the weakness exists
- the AWS services and tools used during testing
- reproducible attack steps
- screenshots, logs, or command output as evidence
- mitigation strategy and implementation notes
- verification results after applying the fix
- final security analysis and lessons learned
