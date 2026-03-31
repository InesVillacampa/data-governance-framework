# Naming Conventions

> Consistent naming makes data easier to find, understand, and maintain. These conventions apply to all datasets, tables, fields, pipelines, and files in this framework.

---

## General Rules

- Use **lowercase** for all names
- Use **underscores** `_` to separate words — never spaces or hyphens in data object names
- Be **descriptive but concise** — names should be self-explanatory
- Avoid abbreviations unless they are universally understood (e.g. `id`, `url`, `api`)
- Never use reserved words (e.g. `date`, `table`, `select`, `order`)
- Use **English** for all names

---

## Databases & Schemas

| Pattern | Example |
|---------|---------|
| `[domain]` | `finance`, `hr`, `operations` |
| Schema names are singular | `customer` not `customers` |

---

## Tables & Views

| Type | Pattern | Example |
|------|---------|---------|
| Raw / source table | `raw_[source]_[entity]` | `raw_salesforce_accounts` |
| Staging table | `stg_[source]_[entity]` | `stg_salesforce_accounts` |
| Intermediate table | `int_[entity]_[transformation]` | `int_accounts_enriched` |
| Final / mart table | `[domain]_[entity]` | `finance_invoices` |
| View | `vw_[entity]` | `vw_active_customers` |
| Lookup / reference | `ref_[entity]` | `ref_country_codes` |

---

## Columns / Fields

| Type | Pattern | Example |
|------|---------|---------|
| Primary key | `id` or `[entity]_id` | `id`, `customer_id` |
| Foreign key | `[referenced_entity]_id` | `order_id`, `product_id` |
| Timestamp (created) | `created_at` | `created_at` |
| Timestamp (updated) | `updated_at` | `updated_at` |
| Timestamp (deleted) | `deleted_at` | `deleted_at` |
| Boolean flag | `is_[condition]` or `has_[condition]` | `is_active`, `has_subscription` |
| Date (not datetime) | `[context]_date` | `invoice_date`, `birth_date` |
| Amount / money | `[context]_amount` | `total_amount`, `tax_amount` |
| Count | `[context]_count` | `order_count`, `login_count` |
| Status | `[context]_status` | `payment_status`, `order_status` |

---

## Files & Documents

| Type | Pattern | Example |
|------|---------|---------|
| Policy documents | `[topic]-policy.md` | `data-access-policy.md` |
| Standards documents | `[topic]-standards.md` | `metadata-standards.md` |
| Templates | `[entity]-template.md` | `data-asset-template.md` |
| Pipeline configs | `[pipeline_name]_pipeline.yaml` | `orders_pipeline.yaml` |
| Scripts | `[action]_[target].py` | `validate_schema.py` |

---

## Pipelines & Jobs

| Pattern | Example |
|---------|---------|
| `[source]_to_[destination]` | `salesforce_to_warehouse` |
| `[domain]_[entity]_[frequency]` | `finance_invoices_daily` |

---

## Branches (Git)

| Type | Pattern | Example |
|------|---------|---------|
| New feature or document | `feat/[short-description]` | `feat/add-retention-policy` |
| Bug fix | `fix/[short-description]` | `fix/glossary-typo` |
| Documentation update | `docs/[short-description]` | `docs/update-raci-matrix` |
| Governance change | `governance/[short-description]` | `governance/access-policy-v2` |

---

## Commit Messages

Follow this format for all commits:

```
[type]: short description (max 72 characters)
```

| Type | When to use |
|------|-------------|
| `feat` | Adding a new document or policy |
| `fix` | Correcting an error |
| `docs` | Updating documentation |
| `refactor` | Restructuring without changing content |
| `chore` | Maintenance tasks (e.g. updating CHANGELOG) |

**Examples:**
```
feat: add data retention policy
fix: correct glossary definition for data lineage
docs: update RACI matrix with new engineering contact
chore: update CHANGELOG for v1.1
```

---

## ❌ Common Mistakes to Avoid

| Wrong | Right | Why |
|-------|-------|-----|
| `CustomerData` | `customer_data` | No camelCase |
| `customer-data` | `customer_data` | No hyphens in data objects |
| `cd` | `customer_data` | No unclear abbreviations |
| `data` | `finance_invoices` | Too generic |
| `tbl_customers` | `customers` | No redundant type prefixes |
| `Date` | `invoice_date` | No reserved words, be specific |

---

## Change Log

| Date | Version | Change | Author |
|------|---------|--------|--------|
| 2026-03-31 | 1.0 | Initial naming conventions | — |

---

*Stored in `standards/naming-conventions.md` | Review annually*
