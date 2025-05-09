**AGX Risk Scoring Framework**
**Version 1.0** — Public Documentation

---

## 🎯 Part 1: Scoring Overview

Each certified actor in the AGX ecosystem (trader, aggregator, exporter, etc.) receives a compliance risk score between 0 and 100. This score reflects the actor’s trustworthiness and operational integrity within the AGX Protocol. Scores are tiered to provide intuitive interpretation:

| Tier      | Score Range | Interpretation                |
| --------- | ----------- | ----------------------------- |
| 🟢 Green  | 80–100      | Trusted / Verified            |
| 🟡 Yellow | 50–79       | At Risk / Needs Review        |
| 🔴 Red    | 0–49        | High Risk / Under Restriction |

Actors’ scores can improve or decay over time based on behavioral inputs, audits, and compliance milestones.

---

## 🧱 Core Risk Criteria

Scoring is based on weighted categories and sub-factors:

| Category                       | Weight (%) | Sub-Factors                                               |
| ------------------------------ | ---------- | --------------------------------------------------------- |
| KYC / Identity Integrity       | 20%        | Verified ID, documentation match, no duplicates           |
| Source & Chain-of-Custody      | 20%        | Origin verification, tamper-proof bag use, miner ID match |
| Document Accuracy & Timeliness | 15%        | On-time submissions, consistent reporting                 |
| Training & Certification       | 15%        | Completed AGX curriculum, current recertification         |
| Red Flags & Complaints         | 15%        | Number and severity of substantiated complaints           |
| Audit Results & Site Visits    | 10%        | Field audit score and last verification outcome           |
| Geographic Risk Modifier       | 5%         | Risk score adjustment for operating region                |

---

## 🧮 Sample Calculation

**Trader A:**

* Verified ID: ✅ (+18/20)
* Chain-of-Custody: Partial (1 improper bagging event) (+15/20)
* Documents on time: ✅ (+14/15)
* Training completed: ✅ (+15/15)
* 1 complaint (resolved): (+10/15)
* Audit score: Pass (+9/10)
* Region: Guinea (moderate risk) (+4/5)
* **Total Score:** 85 → **Tier:** 🟢 Green

---

## ⚠️ Red Flag Triggers (Automatic Downgrades)

The following events trigger instant score penalties:

* ❌ Missing or falsified ID → 🔴 Red
* ❌ Unverified gold source / no miner identity → 🔴 Red
* ⏰ Repeated late submissions (3+) → 🟡 Yellow
* ⚠️ Substantiated fraud, smuggling, or abuse → 🔴 Red
* 🚫 Ignored audit request → 🔴 Red
* 📚 Expired training or certification → 🟡 Yellow (auto-downgrade)

---

## ✅ Part 2: AGX Risk Score Governance Charter

### 🎯 Purpose

The AGX Risk Score must be governed transparently and updated fairly to ensure that certified actors are treated impartially and consistently.

### 🧑‍⚖️ Governance Structure

| Role                 | Authority                                                               |
| -------------------- | ----------------------------------------------------------------------- |
| AGX Scoring Team     | Maintains scoring algorithm, processes mass updates                     |
| Field Auditors       | Submit audit results, verification flags                                |
| Certification System | Feeds training data into scoring model                                  |
| Registry Admin       | Displays updated score in public registry profile                       |
| Appeals Panel        | Reviews challenges to scoring outcomes (min. 3 members incl. 1 neutral) |

---

### 🔁 Scoring Update Triggers

| Update Type              | Frequency      | Source / Trigger                             |
| ------------------------ | -------------- | -------------------------------------------- |
| Certification completion | Immediate      | Passing AGX curriculum                       |
| Audit-based update       | Within 7 days  | Site visit or verification review            |
| Complaint investigation  | Within 14 days | Via AGX’s Red Flag Report system             |
| Auto-decay               | Monthly        | Lack of updated documents or recertification |
| Appeals resolution       | Case-by-case   | Result logged and applied to score           |

---

## 🧾 Transparency & Appeals

* All scoring logic is published and version-controlled
* Each actor may view their full scoring breakdown
* Actors may file 1 appeal per event within 30 days
* Appeals Panel decisions are final and logged
* A public summary of changes is published unless risk of retaliation applies

---

**License:** Open Documentation (CC BY-SA 4.0)
**Maintained by:** AGX Compliance & Protocol Team
