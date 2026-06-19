# Secure Azure Landing Zone

## Recruiter Signal

This project demonstrates cloud security architecture, IAM governance, platform baseline controls, logging, policy management and risk-based cloud adoption.

## Business Problem

A company wants to adopt cloud services while maintaining consistent identity, network, logging, data protection and governance controls across workloads.

## Scenario

A fictional enterprise is creating a secure Azure foundation for application teams. The platform must support business agility while enforcing minimum security and compliance expectations.

## Objectives

| Objective | Expected outcome |
| --- | --- |
| Establish cloud governance | Subscription structure, ownership and policy baseline |
| Secure identity | RBAC, privileged access model and access review process |
| Protect workloads | Network segmentation, private access patterns and secure configuration |
| Enable detection | Centralized logs, alert routing and monitoring ownership |
| Support audit readiness | Evidence model for cloud controls and exceptions |

## Landing Zone Components

| Component | Security purpose |
| --- | --- |
| Management group structure | Separates production, non-production and sandbox governance |
| Subscription model | Aligns workload ownership, cost accountability and risk boundaries |
| RBAC baseline | Enforces least privilege and role separation |
| Conditional Access | Reduces identity risk for users and administrators |
| Network segmentation | Limits lateral movement and separates trust zones |
| Key management | Protects secrets, certificates and encryption keys |
| Policy baseline | Prevents insecure resources and configuration drift |
| Logging and monitoring | Enables detection, investigation and operational visibility |

## Reference Control Baseline

| Area | Baseline control | Evidence |
| --- | --- | --- |
| Identity | MFA for privileged users, just-in-time admin access and access reviews | IAM matrix and review log |
| RBAC | Role assignments must have owner, reason and expiry for elevated access | RBAC register |
| Network | Production workloads use segmented networks and controlled ingress | Network control checklist |
| Secrets | Secrets stored in managed vaults and never in code repositories | Secrets handling standard |
| Logging | Activity logs, identity logs and workload security logs are centralized | Logging coverage matrix |
| Policy | Deny or audit insecure public exposure and missing tags | Policy assignment list |
| Exceptions | Exceptions require risk acceptance, expiry date and compensating controls | Exception register |

## IAM Matrix Example

| Role | Scope | Access type | Review cadence | Notes |
| --- | --- | --- | --- | --- |
| Cloud Platform Owner | Management group | Administrative | Quarterly | Break-glass excluded from daily use |
| Security Reader | Tenant and subscriptions | Read-only security visibility | Quarterly | Used for monitoring and audit |
| Workload Owner | Application subscription | Contributor within workload boundary | Quarterly | No tenant-wide privileges |
| Deployment Pipeline | Resource group | Automated deployment permissions | Monthly | Managed identity preferred |
| Auditor | Evidence workspace | Read-only | Semiannual | No production change rights |

## Logging and Monitoring Plan

| Signal | Purpose | Owner |
| --- | --- | --- |
| Privileged role assignment | Detect elevated access changes | Cloud security |
| Public endpoint creation | Detect internet exposure | Platform team |
| Key vault access anomaly | Detect suspicious secret access | Security operations |
| Policy non-compliance | Track drift from baseline | Governance team |
| Failed privileged login | Detect identity attack attempts | SOC |

## Deliverables

| Deliverable | Purpose |
| --- | --- |
| Landing zone security blueprint | Shows target-state foundation and security decisions |
| RBAC and access review model | Demonstrates identity governance and least privilege |
| Policy baseline | Demonstrates preventive and detective cloud controls |
| Logging matrix | Shows detection coverage and ownership |
| Exception workflow | Shows pragmatic governance for delivery teams |

## Validation Checklist

- Cloud security is connected to identity, network, logging and governance.
- Roles and responsibilities are clear.
- Privileged access is controlled and periodically reviewed.
- Monitoring signals have owners and response expectations.
- Exceptions are documented and time-bound.
- Examples are generic and safe for public review.

## Interview Talking Points

| Question | Strong answer signal |
| --- | --- |
| How do you start a secure landing zone? | Define governance, identity, logging, network and policy before workload migration |
| How do you avoid excessive permissions? | Use RBAC, PIM/JIT concepts, access reviews and scoped managed identities |
| How do you prove cloud control maturity? | Maintain policy assignments, logs, exception register and evidence dashboards |
| How do you balance cloud agility and control? | Provide reusable baseline patterns and documented exception paths |

## Public Safety Statement

This is a defensive and fictionalized project. It contains no tenant identifiers, real subscriptions, private IPs, credentials or employer-specific architecture.
