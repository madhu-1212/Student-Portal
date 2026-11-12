
# Security Risk Register – Student Portal

## 1. Introduction

This risk register identifies potential security threats affecting the fictional Student Management Web Application.

Each risk is evaluated based on:
- Likelihood: Probability of the threat occurring.
- Impact: Potential damage caused by the threat.
- Risk Score: Likelihood × Impact.

The scores are preliminary assessment estimates, not measured incident probabilities.

## 2. Risk Scoring Method

### Likelihood Scale

| Score | Description |
|---|---|
| 1 | Rare |
| 2 | Unlikely |
| 3 | Possible |
| 4 | Likely |
| 5 | Almost Certain |

### Impact Scale

| Score | Description |
|---|---|
| 1 | Negligible |
| 2 | Minor |
| 3 | Moderate |
| 4 | Major |
| 5 | Severe |

### Risk Priority

| Risk Score | Priority |
|---|---|
| 1–4 | Low |
| 5–9 | Medium |
| 10–16 | High |
| 17–25 | Critical |

## 3. Risk Register Table

| ID | Threat | STRIDE | Likelihood | Impact | Score | Priority |
|---|---|---|---:|---:|---:|---|
| R01 | Stolen student credentials | Spoofing | 4 | 5 | 20 | Critical |
| R02 | Unauthorized modification of records | Tampering | 3 | 5 | 15 | High |
| R03 | Denial of user actions | Repudiation | 3 | 3 | 9 | Medium |
| R04 | Exposure of student information | Information Disclosure | 3 | 5 | 15 | High |
| R05 | Excessive requests affecting availability | Denial of Service | 2 | 4 | 8 | Medium |
| R06 | Student gaining admin permissions | Elevation of Privilege | 3 | 5 | 15 | High |

## 4. Risk Treatment Plan

| ID | Recommended Security Control | Priority |
|---|---|---|
| R01 | Strong passwords, MFA and secure sessions | Critical |
| R02 | Server-side authorization and input validation | High |
| R03 | Secure audit logging and activity monitoring | Medium |
| R04 | HTTPS, encryption and access restrictions | High |
| R05 | Rate limiting and traffic monitoring | Medium |
| R06 | Role-Based Access Control and least privilege | High |

## 5. Risk Prioritization

### Critical Risk
R01 – Stolen credentials.

Immediate attention is required because unauthorized account access may expose confidential student information.

### High Risks
- R02 – Unauthorized record modification.
- R04 – Information disclosure.
- R06 – Privilege escalation.

These risks require strong access controls and data protection measures.

### Medium Risks
- R03 – Repudiation.
- R05 – Denial of Service.

These risks require appropriate monitoring, logging and availability controls.

## 6. Conclusion

The risk assessment identifies six major security threats in the proposed student portal.

Authentication security, data protection and access control should receive the highest attention.

Implementing the recommended defensive controls can improve the confidentiality, integrity and availability of the application.
