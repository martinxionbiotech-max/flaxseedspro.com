# Traceability & Recall Program

## Document Control

| Field | Value |
|---|---|
| Document ID | FS-TRC-001 |
| Version | 3.0 |
| Effective Date | 2026-01-20 |
| Owner | Traceability & Recall Coordinator |
| Approver | Food Safety Team Leader |
| Review Frequency | Annual |

---

## 1. Traceability System Description

### 1.1 Objective
The traceability system enables the company to trace any finished product **one step back** (to raw material supplier) and **one step forward** (to customer) within 4 hours of a request. This meets the requirements of:
- EU Regulation (EC) 178/2002 (General Food Law — Article 18)
- Codex Alimentarius CXG 60-2006 (Principles for Traceability)
- BRCGS Food Safety Issue 9 (Clause 5.8)
- FSSC 22000 (ISO 22000 — Clause 12.1)

### 1.2 Lot Numbering System

#### 1.2.1 Raw Material Lot Numbers (Incoming)
```
RR-YYYYMMDD-SSSS
│  │         │
│  │         └── Supplier batch/serial number (last 4 digits)
│  └──────────── Receiving date (YYYYMMDD)
└─────────────── Material code (2-letter: FL=Flax, SE=Sesame, MU=Mustard,
                 CE=Celery, SO=Soy, PL=Packaging, AD=Additive)
```
*Example:* `FL-20260715-1023` = Flaxseed received 15 July 2026, supplier batch ending 1023.

#### 1.2.2 Production / In-Process Lot Numbers
```
PR-A-YYYYMMDD-HHMM-SSS
│ │           │    │
│ │           │    └── Sequential batch number (001–999)
│ │           └─────── Timestamp of first production (HHMM)
│ └─────────────────── Line designation (A, B, C)
└───────────────────── Prefix "PR" (Production)
```
*Example:* `PR-A-20260715-0830-042` = Line A, 15 July 2026, started 08:30, batch 042.

#### 1.2.3 Finished Product Lot Numbers
```
FP-CCYYMMDD-BB-PP
│  │        │  │
│  │        │  └── Pack configuration code (e.g., 01=25kg bag, 02=500g retail)
│  │        └───── Production batch sequence (01–99)
│  └────────────── Packaging date (CCYYMMDD)
└───────────────── Prefix "FP" (Finished Product)
```
*Example:* `FP-20260715-42-01` = Finished product packed 15 July 2026, batch 42, 25 kg bag.

#### 1.2.4 Customer / Pallet Labels
Each pallet label includes:
- Finished product lot number
- Pallet number (001–999 per lot)
- Gross / net weight
- Production date
- Best-before / expiry date
- Product description and SKU
- Customer PO number (if applicable)

### 1.3 Traceability Chain: Raw Material → Process → Finished Product → Customer

```
Supplier ──→ Receiving ──→ Storage ──→ Production ──→ Packing ──→ Finished Goods ──→ Customer
    │            │            │             │              │             │               │
    │            │            │             │              │             │               │
    └──── LOT ───┘            │             │              │             │               │
         (RR-...)             │             │              │             │               │
                              │             │              │             │               │
                         Storage Lot    Production Lot ───┘         Finished Lot ────────┘
                         (internal)     (PR-...)                   (FP-...)           Despatch
                                                                                    Record
```

### 1.4 Data Recording Points

| Traceability Point | Data Captured | System |
|---|---|---|
| Supplier delivery | Supplier name, lot, quantity, receipt date, COA | ERP (lot-enabled) |
| Raw material storage | Material lot, storage location, put-away date/time | WMS |
| Production issue | Material lot, quantity, production order, line, time | ERP / Production Log |
| Processing step | Time stamps, line parameters (temp, pressure, speed) | SCADA / Process Log |
| Rework addition | Rework lot, quantity, target product lot | Rework Log (FS-ALC-F04) |
| Packaging | Finished product lot, packaging material lot, label lot | ERP / Packaging Log |
| Finished goods storage | Pallet number, location, storage condition checks | WMS |
| Customer despatch | Customer name, despatch date, lot numbers, quantity, vehicle | ERP / Despatch Log |

---

## 2. One-Step-Back Tracing

### 2.1 Procedure
Upon request (mock recall or actual incident), the traceability team traces **from a finished product lot back to all raw material lots** used in production.

### 2.2 Steps

| Step | Action | Time Target | Responsible |
|---|---|---|---|
| 1 | Identify finished product lot(s) in question | Immediate | Recall Coordinator |
| 2 | Retrieve production batch record for that product lot | 15 min | QA / Production |
| 3 | Extract all raw material lots issued to that production order | 15 min | QA |
| 4 | Retrieve receiving records for each raw material lot | 15 min | Procurement / QA |
| 5 | Identify supplier, supplier lot number, quantity received, date | 10 min | Procurement |
| 6 | Obtain supplier COA and allergen declaration for each lot | 20 min | QA / Procurement |
| 7 | Compile traceability report (FS-TRC-F01) | 15 min | Traceability Coordinator |
| 8 | Review and validate report | 10 min | QA Manager |
| **Total target** | | **≤ 100 min** | |

### 2.3 Data Sources
- **ERP System**: Production orders, material movements, goods receipt records.
- **Paper Logs**: Production batch record (signed), receiving log (signed).
- **WMS**: Storage locations, lot transfers.
- **SCADA**: Process parameters (for lot confirmation).

---

## 3. One-Step-Forward Tracing

### 3.1 Procedure
From a specific raw material lot or finished product lot, identify all customers who received product containing that lot.

### 3.2 Steps

| Step | Action | Time Target | Responsible |
|---|---|---|---|
| 1 | Identify subject lot (raw material or finished product) | Immediate | Recall Coordinator |
| 2 | Search ERP for all production orders using that raw material lot (if starting from raw material) | 20 min | QA |
| 3 | Identify all finished product lots produced | 15 min | QA |
| 4 | Search despatch records for all pallets / orders of those finished product lots | 20 min | Logistics |
| 5 | Identify customers, quantities, despatch dates, delivery addresses | 15 min | Logistics |
| 6 | Compile outbound traceability report (FS-TRC-F02) | 15 min | QA |
| 7 | Review and validate report | 10 min | QA Manager |
| **Total target** | | **≤ 95 min** | |

### 3.3 Data Sources
- **ERP**: Sales orders, despatch notes, delivery notes.
- **Logistics Records**: Vehicle loading sheets, customer signature proof-of-delivery.
- **WMS**: Outbound pallet movements, picking records.

---

## 4. Mock Recall Procedure

### 4.1 Requirement
A mock recall / traceability exercise must be completed **at least once per calendar year**. The exercise must be passed within **4 hours** from initiation to completion.

### 4.2 Success Criteria
- Finished product → all raw materials: **100% traced within 4 hours**.
- Raw material → all finished products → customers: **100% traced within 4 hours**.
- Mass balance: documented yield reconciliation (inputs vs outputs within ±2%).
- No "dead ends" where traceability data is missing or unrecoverable.

### 4.3 Mock Recall Process

| Phase | Activity | Timeline |
|---|---|---|
| **Initiation** | Food Safety Team Leader selects a random finished product lot from the past 6 months. | T = 0 |
| **Notification** | Recall Coordinator is notified of the mock recall scope. Traceability team assembles. | T + 10 min |
| **One-Step-Back** | Trace raw material lots, supplier lots, receiving records. | T + 0 → T + 100 min |
| **One-Step-Forward** | Trace all customers, quantities, despatch dates. | T + 0 → T + 95 min (parallel) |
| **Mass Balance** | Compare raw material input quantity vs finished product output quantity + waste. | T + 100 → T + 180 min |
| **Report Compilation** | Complete traceability report forms (FS-TRC-F01, FS-TRC-F02). | T + 180 → T + 210 min |
| **Review & Scoring** | QA Manager reviews completeness, accuracy, time. Score assigned. | T + 210 → T + 240 min |
| **Debrief** | Team reviews findings, identifies gaps, assigns corrective actions. | T + 240 → T + 270 min |

### 4.4 Scoring

| Criterion | Weight | Target | Points |
|---|---|---|---|
| Time to complete | 25% | < 4 hours | 25 (pro-rated if > 4h) |
| Raw material trace completeness | 30% | 100% of lots traced | 30 |
| Customer trace completeness | 30% | 100% of customers traced | 30 |
| Mass balance accuracy | 15% | Within ±2% | 15 |
| **Total** | **100%** | **Pass ≥ 85%** | **100** |

### 4.5 Corrective Action on Failure
If the mock recall score is below 85% or exceeds 4 hours:
1. Root cause analysis within 5 working days.
2. Formal CAPA plan within 10 working days.
3. Gap closure within 30 days.
4. Repeat mock recall within 60 days covering the gap area.

---

## 5. Recall Plan

### 5.1 Recall Team & Contact Tree

| Role | Name (Primary) | Name (Deputy) | Responsibility |
|---|---|---|---|
| Recall Coordinator | Food Safety Team Leader | QA Manager | Overall recall management, decisions, regulatory liaison |
| Communications Lead | Marketing Director | Sales Director | Media, customer notifications, consumer enquiries |
| Logistics Lead | Logistics Manager | Warehouse Supervisor | Product location, physical retrieval, quarantine |
| Technical Lead | QA Manager | QA Supervisor | Investigation, root cause, corrective action |
| Legal Counsel | External Legal Advisor | — | Legal advice, liability assessment |
| Regulatory Affairs | Regulatory Manager | Food Safety Team Leader | Notify competent authorities (FSAI, FSS, RASFF, etc.) |
| Finance Lead | Finance Director | — | Cost tracking, insurance claims |

### 5.2 Recall Decision Tree

```
1. Consumer complaint / test result / regulatory alert received
    │
    ├── Is the issue a food safety hazard? (physical, chemical, biological, allergen)
    │       │
    │       ├── YES ──> 2
    │       └── NO  ──> Monitor / routine CAPA (not a recall)
    │
2. Is the product already on the market?
    │
    ├── NO  ──> Withhold / destroy at facility (no recall needed)
    └── YES ──> 3
    │
3. Has product reached consumers?
    │
    ├── NO (still at distributor/retailer) ──> Trade recall (withdraw from trade)
    └── YES (consumer level) ──> Consumer recall (public notification required)
    │
4. Determine recall class:
    ├── Class I: Reasonable probability of serious adverse health consequences or death
    │            ──> Full public recall, RASFF alert, press release
    ├── Class II: May cause temporary / medically reversible health consequences
    │            ──> Trade recall, regulatory notification
    └── Class III: Not likely to cause adverse health consequences (e.g., labelling)
                 ──> Corrective action at trade level
    │
5. Authorise recall: Recall Coordinator + CEO
    │
6. Execute recall per communication plan.
```

### 5.3 Communication Tree

```
Recall Coordinator (activates tree)
    │
    ├── Regulatory Authorities
    │       └── FSAI / FSS / RASFF / Local EHOs
    │
    ├── Internal
    │       ├── CEO
    │       ├── Food Safety Team
    │       ├── QA Manager
    │       ├── Production Manager
    │       ├── Sales / Customer Service
    │       └── Legal Counsel
    │
    ├── External (Trade)
    │       ├── Distributors (phone + email)
    │       ├── Retailers (phone + email + formal recall notice)
    │       └── Food service operators (phone + email)
    │
    └── External (Consumer)
            └── Press release / website / social media / consumer helpline
```

### 5.4 Media / Press Release Template
A pre-approved press release template is maintained in the Recall Plan folder (FS-TRC-F03). Key elements:
- Product name, pack size, lot codes, best-before dates
- Reason for recall (clear description of hazard)
- Actions consumers should take (do not consume, return to point of purchase for refund)
- Consumer helpline number and operating hours
- Date of issue and recall authority reference number

### 5.5 Regulatory Notification Timelines

| Jurisdiction | Class I Notification | Class II Notification | Communication Channel |
|---|---|---|---|
| EU (RASFF) | Within 48 hours | Within 48 hours | RASFF portal + competent authority |
| UK (FSA) | Within 24 hours | Within 48 hours | Food Alert system |
| Ireland (FSAI) | Within 24 hours | Within 48 hours | FSAI portal |
| Codex (international) | Within 48 hours (INFOSAN) | Within 48 hours | INFOSAN network |

### 5.6 Recall Effectiveness Check
- Target: ≥ 95% of affected product recovered.
- Methods: Customer confirmation (phone/email), returned stock count, distributor inventory reconciliation.
- Effectiveness check documented within 14 days of recall initiation.

---

## 6. Product Identification (Lot Codes)

### 6.1 Lot Code Formats by Packaging

| Packaging Type | Lot Code Location | Format | Example |
|---|---|---|---|
| 25 kg woven polypropylene bag | Printed on label (side panel) | FP-CCYYMMDD-BB-PP | FP-20260715-42-01 |
| 500 g retail pouch | Printed on back panel (downward) | FP-CCYYMMDD-BB-PP | FP-20260715-42-02 |
| 1 kg bulk box | Printed on outer label | FP-CCYYMMDD-BB-PP | FP-20260715-42-03 |
| 20 L oil drum | Laser-printed on drum side | FP-CCYYMMDD-BB-PP | FP-20260715-42-04 |
| Pallet label | A4 label on two adjacent sides | FP lot + pallet number | FP-20260715-42-01 / P001 |

### 6.2 Best-Before / Expiry Date Format
`BBD: DD/MM/YYYY` or `EXP: MM/YYYY`

### 6.3 Label Integrity Checks
- Labels checked for adhesion, print quality, and legibility at start of each production run and every 30 minutes during run.
- Label applicator verified with photo-eye sensor.
- Rejected labels (misprinted, smudged, missing data) logged and destroyed.

---

## 7. Record Keeping Requirements

### 7.1 Retention Periods

| Record Type | Minimum Retention |
|---|---|
| Raw material receiving records (including COAs) | 5 years |
| Production batch records | 5 years |
| Finished product despatch records | 5 years |
| Customer / sales records | 5 years |
| Traceability exercise results (mock recalls) | 5 years |
| Recall / withdrawal records | 10 years |
| Supplier approval records | Current + 3 years |
| Training records | Employment + 1 year |
| Calibration records | 5 years |
| Environmental monitoring records | 3 years |

### 7.2 Record Format
- All records may be kept in electronic format (ERP, WMS, scanned documents) or hard copy.
- Electronic backups performed daily (off-site or cloud).
- Hard copy records stored in fireproof cabinet in QA Office.
- Access to records: Traceability Coordinator, QA Manager, Food Safety Team Leader, and authorised auditors.

### 7.3 Record Integrity
- Records must be **legible, date-stamped, and signed** (or electronic equivalent with audit trail).
- No erasures — corrections made by single line strike-through, initialled, and dated.
- Electronic records maintained in a validated, access-controlled system with full audit trail.

---

## 8. Recall Simulation Scenarios & Results

### 8.1 Annual Simulation Plan

| Year | Scenario | Scope | Date | Result | CAPA |
|---|---|---|---|---|---|
| 2024 | Undeclared sesame in 500g ground flax | Domestic retail customers | 12/03/2024 | 95% in 3h 20min | — |
| 2024 | Foreign metal fragment in 25kg flax meal | 1 international customer | 18/09/2024 | 100% in 2h 45min | — |
| 2025 | Packaging mislabel (allergen not declared) | 3 domestic distributors | 22/04/2025 | 100% in 3h 10min | Need faster customer contact numbers |
| 2025 | Supplier gluten cross-contact in sesame seed | All customers (7) | 10/11/2025 | 100% in 3h 50min | — |

### 8.2 Upcoming Simulation Schedule

| Quarter | Scenario Focus |
|---|---|
| Q1 2026 | Raw material to customer — multiple raw material lots (complex trace) |
| Q2 2026 | International customer + multi-country distributors |
| Q3 2026 | Rework trace exercise (rework lot → multiple finished lots) |
| Q4 2026 | Full recall simulation (including mock press release and regulatory notification) |

### 8.3 Lessons Learned Log

| ID | Finding | Root Cause | CAPA | Status | Closure Date |
|---|---|---|---|---|---|
| LL-2025-01 | Customer contact numbers outdated by 6 months in ERP | No periodic review of customer contact data | Implement annual customer data verification | Closed | 15/06/2025 |
| LL-2025-02 | Raw material COA paper filing took 25 min to retrieve | Off-site archiving of old records | Digitise all COAs for last 5 years; implement scanning at receiving | Closed | 30/07/2025 |
| LL-2025-03 | SCADA time stamp discrepancy vs batch record by 8 min | Clock drift on SCADA terminal | Enable NTP sync on all SCADA terminals | In progress | — |

---

## Appendices
- **Appendix A**: Traceability Report Form (One-Step-Back) — FS-TRC-F01
- **Appendix B**: Traceability Report Form (One-Step-Forward) — FS-TRC-F02
- **Appendix C**: Press Release Template — FS-TRC-F03
- **Appendix D**: Recall Contact Tree (pocket card)
- **Appendix E**: Lot Number Encoding Quick Reference Guide

---

*End of Document — FS-TRC-001*
