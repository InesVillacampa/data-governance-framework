# Data Ownership & RACI Matrix

> This document defines who is **R**esponsible, **A**ccountable, **C**onsulted, and **I**nformed for key data governance activities across each data domain.

---

## RACI Key

| Letter | Role | Meaning |
|--------|------|---------|
| **R** | Responsible | Does the work |
| **A** | Accountable | Owns the outcome — the final decision maker |
| **C** | Consulted | Provides input before a decision is made |
| **I** | Informed | Notified after a decision is made |

> Each activity must have exactly **one A** (accountable). It may have multiple R, C, and I.

---

## Data Domain Ownership

| Domain | Data Owner | Data Steward | Engineering Contact |
|--------|------------|--------------|---------------------|
| Finance | — | — | — |
| HR / People | — | — | — |
| Operations | — | — | — |
| Customer | — | — | — |
| Legal & Compliance | — | — | — |
| Product | — | — | — |

> Fill in names or team names as your organization grows.

---

## RACI: Core Governance Activities

### Policy Management

| Activity | Governance Lead | Data Owner | Data Steward | IT / Engineering | Data User |
|----------|----------------|------------|--------------|-----------------|-----------|
| Create new policy | A/R | C | C | C | I |
| Review existing policy | A | R | C | C | I |
| Approve policy changes | A | C | I | I | I |
| Communicate policy updates | R | I | I | I | I |

---

### Data Catalog & Glossary

| Activity | Governance Lead | Data Owner | Data Steward | IT / Engineering | Data User |
|----------|----------------|------------|--------------|-----------------|-----------|
| Register new data asset | I | A | R | C | I |
| Update data asset entry | I | A | R | C | I |
| Add glossary term | I | C | R/A | I | C |
| Review catalog for accuracy | I | A | R | C | I |

---

### Data Access Management

| Activity | Governance Lead | Data Owner | Data Steward | IT / Engineering | Data User |
|----------|----------------|------------|--------------|-----------------|-----------|
| Request data access | I | C | I | I | R |
| Approve access request | I | A | C | R | I |
| Revoke access | I | A | C | R | I |
| Conduct access review | A | R | C | C | I |

---

### Data Quality

| Activity | Governance Lead | Data Owner | Data Steward | IT / Engineering | Data User |
|----------|----------------|------------|--------------|-----------------|-----------|
| Define quality rules | C | A | R | C | I |
| Monitor data quality | I | A | R | R | I |
| Report quality issue | I | I | I | I | R |
| Resolve quality issue | I | A | R | R | I |
| Escalate unresolved issue | A | R | C | C | I |

---

### Data Lineage

| Activity | Governance Lead | Data Owner | Data Steward | IT / Engineering | Data User |
|----------|----------------|------------|--------------|-----------------|-----------|
| Document pipeline lineage | I | A | C | R | I |
| Update lineage on change | I | A | C | R | I |
| Review lineage accuracy | I | A | R | C | I |

---

### Incident & Breach Response

| Activity | Governance Lead | Data Owner | Data Steward | IT / Engineering | Data User |
|----------|----------------|------------|--------------|-----------------|-----------|
| Detect and report incident | C | C | C | R | R |
| Assess severity | A | R | C | R | I |
| Contain and remediate | A | R | C | R | I |
| Notify affected parties | A/R | C | I | C | I |
| Document and close incident | A/R | C | C | C | I |

---

## Change Log

| Date | Version | Change | Author |
|------|---------|--------|--------|
| 2026-03-31 | 1.0 | Initial RACI matrix created | — |

---

*Stored in `lineage/ownership-raci.md` | Review annually or when roles change*
