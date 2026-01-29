# Project Roadmap

This project evolves as an **Azure Governance & Guardrails Platform** that is focused on **identity-first security, policy-as-code, and secure-by-default Azure foundations**.

The roadmap prioritizes **preventive platform controls** over reactive monitoring
and it is designed to demonstrate mastery of Azure governance, identity, and policy
enforcement at scale.

---

## v1 – Governance Foundation (Current Focus)

Establish a secure Azure foundation with clear ownership, boundaries, and standards.

**Scope**

- Management group hierarchy design
- Subscription segmentation (prod / non-prod / shared services)
- Naming and tagging standards
- Identity boundary definition (tenant vs subscription)
- RBAC baseline (least privilege)
- Privileged Identity Management (PIM) model
- Governance architecture documentation and diagrams

**Outcome**

- Secure-by-default Azure structure
- Clear platform ownership and trust boundaries

---

## v2 – Guardrails as Code

Implement enforceable Azure guardrails using policy-as-code.

**Scope**

- Azure Policy definitions (built-in and custom)
- Policy initiatives for baseline controls:
  - tagging and ownership
  - allowed regions and SKUs
  - diagnostic settings
  - encryption and secure transfer where applicable
- Policy assignments at management group scope
- Audit → enforce rollout strategy
- Policy exemptions with documented justification

**Outcome**

- Preventive controls that reduce misconfiguration risk
- Consistent standards enforced across subscriptions

---

## v3 – Governance Automation & Compliance Evidence

Operationalize governance using infrastructure as code and evidence generation.

**Scope**

- Terraform or Bicep deployment of:
  - management groups
  - policy initiatives and assignments
  - role assignments
- Compliance posture measurement via policy states
- Defender for Cloud posture management (CSPM, not alerting)
- Evidence artifacts for audit and review

**Outcome**

- Repeatable, reviewable governance deployments
- Measurable compliance and reduced configuration drift

---

## v4 – Platform CI/CD & Change Management

Introduce controlled change workflows for governance at scale.

**Scope**

- CI pipelines for IaC validation and policy checks
- Pull request–based governance changes
- Environment promotion (dev → prod guardrails)
- Change history and approval workflows

**Outcome**

- Safe, auditable evolution of Azure guardrails
- Governance treated as a product, not a one-time setup

---

## Validation Philosophy

Telemetry and validation activities are used **only to confirm control effectiveness** such as policy enforcement, identity restrictions. They are not intended to represent SOC operations or continuous alert monitoring.
