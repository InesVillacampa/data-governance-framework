# Data Asset Template

> Use this template when registering a new data asset in the catalog. Copy this file, fill in all sections, and save it under `data-catalog/domains/[your-domain]/[asset-name].md`.

---

## Asset Overview

| Field | Value |
|-------|-------|
| **Asset Name** | *(e.g. customer_transactions)* |
| **Domain** | *(e.g. Finance / HR / Operations / Customer)* |
| **Asset Type** | *(Table / View / Report / API / Feed / Dashboard)* |
| **Classification** | *(Public / Internal / Confidential / Restricted)* |
| **Status** | *(Active / Deprecated / In Review)* |
| **Created Date** | *(YYYY-MM-DD)* |
| **Last Updated** | *(YYYY-MM-DD)* |

---

## Ownership

| Role | Name / Team |
|------|-------------|
| **Data Owner** | *(Team or individual accountable for this asset)* |
| **Data Steward** | *(Person responsible for day-to-day management)* |
| **Engineering Contact** | *(Team or person who maintains the pipeline/system)* |

---

## Description

*(Write a plain-language description of what this data asset is, what it represents, and what it is used for. 2–4 sentences.)*

---

## Source System

| Field | Value |
|-------|-------|
| **Source System Name** | *(e.g. Salesforce, PostgreSQL, SAP)* |
| **Source Type** | *(Database / API / File / Stream / Manual)* |
| **Source Location** | *(e.g. db.prod.company.com/schema/table)* |
| **Ingestion Method** | *(e.g. daily ETL, real-time stream, manual upload)* |

---

## Schema

List the key fields in this data asset:

| Field Name | Data Type | Description | PII? | Required? |
|------------|-----------|-------------|------|-----------|
| `id` | `string` | Unique identifier | No | Yes |
| `created_at` | `timestamp` | Record creation time | No | Yes |
| *(add more rows)* | | | | |

> For full schema details, see [schema-registry.yaml](../../schema-registry.yaml)

---

## Data Quality

| Rule | Description | Threshold |
|------|-------------|-----------|
| **Completeness** | % of required fields that are non-null | ≥ 99% |
| **Freshness** | Maximum acceptable age of data | *(e.g. 24 hours)* |
| **Uniqueness** | No duplicate records on primary key | 100% |
| **Validity** | Values conform to expected format/range | *(define per field)* |

---

## Access & Usage

| Field | Value |
|-------|-------|
| **Who can access** | *(e.g. Data Analysts, Finance Team, All Internal)* |
| **How to request access** | *(e.g. submit request via [data-access-policy.md](../../policies/data-access-policy.md))* |
| **Usage restrictions** | *(e.g. not to be used for marketing without approval)* |
| **Retention period** | *(e.g. 7 years — see [data-retention-policy.md](../../policies/data-retention-policy.md))* |

---

## SLA

| Metric | Commitment |
|--------|------------|
| **Refresh frequency** | *(e.g. Daily at 6:00 AM UTC)* |
| **Availability** | *(e.g. 99.9% uptime)* |
| **Issue response time** | *(e.g. critical issues resolved within 4 hours)* |

---

## Lineage

| Direction | Asset / System |
|-----------|---------------|
| **Upstream (sources)** | *(What feeds into this asset?)* |
| **Downstream (consumers)** | *(What depends on this asset?)* |

> For full lineage diagram, see [lineage/pipeline-maps/](../../lineage/pipeline-maps/)

---

## Change Log

| Date | Version | Change | Author |
|------|---------|--------|--------|
| *(YYYY-MM-DD)* | 1.0 | Initial registration | *(name)* |

---

## Notes

*(Any additional context, known issues, or important caveats about this data asset.)*

---

*Template version: 1.0 | Stored in `data-catalog/data-asset-template.md`*
