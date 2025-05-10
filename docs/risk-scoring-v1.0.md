# AGX Risk Scoring Framework v1.0

## ✨ Reimagining Risk in African Gold Trade

Western models often frame risk as static, punitive, and centralized. In contrast, AGX understands risk as contextual, evolving, and communal. Rooted in field realities across Ghana and Guinea, our scoring framework respects informal networks, values lived experience, and recognizes that trust must be earned and rebuilt — not imposed.

> “At AGX, risk is not a verdict — it’s a conversation. We use scores to open doors, not close them.”

This framework moves beyond colonial-style gatekeeping. It centers African agency, feedback loops, and the ability to ascend — not just comply.

## 🎯 Purpose

This document defines the official, version-controlled risk scoring model for evaluating actors in the AGX gold supply chain. It supports real-time decision-making, certification, audit targeting, and partner trust assessments.

---

## 🧱 Scoring Architecture

### The Trust Pathway

```
   🔴 RED     →     🟡 YELLOW     →     🟢 GREEN
 High Risk     Under Review         Trusted Actor
 (e.g., no docs) (training complete) (certified + verified)
```

This journey reflects AGX’s philosophy: actors can improve their score by learning, engaging, and contributing. Trust is not binary — it is built.

### Tier Visualization

```
  ┌───────────────┐     ┌───────────────┐     ┌───────────────┐
  │ 🟢 GREEN      │     │ 🟡 YELLOW     │     │ 🔴 RED         │
  │ 80–100 pts    │     │ 50–79 pts     │     │ 0–49 pts       │
  │ TRUSTED       │     │ NEEDS REVIEW  │     │ HIGH RISK      │
  └───────────────┘     └───────────────┘     └───────────────┘
```

These tiers help buyers, customs officers, and auditors make quick risk determinations in both field and digital environments.

* **Score Range:** 0–100
* **Tiers:**

  * 🟢 Green (80–100): Trusted
  * 🟡 Yellow (50–79): Caution / Review Required
  * 🔴 Red (0–49): High Risk / Restricted

### Weight Table

| Category                    | Weight |
| --------------------------- | ------ |
| KYC & Identity Integrity    | 20%    |
| Chain of Custody Compliance | 20%    |
| Document Timeliness         | 15%    |
| Training & Certification    | 15%    |
| Complaints / Red Flags      | 15%    |
| Audit Outcomes              | 10%    |
| Geographic Risk Modifier    | 5%     |

---

## 🧮 Example Scoring Breakdown

### Trader A — Sample Calculation

| Category                    | Score (out of max) |
| --------------------------- | ------------------ |
| KYC & Identity Integrity    | 18 / 20            |
| Chain of Custody Compliance | 15 / 20            |
| Document Timeliness         | 14 / 15            |
| Training & Certification    | 15 / 15            |
| Complaints / Red Flags      | 10 / 15            |
| Audit Outcomes              | 9 / 10             |
| Geographic Risk Modifier    | 4 / 5              |

**Total Score:** 85 → **Tier:** 🟢 Green (Trusted)

Certain events automatically downgrade scores:

* Falsified identity documents → 🔴
* Smuggling or unverified gold origin → 🔴
* Ignored audit request → 🔴
* Expired certification → 🟡

---

## 🔐 Data Privacy & Field Considerations

The AGX Risk Scoring Framework is designed with a strong emphasis on privacy, accessibility, and regional operability:

### Data Privacy

* Personally identifiable information (PII) is never exposed in public tier outputs.
* Risk scores are tied to TradePass IDs but reveal only tier and timestamp unless explicitly unlocked by authorized parties.
* All data updates are cryptographically signed and logged for auditability.

### Regional Relevance (Ghana & Guinea)

* The framework is calibrated to reflect legal, regulatory, and informal dynamics within Ghana and Guinea.
* Geographic modifiers account for known smuggling routes, high-risk zones, and governance gaps.
* Red flag detection thresholds were developed in consultation with local field agents and regulatory partners.

### Accessibility

* Designed for mobile and low-bandwidth environments.
* Scores can be queried via QR, offline-capable tools, and field agent dashboards.
* Interfaces are localized in English, French, Twi, and Malinké.

| Trigger           | Update Frequency |
| ----------------- | ---------------- |
| New certification | Immediate        |
| Audit results     | Within 7 days    |
| Complaint review  | Within 14 days   |
| Auto-decay        | Monthly          |
| Appeal outcome    | Case-by-case     |

**New Certification**
A risk score is updated immediately when an actor completes AGX-approved training, recertification, or compliance milestones. These changes reflect intentional improvement and allow actors to progress along the Trust Pathway without delay.

**Audit Results**
Field audits—including site inspections and records reviews—are incorporated into scores within seven days. This ensures real-world behaviors (positive or negative) are reflected in near real-time for downstream stakeholders.

**Complaint Review**
Complaints filed by miners, aggregators, field agents, or buyers trigger an internal review. If substantiated, the resulting penalty or red flag is applied within 14 days. This timeframe balances speed with due process.

**Auto-decay**
When actors become inactive—failing to update their documents, participate in recertification, or submit required data—their score is gradually reduced each month. This discourages dormancy and incentivizes active, ongoing participation.

**Appeal Outcome**
If an actor disputes a scoring event and wins the appeal, their score is adjusted upon resolution. While the timing varies by case, all changes are logged and linked to an auditable appeal ID.

---

## 🧑‍⚖️ Governance Structure

### Governance Flow Overview

```
 Actor → Certification or Audit → Score Assigned → Public Registry
     ↓                            ↓                     ↓
  Complaint Filed → Review → Appeal (if applicable) → Score Adjusted
```

This governance flow ensures checks and balances between field data, technical scoring, and institutional oversight.

| Role             | Responsibility                                                                                                                                                                                                               |                                                |
| ---------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------- |
| AGX Scoring Team | Maintains the core risk scoring algorithm, implements new rules, processes bulk updates (e.g. post-certification), and publishes changelogs. This team ensures consistency, fairness, and version control across the system. |                                                |
| Auditors         | Conduct on-site and virtual inspections, submit verified observations, flag anomalies, and feed qualitative and quantitative data into the scoring engine. Their work anchors the score in real-world activity.              |                                                |
| Certification    | Provides training and recertification data from the AGX curriculum, ensuring only validated participants contribute to score upgrades. Certification updates feed directly into the scoring pipeline.                        |                                                |
| Appeals Panel    | A neutral and multi-stakeholder body that reviews contested scoring events. It includes at least one independent member and must resolve disputes within set timelines. Its decisions are binding and logged.                | Handles disputes (3+ members, incl. 1 neutral) |

---

## 🧠 Field Insights

Risk does not always present itself in paperwork. In the gold trade, trust is spoken, observed, and remembered long after contracts fade. The field is not a neutral stage—it is emotional, political, and seasonal. AGX field agents frequently report trust signals that systems fail to detect:

> “A trader’s documents were perfect, but miners wouldn’t work with him. Turns out he withheld payment during the rains. The registry didn’t catch it — but a field agent did.”  — AGX Auditor, Upper Guinea

In another case, an aggregator consistently paid below-market prices but delivered on time and protected his team during a regional lockdown. His actions built trust that wasn’t reflected in any official form.

These examples show that trust and risk must be co-constructed from both digital records and lived memory. AGX scoring recognizes this duality—and honors what is seen in the bush, not just what’s signed in the capital.

---

## 📘 Use Cases

AGX Risk Scores are not just back-office metrics—they are **living signals** that circulate through every layer of the gold trade. From border clearance to miner payouts, the score informs trust at speed.

* **TradePass Integration**: Every certified actor’s score is embedded in their TradePass profile and QR code. A vault, buyer, or customs agent scanning the profile sees their current trust tier—green, yellow, or red—and can view context notes where authorized.

* **Customs & Border Control**: Border officials use AGX scores as a real-time triage layer. A green score can fast-track a parcel; a red score may flag it for additional inspection, verification, or rejection.

* **Vaults, Refineries, and Aggregators**: Internal workflows may prioritize green-tier suppliers for intake and lending. Yellow-tier actors may be required to submit a recertification or training update before shipment.

* **Field Agent Dashboards**: Scores guide which actors need follow-up, audit attention, or support. A falling score is not just a flag—it’s a prompt to reach out, retrain, or revisit.

* **Community Trust Signaling**: Co-ops and associations may view aggregated scores to determine eligibility for shared loans, joint export, or cooperative branding under AGX-certified clusters.

---

## 📚 Glossary

**Risk Score**
A numerical value between 0 and 100 assigned to each certified actor. It reflects the actor’s compliance behavior, audit outcomes, documentation quality, and social signals over time. It is not a fixed identity but a dynamic measure that changes with behavior and environment.

**Tier**
A simplified color-coded categorization (Green, Yellow, Red) derived from the Risk Score. Tiers help external parties (e.g., customs, vaults, buyers) make fast trust decisions without accessing full profile details. Tier does not capture nuance but flags general status.

**Auto-Decay**
A system-triggered reduction in Risk Score when an actor does not engage in required updates (e.g., document submission, recertification) over time. It prevents actors from maintaining high scores while inactive or avoiding review.

**Red Flag**
An automatically triggered override of the score based on critical risk events such as falsified ID, unresolved complaints, or unverified gold origin. Red flags are grounded in field realities and are defined in collaboration with local stakeholders.

**Appeals Panel**
A multi-stakeholder committee including at least one neutral member. It reviews disputed risk scores, investigates irregularities, and issues binding resolutions. The panel is part of AGX’s commitment to procedural fairness and local voice inclusion.

---

## 🌍 The Future of Risk: Toward an African Trust Model

Western systems often use risk as a control mechanism: a reason to exclude, blacklist, or deny access. AGX proposes a new model—**risk as a relationship**, not a verdict.

We introduce two innovations:

### 🧠 1. Trust Memory (Qualitative Context Layer)

Every actor may accrue a "Trust Memory"—field-submitted, human-reviewed entries that reflect conduct, contribution, and social trust. These memories add narrative depth to a numeric score and are especially important in contexts where behavior and consistency speak louder than documents.

The following profiles illustrate how trust is built through behavior, not bureaucracy:

```
🟡 Trader B – Score: 74
Trust Memory:
✔ Repaid a local miner in advance during a family emergency (June 2024)
✔ Facilitated a co-op meeting to resolve conflict between miners and transporters (May 2024)
✔ Coordinated with village elders to ensure safe passage during local unrest (March 2024)
⚠️ Accepted underweight gold once without correction (February 2024)
✔ Helped a miner acquire medical care after a worksite injury (January 2024)
✔ Supported digitization of weighing logs across 3 communities (December 2023)
✔ Mentored two young women entering the gold trade through local apprenticeship (November 2023)
✔ Shared transport costs with other aggregators to reduce community burden (October 2023)
✔ Hosted an informal audit prep session for surrounding miners (September 2023)
```

```
🟢 Miner A – Score: 88
Trust Memory:
✔ Consistently delivers high-integrity gold with full traceability (June 2024)
✔ Educated peers on safety measures during the rainy season (May 2024)
✔ Donated tools to a nearby cooperative after equipment failure (April 2024)
✔ Participated in AGX environmental workshop and led community clean-up (March 2024)
```

```
🟡 Exporter A – Score: 72
Trust Memory:
✔ Voluntarily disclosed customs irregularity and corrected it proactively (May 2024)
✔ Sponsored training for two aggregators in digital traceability (April 2024)
⚠️ Missed one quarterly reporting deadline due to administrative backlog (March 2024)
✔ Partnered with AGX to pilot mobile inspection module at border checkpoint (February 2024)
```

Trust Memories are not for punishment or praise alone—they give regulators, buyers, and auditors the social context that documents often miss. They recognize that trust is built over time through small, meaningful actions that build confidence and accountability in a community of practice.

### 🔄 2. Dynamic Trust Index

Separate from the numeric score, the Trust Index is a qualitative signal designed to reflect trust as observed—not just measured. It complements the risk score by capturing nuance, reputation, and social legitimacy in ways that numbers alone cannot.

**Narrative-driven**
The Trust Index includes human-readable summaries sourced from field agents, miners, and cooperatives. It reflects real events, like conflict resolution, consistent payout behavior, or community-building contributions. These narratives are logged as part of the actor’s profile and are accessible in TradePass field views.

**Community-influenced**
Unlike the risk score, which is computed centrally, the Trust Index is shaped by decentralized input: community endorsements, field audits, miner feedback, and regional validators. This distributed validation helps capture relational trust that documents overlook—particularly in informal or low-literacy environments.

**Role-weighted**
Trust signals are evaluated differently depending on the actor's role. For example:

* For a miner: trust may emphasize honesty in weighing, consistency of supply, and environmental practices.
* For an aggregator: reliability in payments, transparency in volume reporting, and fair negotiation.
* For an exporter: customs cooperation, complaint resolution, and audit responsiveness.

These weighted insights ensure that trust is measured in context—not by a uniform yardstick, but by what matters for that actor’s function in the gold ecosystem.

This index is visible in field apps and TradePass, offering an organic signal that complements algorithmic scoring.

## 🌱 A Living Risk Model

AGX scoring is not a static spreadsheet. It is a **living system**, shaped by people, context, and time. Risk must evolve alongside trust, seasonality, and the realities of those operating in the field.

### Quarterly Recalibration Forums

In each region of deployment, AGX facilitates quarterly convenings that include local miners, traders, cooperatives, AGX field representatives, and government partners. These sessions serve not only as accountability checkpoints but as interpretive spaces—where context is brought to data. Participants review emerging risk patterns, surface regional challenges (e.g. flooding, permit delays, extortion at checkpoints), and recommend adjustments to scoring weightings or red flag sensitivity.

This community-led governance ensures that no score is ever frozen in abstraction. It evolves with feedback, climate, and context.

### Decentralized Scoring Nodes

To avoid over-centralization and colonial-style control, AGX introduces scoring “nodes”—cooperative-level or field-based bodies with limited, accountable rights to propose or modify local risk scoring rules. These nodes can:

* **Recommend contextual flags**: For example, if a particular region faces transport challenges during the dry season due to road degradation, nodes can flag deliveries made under such conditions as lower risk than missed deliveries in better conditions. Risk, in this context, is modulated by reality—not just rules.

* **Submit role-specific adjustments**: A mobile aggregator operating in rural, low-density areas may have fewer verifiable documents but high relational trust. Nodes can propose adjusted scoring logic that balances informal systems with traceability tools.

* **Report risk signals not visible in documents**: These include behaviors like consistently paying miners fairly even in volatile markets, handling disputes transparently, or conversely, creating bottlenecks in community flows. These signals are submitted as qualitative notes and logged as part of the actor’s Trust Memory.

### Role-Specific Thresholds

One score does not fit all. A vault operator managing 500kg under armed transport cannot be assessed by the same bar as an informal aggregator riding a motorbike across village roads. Risk must be **calibrated, not copied**.

Each actor type in AGX is assigned threshold bands, red flag sensitivity levels, and trust-pathway logic based on:

**Role Exposure**
Refers to the level and nature of operational risk an actor carries due to the volume of gold handled, the sensitivity of their touchpoints (e.g., access to export permits, contact with vulnerable miners), and the inherent security implications. For instance, a vault operator managing large quantities under armed guard requires different scrutiny than a community aggregator who transports by motorcycle across rural paths.

**Local Volatility**
Accounts for the instability or complexity of the actor’s operating region. This includes factors such as political unrest, the presence of unofficial toll checkpoints, regional corruption practices, or a history of enforcement inconsistencies. An actor working in high-conflict zones may require additional narrative inputs to avoid unfair penalization.

**Community Reliance**
Recognizes the social and economic interdependence surrounding the actor. It asks: How many livelihoods are linked to this person’s fairness? How disruptive would their absence be? A mid-tier aggregator serving 80 miners across 3 villages carries different systemic importance than a lone trader in a city. Risk scoring here includes responsibility as a proxy for embeddedness.

This allows the framework to flex without bias, and to center what matters: **not perfect documentation, but measurable contribution to a trusted system.**

### Acknowledgments

The AGX Risk Scoring Framework builds upon foundational international guidelines, while explicitly adapting them to African field realities:

* **OECD Due Diligence Guidance Annex II**: Our model incorporates the core principles of Annex II, especially the importance of identifying and mitigating risks of conflict financing, money laundering, and human rights abuses in mineral supply chains. We extend this by operationalizing risk not only at the exporter level but down to aggregators and field agents.

* **planetGOLD Risk Mitigation Standards**: AGX aligns with planetGOLD’s emphasis on progressive formalization, transparency in ASM (Artisanal and Small-scale Mining), and human-centric monitoring systems. Our Trust Memory and Dynamic Trust Index build on planetGOLD’s idea of risk as a social and behavioral pattern—not just a legal status.

* **LBMA Responsible Gold Guidance**: While LBMA’s framework centers on refiners, AGX adapts the five-step approach to pre-export field actors. Our red flag triggers and audit-linked scoring mirror LBMA’s escalation procedures but apply them preemptively—where interventions matter most.

Field practices and scoring calibrations were co-developed through immersive research and stakeholder engagement in Ghana and Guinea. These included input from auditors, aggregators, customs agents, regulatory bodies, and local cooperatives. build on planetGOLD’s idea of risk as a social and behavioral pattern—not just a legal status.

* **LBMA Responsible Gold Guidance**: While LBMA’s framework centers on refiners, AGX adapts the five-step approach to pre-export field actors. Our red flag triggers and audit-linked scoring mirror LBMA’s escalation procedures but apply them preemptively—where interventions matter most.

Field practices and scoring calibrations were co-developed through immersive research and stakeholder engagement in Ghana and Guinea. These included input from auditors, aggregators, customs agents, regulatory bodies, and local cooperatives.

**Transparency Protocols**
All AGX risk scoring criteria, weightings, and red flag triggers are publicly documented and version-controlled. Any modification to the scoring logic undergoes community review and is published with a changelog and implementation date. This ensures that no scoring decision happens in the dark, and that actors can align with the most current expectations.

**Actor Access**
Every certified actor has the right to view their own scoring breakdown—including points earned in each category, active red flags, and the historical trend of their score. Access is available via mobile dashboard, printed report, or digitally through TradePass integration.

**Appeals and Dispute Resolution**
Actors may file a formal appeal within 30 days of a scoring event they believe is inaccurate, biased, or unsupported. Appeals are reviewed by the independent AGX Appeals Panel and must be resolved within a transparent and recorded timeframe. During appeals, no further score penalties are applied.

**Audit Logging and Integrity**
All final score changes—whether from audits, appeals, or decay—are recorded in a cryptographically signed ledger. This ensures integrity, traceability, and the ability for external review by partners, donors, or regulatory bodies.

---

**License:** CC BY-SA 4.0
**Maintained by:** AGX Protocol Compliance Team
