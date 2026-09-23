<p align="center"><img src="logo.svg" width="96" alt="Recall logo"></p>

# Recall – Client memory for banks

Hackathon prototype for the challenge *Customer Know-How Repo / Self-Learning CRM*.

Recall turns scattered client information — account-opening documents, KYC evidence, emails, meeting notes, CRM records — into a single, trustworthy account view that a relationship manager can act on. Every statement is traceable back to the exact passage in its source, and every proposed update flows through a review workflow that respects the bank's four-eyes principle.

> All data is fictional and hard-coded. No backend, no real client data.

---

## What Recall does

- **Client overview** with today's focus, open risks, key people, and a chronological timeline
- **KYC profile** covering identity, tax status (CRS/FATCA), Form A, source of wealth and funds, screening, and suitability
- **Documents** checklist for account opening and KYC evidence, with one-click request actions
- **Conflicts & gaps** view showing where sources disagree, are outdated, or are incomplete
- **Meeting prep** with pre-generated questions and next steps
- **Learning loop**: new emails become proposed updates, reviewed by the RM and — for KYC changes — by compliance
- **Trust & controls**: source traceability, labels distinguishing verified facts from inferences, full audit trail, and clear system limits

---

## Features relevant to a bank

### Regulatory & compliance coverage
- **KYC lifecycle management** — identity verification, periodic review scheduling, and evidence tracking across the client's tenure
- **AML monitoring hooks** — surface source-of-funds alerts with linked evidence and resolution status
- **PEP screening state** — track last-screened date, re-screening cadence, and open escalations
- **CRS / FATCA** — flag US-person exposure at both client and beneficiary level, prompt W-9 handling where needed
- **UBO transparency** — beneficial-owner structures for corporate clients, including trust and family-office arrangements
- **Source of wealth attestation** — cadence tracking with automatic staleness warnings before high-value inbound transfers
- **Suitability & risk profiling** — mandate type, risk category, and reference currency captured per client

### Client intelligence
- **Unified profile per client** — individual, family, and corporate views with tier segmentation (Tier A / B / Corporate)
- **Relationship graph** — spouse, power of attorney, tax advisor, prior RM, next-generation heirs, corporate signatories
- **Contact preferences** — preferred channel (in-person, phone, paper), language, and cadence per client
- **Portfolio snapshot** — AUM, mandate type, strategy, booking centre, and structure at a glance
- **Handover memory** — captures notes from outgoing RMs so continuity is preserved when clients transfer

### Governance & audit
- **Every fact is sourced** — statements link back to the specific document, email, or meeting-note passage that supports them
- **Verified vs. inferred labels** — distinguishes what is confirmed from what the system suggests, so RMs know what to double-check
- **Four-eyes workflow** — KYC-relevant proposals require compliance review before they enter the record
- **Immutable audit trail** — who changed what, when, and based on which source
- **Explicit limits** — the system shows what it will not do (e.g. autonomous updates to KYC fields), building trust with second-line functions

### Operational efficiency
- **Meeting prep on demand** — questions, open items, and recent changes surfaced before every conversation
- **Task suggestions** — actionable next steps tied to specific KYC gaps or client requests
- **Document request actions** — trigger the request for missing evidence directly from the gap
- **Daily focus** — a single view highlighting risks and time-sensitive items across the RM's book
- **Cross-source deduplication** — the same fact stated in multiple places is consolidated, with all sources retained

### Data integration surface (conceptual)
- Account-opening documentation (Form A, mandate agreements, ID copies)
- KYC evidence (source-of-wealth letters, screening reports, tax rulings)
- Email correspondence with clients and their advisors
- CRM records and meeting notes
- Internal case-management tickets (e.g. compliance escalations)

---

## Run locally

Open `index.html` in any browser. It is a single self-contained file — React, Tailwind CSS, Framer Motion, and Lucide are bundled inline. No build step, no backend.

## Live demo

**https://razije.github.io/Recall/** (GitHub Pages)
