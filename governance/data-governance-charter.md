# Data Governance Charter

> **Version:** 1.0  
> **Status:** Active  
> **Last Updated:** 2026-03-31  

---

## 1. Purpose

This Data Governance Charter establishes the foundation for how data is managed, protected, and used within this framework. It defines the principles, responsibilities, and structures that ensure data is treated as a valuable, trusted, and well-managed asset.

This charter exists to:
- Create a shared understanding of data governance across all stakeholders
- Define clear accountability for data ownership and stewardship
- Establish the rules and standards that govern how data is handled
- Enable consistent, high-quality, and compliant use of data

---

## 2. Scope

This framework applies to:
- All data assets created, collected, stored, or processed
- All teams and individuals who access or work with data
- All systems, tools, and platforms that store or transmit data

---

## 3. Governing Principles

All data governance decisions and practices are guided by the following principles:

| Principle | Description |
|-----------|-------------|
| **Accountability** | Every data asset has a named owner who is responsible for its quality, access, and lifecycle |
| **Transparency** | Data policies, definitions, and decisions are documented, versioned, and accessible to all stakeholders |
| **Integrity** | Data is accurate, consistent, and trustworthy across all systems and uses |
| **Security** | Data is classified by sensitivity and protected accordingly, with access granted on a need-to-know basis |
| **Compliance** | Data handling follows applicable laws, regulations, and contractual obligations |
| **Usability** | Data is well-documented and discoverable so that authorized users can find and use it effectively |

---

## 4. Roles and Responsibilities

### 4.1 Data Governance Lead
- Owns and maintains this charter and all governance documentation
- Chairs governance reviews and resolves escalated issues
- Ensures alignment between governance policies and organizational goals

### 4.2 Data Owners
- Accountable for specific data domains (e.g. finance, operations, customer)
- Approve access requests for their data domain
- Ensure data quality standards are met within their domain
- Review and sign off on any changes to policies affecting their data

### 4.3 Data Stewards
- Responsible for day-to-day management of data assets
- Maintain the data catalog entries, glossary terms, and lineage documentation
- Monitor data quality and escalate issues to the Data Owner

### 4.4 Data Users
- Consume data in accordance with approved policies and standards
- Report data quality issues to the relevant Data Steward
- Complete required training before accessing sensitive data

### 4.5 IT / Engineering
- Implement and maintain the technical controls that enforce governance policies
- Ensure systems meet security and compliance requirements
- Support data lineage tracking and catalog integrations

---

## 5. Governance Structure

### 5.1 Decision Making
- **Routine decisions** (e.g. adding glossary terms, updating templates) — made by Data Stewards
- **Policy changes** — require review and approval by the Data Governance Lead
- **Escalated issues** (e.g. data breaches, access disputes) — escalated to senior leadership

### 5.2 Review Cadence
| Review Type | Frequency |
|-------------|-----------|
| Policy review | Annually |
| Data catalog review | Quarterly |
| Governance committee meeting | Monthly |
| Charter review | Annually or after major changes |

---

## 6. Data Classification

All data assets must be classified into one of the following tiers:

| Classification | Description | Example |
|---------------|-------------|---------|
| **Public** | Safe to share openly | Published reports, public documentation |
| **Internal** | For internal use only | Internal policies, process documents |
| **Confidential** | Restricted to authorized personnel | Employee records, financial data |
| **Restricted** | Highly sensitive, tightly controlled | Legal documents, personal identifiable information (PII) |

Full classification rules are defined in [data-classification.md](../policies/data-classification.md).

---

## 7. Policy Framework

This charter is supported by the following policies and standards:

| Document | Purpose |
|----------|---------|
| [Data Access Policy](../policies/data-access-policy.md) | Who can access what data and under what conditions |
| [Data Retention Policy](../policies/data-retention-policy.md) | How long data is kept and when it is deleted |
| [Data Classification Policy](../policies/data-classification.md) | How data is categorized by sensitivity |
| [Privacy Policy](../policies/privacy-policy.md) | How personal data is handled and protected |
| [Naming Conventions](../standards/naming-conventions.md) | Standards for naming datasets, fields, and pipelines |
| [Data Quality Rules](../standards/data-quality-rules.md) | Rules that define acceptable data quality thresholds |

---

## 8. Compliance and Legal Alignment

This framework is designed to align with common data protection regulations and best practices, including:

- **GDPR** — General Data Protection Regulation (EU)
- **CCPA** — California Consumer Privacy Act (US)
- **HIPAA** — Health Insurance Portability and Accountability Act (where applicable)
- **SOC 2** — Service Organization Control (where applicable)

As a lawyer-maintained framework, legal interpretation of these regulations should be sought before implementing in a regulated environment.

---

## 9. Enforcement

Failure to comply with this governance framework may result in:
- Revocation of data access privileges
- Escalation to management or legal counsel
- Remediation actions as defined by applicable policies

---

## 10. Charter Amendments

This charter may be amended at any time. All changes must be:
1. Documented with a version number and date
2. Reviewed by relevant stakeholders
3. Communicated to all affected parties
4. Reflected in the [CHANGELOG.md](../CHANGELOG.md)

---

## 11. Approval

| Role | Name | Date |
|------|------|------|
| Data Governance Lead | — | — |
| Reviewed by | — | — |

---

*This charter is maintained as a living document in the `data-governance-framework` repository.*
