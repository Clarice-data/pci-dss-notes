# PCI-DSS Compliance Notes

Real-world compliance analysis from an active consulting engagement with a small healthcare practice. Documents the discovery, analysis, and remediation of PCI-DSS gaps across payment processing systems, staff access controls, and legacy cardholder data.

## Project Overview

**Role:** Compliance analyst (independent)  
**Setting:** Small healthcare practice using cloud-based practice management and payment software  
**Scope:** PCI-DSS gap assessment and remediation across four identified findings  
**Status:** Phase 2 — remediation in progress

all client-identifying information has been removed.

## what's here

### [overview.md](overview.md)
what PCI-DSS is, why it matters for small businesses, and a plain-language
summary of the remediation process.

### [gap-analysis-notes.md](gap-analysis-notes.md)
the categories of gaps identified and how they were prioritized.
no specific system names or client data included.

### [remediation-process.md](remediation-process.md)
the steps taken to move from non-compliant to compliant, including
vendor coordination, documentation requirements, and timeline.

## what i learned
- compliance work is fundamentally about documentation and process, not just technology
- small businesses often fail audits due to gaps in policy, not just technical controls
- communicating requirements to non-technical stakeholders is its own skill
## The Four Findings

### Finding 1 — Phone Call Recordings Containing Card Data
Verbal card payments taken over potentially recorded phone lines created unintended PCI scope. Remediation path: transition to text-to-pay, identify and purge historical recordings containing cardholder data.

Key considerations: recording consent disclosure (FL Stat. § 934.03), vendor deletion process, written deletion confirmation as evidence of remediation.

### Finding 2 — Legacy Cardholder Data Across System Migrations
Historical card data remained in free-text fields following two practice management system migrations. Discovery approach: custom SQL queries across financial notes, communication logs, and procedure notes — 1,000+ records identified for review. Remediation requires admin-level access to execute deletions systematically.

Key considerations: scoping legacy data correctly, working within vendor constraints, using database queries as a discovery tool.

### Finding 3 — SAQ Form Selection
To be completed after all active remediation is finished. Likely path: SAQ A if text-to-pay only; SAQ C-VT if staff manually enter card data into a payment dashboard. Final determination to be confirmed with QSA.

### Finding 4 — Shared Staff Login Credentials
A shared email account was in use across multiple staff members for a cloud-based phone and payments platform — a violation of PCI DSS Req. 8.2.1 (unique IDs per user). Remediation: individual accounts provisioned for all staff; shared account retired.

**Finding 4 addendum — coverage account exception:** A limited-access shared account was later approved as an operational exception for front desk coverage. Documented as compliant because payment roles were fully excluded and account access is administrator-controlled.

---

## Skills Demonstrated

- PCI-DSS requirements interpretation and gap analysis
- SQL-based cardholder data discovery
- Risk prioritization across multiple concurrent findings
- Vendor coordination (payment processor, practice management, telephony)
- Stakeholder communication with non-technical decision makers
- Compliance documentation and evidence management

---

## Notes on Data

All documentation in this repo is sanitized. No client names, patient data, staff information, or credentials are included. SQL queries reference field structures only — no live data.

---

## Background

This project draws on experience in healthcare practice operations, including familiarity with HIPAA data handling standards, practice management systems, and payment processing workflows. The compliance analysis work builds directly on that operational background.

---

*Part of an ongoing data analytics and compliance portfolio.*
---
*this is a learning document. it reflects my experience coordinating a real engagement,
not a complete technical security guide.*
