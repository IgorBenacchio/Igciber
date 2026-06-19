# Security by Design Framework

## Recruiter Signal

This project demonstrates security architecture judgment, risk-based prioritization, governance communication and control mapping for enterprise technology initiatives.

## Business Problem

A regulated business needs a repeatable way to review new systems before implementation, reduce late security findings and provide clear evidence for architecture, audit and executive stakeholders.

## Scenario

A fictional digital platform is being designed with web, API, identity, data and third-party integration layers. The security architecture function must help the delivery team identify risks early, define baseline controls and document decisions without exposing internal implementation details.

## Objectives

| Objective | Expected outcome |
| --- | --- |
| Identify business and technical risk | Risk register with likelihood, impact and treatment |
| Define baseline controls | Minimum security requirements for architecture review |
| Support delivery teams | Clear checklist that can be used before build and release |
| Create audit-ready evidence | Security opinion, ADR and control mapping artifacts |
| Communicate with leadership | Executive risk summary with decision options |

## Architecture Domains Covered

| Domain | Review focus |
| --- | --- |
| Identity and access | Authentication, authorization, privileged access, access reviews |
| Application security | Secure SDLC, input validation, secure logging, error handling |
| API security | OAuth2/OIDC, token handling, rate limiting, schema validation |
| Data security | Classification, encryption, retention, masking and privacy controls |
| Cloud and platform | Segmentation, logging, policy, secrets and configuration baseline |
| Third parties | Integration risk, data sharing, SLA, auditability and exit plan |
| Monitoring | Security events, alert ownership and incident response handoff |

## Risk Matrix Example

| Risk | Business impact | Likelihood | Severity | Treatment | Evidence |
| --- | --- | --- | --- | --- | --- |
| Excessive privileged access | Unauthorized change or data exposure | Medium | High | Enforce least privilege and access reviews | RBAC matrix and approval workflow |
| Missing audit logs | Reduced incident investigation capability | Medium | High | Centralize application and platform logs | Logging requirements and SIEM mapping |
| Weak API authorization | Data exposure through object-level access flaw | Medium | Critical | Add authorization tests and API gateway policies | API security checklist |
| Unclassified sensitive data | Privacy and compliance exposure | Medium | High | Classify data and define handling requirements | Data classification register |
| Untracked exceptions | Control bypass without accountability | Medium | Medium | Create exception workflow with expiry dates | Exception register |

## Control Mapping

| Control area | Example control | Framework alignment |
| --- | --- | --- |
| Governance | Security review required for material architecture changes | ISO 27001, NIST CSF Govern |
| Identity | MFA, RBAC, least privilege and periodic access review | CIS Controls, Zero Trust |
| Application | Secure coding checklist, SAST/SCA, API authorization tests | OWASP ASVS, OWASP API Top 10 |
| Data | Classification, encryption and retention requirements | ISO 27001, privacy principles |
| Monitoring | Central logs, alert ownership and incident response process | NIST CSF Detect/Respond |
| Supplier risk | Third-party security review and data sharing approval | ISO 27001 supplier controls |

## Deliverables

| Deliverable | Purpose |
| --- | --- |
| Security opinion | Summarizes risk, required controls and decision recommendation |
| Architecture decision record | Captures tradeoffs and approved security decisions |
| Risk register | Shows prioritization and treatment plan |
| Control checklist | Helps delivery teams validate readiness |
| Executive summary | Translates security concerns into business impact |

## Validation Checklist

- Business problem is stated before tools or controls.
- Risks are prioritized by impact and likelihood.
- Controls are mapped to recognized frameworks.
- Decisions are documented with owners and next steps.
- Exceptions have justification, expiry and compensating controls.
- Content is sanitized and does not reveal employer-specific information.

## Interview Talking Points

| Question | Strong answer signal |
| --- | --- |
| How do you avoid blocking delivery? | Use risk-based prioritization, minimum viable controls and documented exceptions |
| How do you communicate risk to executives? | Convert technical weaknesses into business impact, options and decision points |
| How do you prove architecture maturity? | Show repeatable review flow, control mapping and evidence artifacts |
| How do you handle exceptions? | Require owner, reason, expiry, compensating controls and review cadence |

## Public Safety Statement

This is a defensive and fictionalized project. It contains no real credentials, real IP addresses, internal diagrams, confidential architecture or offensive instructions.
