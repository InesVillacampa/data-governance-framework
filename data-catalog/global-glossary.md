# Global Data Glossary

> A shared vocabulary for all data terms used across this framework. Consistent definitions reduce confusion and improve communication between technical and non-technical stakeholders.

**How to use this glossary:**
- Before creating a new term, check if it already exists here
- To add or update a term, submit a Pull Request following [CONTRIBUTING.md](../CONTRIBUTING.md)
- Terms are listed alphabetically within each category

---

## A

**Data Asset**
Any data object that has value to the organization — including datasets, tables, reports, dashboards, APIs, or data feeds. Every data asset should be registered in the [data catalog](../data-catalog/).

**Data Audit**
A systematic review of data assets to verify accuracy, completeness, and compliance with governance policies.

**Access Control**
The process of granting or restricting access to data based on a user's role, responsibilities, and the data's classification level.

---

## C

**Catalog (Data Catalog)**
A centralized inventory of all data assets, including metadata, ownership, classification, and lineage information. See [data-catalog/](../data-catalog/).

**Classification (Data Classification)**
The process of categorizing data by its sensitivity level — Public, Internal, Confidential, or Restricted. See [data-classification.md](../policies/data-classification.md).

**Compliance**
Adherence to applicable laws, regulations, and internal policies governing how data is collected, stored, used, and shared.

**Confidential Data**
Data restricted to authorized personnel only. Examples include employee records and financial data. See [data-classification.md](../policies/data-classification.md).

---

## D

**Data Domain**
A logical grouping of related data assets managed by a specific team or business unit. Examples: Finance, HR, Operations, Customer.

**Data Governance**
The set of policies, standards, roles, and processes that ensure data is accurate, secure, consistent, and used appropriately across an organization.

**Data Lineage**
A record of where data comes from, how it moves through systems, and how it is transformed over time. See [lineage/](../lineage/).

**Data Owner**
The individual or team accountable for a specific data domain or dataset. Responsible for quality, access decisions, and lifecycle management.

**Data Quality**
The degree to which data meets defined standards of accuracy, completeness, consistency, timeliness, and validity. See [data-quality-rules.md](../standards/data-quality-rules.md).

**Data Steward**
The person responsible for the day-to-day management of a data asset — maintaining catalog entries, monitoring quality, and acting as a point of contact for data users.

**Data User**
Any individual or system that accesses and consumes data assets. Data users must comply with applicable access and usage policies.

---

## G

**Governance Committee**
The group of stakeholders responsible for reviewing governance policies, resolving escalated issues, and ensuring the framework remains current and effective.

**Glossary**
A defined list of business and technical terms with agreed-upon meanings. This document is the master glossary for the framework.

---

## M

**Metadata**
Data that describes other data. Examples include a dataset's name, owner, creation date, source system, and schema. Metadata is stored in the [data catalog](../data-catalog/).

---

## P

**Personal Data (PII)**
Any information that can identify a specific individual — such as name, email address, phone number, or government ID. Subject to strict handling requirements under GDPR, CCPA, and similar regulations.

**Pipeline**
An automated process that moves, transforms, or loads data from one system to another. Pipelines are documented in [lineage/pipeline-maps/](../lineage/pipeline-maps/).

**Policy**
A formal document that defines rules and requirements for how data must be handled in a specific area (e.g. access, retention, classification). Policies are stored in [policies/](../policies/).

**Public Data**
Data that is safe to share openly with no access restrictions. Examples include published reports and public documentation.

---

## R

**RACI**
A framework for defining roles and responsibilities: **R**esponsible, **A**ccountable, **C**onsulted, **I**nformed. Used in [ownership-raci.md](../lineage/ownership-raci.md) to clarify who owns each data domain.

**Retention (Data Retention)**
The policy defining how long data is stored before it is archived or deleted. See [data-retention-policy.md](../policies/data-retention-policy.md).

**Restricted Data**
The most sensitive classification tier — tightly controlled data such as legal documents or PII. Requires explicit authorization to access.

---

## S

**Schema**
The structure of a dataset — including field names, data types, and relationships. Schemas are registered in [schema-registry.yaml](../data-catalog/schema-registry.yaml).

**SLA (Service Level Agreement)**
A documented commitment about data availability, freshness, or quality — e.g. "this dataset is refreshed daily by 6am." See [SLA-templates.md](../standards/SLA-templates.md).

**Source System**
The originating system where data is first created or captured. Documented in [source-systems.md](../lineage/source-systems.md).

**Standard**
A documented rule or convention that defines how something must be done — such as how datasets are named or how metadata is structured. Standards are stored in [standards/](../standards/).

---

## T

**Taxonomy**
A hierarchical classification system for organizing data domains, categories, or terms consistently across the organization.

---

## V

**Version Control**
The practice of tracking changes to documents and files over time using a system like Git. All governance documents in this repository are version controlled.

---

## Contributing a New Term

To propose a new glossary term:
1. Check that the term doesn't already exist
2. Use this format:

```
**Term Name**
A clear, plain-language definition. Include links to related policies or documents where relevant.
```

3. Submit a Pull Request with the label `glossary`

---

*Last updated: 2026-03-31 | Maintained in `data-catalog/global-glossary.md`*
