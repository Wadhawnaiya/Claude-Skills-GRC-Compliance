# SWIFT Customer Security Programme (CSP) Skill for Claude

> **Disclaimer:** This skill provides educational and advisory guidance based on publicly available SWIFT Customer Security Controls Framework (CSCF) documentation. It is not a substitute for an independent assessment conducted by a qualified SWIFT CSP assessor. Attestation decisions must be made by your organisation and its approved independent assessor. SWIFT CSP requirements are subject to annual revision — always verify against the current CSCF version published by SWIFT.

---

## 1. What Does the Skill Do?

This skill turns Claude into an expert advisor on the **SWIFT Customer Security Programme (CSP)** and the **Customer Security Controls Framework (CSCF) v2025**. It provides structured, actionable guidance to financial institutions, custodians, brokers, corporates, and service bureaux that must achieve and maintain mandatory compliance with SWIFT's security controls across the global payment network.

The skill is grounded in **CSCF v2025** (effective July 2025), which defines 31 security controls — 23 mandatory and 8 advisory — organised across three objectives: Secure Your Environment, Know and Limit Access, and Detect and Respond. It covers all five SWIFT connectivity architecture types (A1, A2, A3, A4, B), enabling precise scoping of which controls are mandatory or advisory for a given institution's infrastructure footprint.

Rather than generic cybersecurity advice, the skill produces control-specific output keyed to CSCF control numbers: gap assessments with per-control evidence requirements, architecture scoping matrices, KYC-SA attestation preparation checklists, implementation guidance with concrete evidence artifacts, incident response procedures aligned to SWIFT notification obligations, and cross-framework mappings to ISO 27001:2022, PCI DSS v4.0.1, and NIST CSF 2.0.

The skill also covers the annual attestation lifecycle — from independent assessment through KYC Security Attestation (KYC-SA) portal submission — and is current with the v2024 to v2025 changes including tightened patching SLAs (critical patches reduced from 7 to 3 calendar days) and clarified hardware token requirements under Control 4.2.

---

## 2. Intended Audiences

| Audience | How They Use the Skill |
|----------|----------------------|
| **CISO / Head of Information Security** | Gap assessments against CSCF v2025, strategic remediation roadmap, risk ownership decisions, cross-framework alignment |
| **SWIFT Operations / Payments Technology Teams** | Control implementation guidance, architecture scoping (A1/A2/A3/A4/B), evidence artifact collection, configuration walkthroughs |
| **Internal Audit / Independent Assessors** | Control test procedures, evidence quality review, KYC-SA attestation workflow, assessor qualification requirements |
| **Compliance Officers** | Attestation timeline management, regulatory context (DORA, NY DFS, MAS TRM, HKMA CFI, APRA CPS 234), counterparty notification obligations |
| **Third-Party Risk / Vendor Management Teams** | Service bureau (Type B) responsibility mapping, Control 2.8 outsourcing obligations, provider KYC-SA review |
| **Incident Response Teams** | SWIFT-specific incident response planning (Control 7.1), SWIFT notification obligations (24-hour initial, 30-day full report) |
| **Security Engineers** | MFA hardware token deployment (4.2), SIEM log source configuration (6.4), vulnerability scanning scope (2.7), system hardening baselines (2.3) |

---

## 3. Common Use Cases

### Gap Analysis and Attestation Readiness

- Assess our SWIFT environment against all 23 mandatory CSCF v2025 controls for an A1 architecture
- Produce a gap report with red/amber/green status, evidence availability, and remediation actions
- What changed between CSCF v2024 and v2025 and how does it affect our current attestation?
- We're submitting our KYC-SA by the July 31 deadline — give me a pre-submission checklist

### Architecture Scoping

- We use Alliance Access on-premises — which controls apply to us and which are not applicable?
- We switched from a service bureau to a direct A1 connection — how does our control scope change?
- Map all 31 controls to each architecture type (A1/A2/A3/A4/B) in a single reference table
- Our cloud team wants to move SWIFT connectivity to the SWIFT Cloud (A4) — what new controls apply?

### Control Deep-Dives and Implementation

- Walk me through implementing Control 4.2 Multi-Factor Authentication — what hardware token options satisfy CSCF v2025?
- What does Control 1.1 require for our SWIFT Secure Zone network architecture? Give me the evidence artifacts
- We're failing Control 6.4 Log and Monitoring — what log sources must feed our SIEM and what is the retention requirement?
- How do we comply with Control 2.8 if our SWIFT messaging is operated by a service bureau?

### KYC-SA Attestation Preparation

- Generate a KYC-SA attestation checklist for all mandatory controls with evidence pointers
- Walk me through the independent assessment requirements for CSCF v2025 — who qualifies as an assessor?
- What does "Partially Implemented" mean in the KYC-SA portal and when should we use it?
- Our counterparty is asking about our attestation status — what do they see on the KYC Registry?

### Incident Response and SWIFT Notifications

- Draft a SWIFT-specific Incident Response Plan covering detection, containment, and SWIFT notification
- At what point does an incident become notifiable to SWIFT and what is the timeline?
- Walk me through the SWIFT incident notification obligations under Control 7.1
- A malware alert was triggered on a SWIFT operator workstation — what do we do in the next 24 hours?

### Cross-Framework Mapping

- Map CSCF v2025 mandatory controls to ISO 27001:2022 Annex A controls
- How does SWIFT CSP relate to PCI DSS v4.0.1 — what gaps remain if we're already PCI-compliant?
- Show me CSCF controls mapped to NIST CSF 2.0 functions and categories
- Does ISO 27001 certification cover our SWIFT CSP obligations?

---

## 4. How to Use the Skill

### Installation

1. Download the `swift-csp.skill` file from the `SWIFT CSP - Claude Skill/` folder
2. In Claude, go to **Settings → Skills**
3. Upload the `.skill` file
4. The skill activates automatically for relevant conversations — no special command needed

### Triggering the Skill

The skill triggers automatically when your message relates to SWIFT security, CSCF controls, or SWIFT attestation. Example phrases that activate it:

- *"We need to complete our SWIFT CSP attestation by July"*
- *"What does CSCF v2025 require for MFA?"*
- *"Our SWIFT audit found gaps in Control 6.4 — how do we remediate?"*
- *"We use a service bureau for SWIFT — what are our obligations?"*
- *"Map our SWIFT controls to ISO 27001"*
- *"Help us prepare our KYC-SA submission"*
- *"What changed from CSCF v2024 to v2025?"*

### Example Prompts

```
"Run a CSCF v2025 gap assessment for our A1 architecture. We have 
hardware MFA tokens for SWIFT operators, a dedicated SWIFT VLAN with 
firewall rules, SIEM coverage, but our patch SLAs are not formally 
documented and we have no SWIFT-specific incident response plan."
```

```
"We are a Type B user (service bureau). Which of the 23 mandatory 
controls do we attest to ourselves versus relying on our bureau's 
attestation? Produce a responsibility assignment table."
```

```
"Draft a SWIFT-specific Incident Response Plan section covering: 
detection triggers, internal escalation, SWIFT notification obligations 
(24-hour and 30-day reporting), evidence preservation, and recovery steps."
```

```
"Produce a KYC-SA attestation preparation checklist for all 23 mandatory 
CSCF v2025 controls. For each control, list: the attestation status options, 
minimum evidence required, and common findings that result in 'Partially 
Implemented' attestation."
```

```
"Map all CSCF v2025 mandatory controls to ISO 27001:2022 Annex A. 
Highlight any SWIFT-specific requirements that are not covered by ISO 27001 
and would require additional controls beyond our ISMS."
```

---

## 5. Skill Implementation Details

### Architecture

```
plugins/swift-csp/skills/swift-csp/
├── SKILL.md                        # Main skill: framework overview, architecture types,
│                                   # all 31 controls summary table, response format
│                                   # routing, key implementation priorities, attestation
│                                   # timeline, common findings and remediation
└── references/
    ├── swift-controls.md           # Full control reference: architecture applicability
    │                               # matrix, all 31 controls with purpose, requirements,
    │                               # implementation steps, and evidence artifacts
    └── swift-assessment.md         # KYC-SA attestation process, independent assessor
                                    # requirements, v2024→v2025 changes, SWIFT incident
                                    # notification obligations, service bureau
                                    # responsibility split, cross-framework mappings
                                    # (ISO 27001, PCI DSS, NIST CSF), regulatory context,
                                    # gap assessment checklist template

SWIFT CSP - Claude Skill/
├── SWIFT-CSP-README.md             # This file
└── swift-csp.skill                 # Standalone installable skill file
```

### What's in SKILL.md

- **YAML frontmatter** with skill name, description, and auto-trigger phrases
- **Framework overview table** — CSCF version, control count, attestation type, compliance consequences
- **Architecture types reference** — A1, A2, A3, A4, B with descriptions and typical users
- **Three security objectives** — Secure Your Environment (1.x, 2.x, 3.x), Know and Limit Access (4.x, 5.x), Detect and Respond (6.x, 7.x)
- **Control summary table** — all 31 controls with control number, name, mandatory/advisory status, and objective
- **Response format routing** — task type to output format mapping (gap assessment, architecture scoping, control deep-dive, KYC-SA prep, incident response, cross-framework)
- **Key implementation priorities** — the 7 highest-risk controls most commonly cited in assessments
- **Annual attestation timeline** — from January 1 assessment start through July 31 submission deadline
- **Common findings and remediation** — 8 most frequent non-compliance patterns with specific remediation steps
- **Reference file pointers** — instructions directing Claude to load reference files for deep content

### What's in the reference files

| File | Contents |
|------|----------|
| `references/swift-controls.md` | Architecture applicability matrix (all 31 controls × 5 architecture types); full implementation details for all mandatory controls including Control 1.1 (SWIFT Environment Protection), 1.2, 1.4, 2.1–2.10, 3.1, 4.1–4.2, 5.1–5.2, 5.4, 6.1–6.4, 7.1–7.2 with purpose, requirements, implementation steps, and evidence artifacts; summary entries for all advisory controls |
| `references/swift-assessment.md` | KYC-SA attestation workflow (5-step process); independent assessor qualification requirements; CSCF v2024→v2025 change table; SWIFT incident notification obligations with deadlines; service bureau (Type B) responsibility split table; CSCF↔ISO 27001:2022 mapping; CSCF↔PCI DSS v4.0.1 mapping; CSCF↔NIST CSF 2.0 mapping; regulatory context (EU DORA, US FFIEC/NY DFS, UK PRA, MAS TRM, HKMA CFI, APRA CPS 234); gap assessment checklist template; 7 most common non-compliance patterns |

### Inputs used to build the skill

| Source | Description |
|--------|-------------|
| **SWIFT CSCF v2025** | Authoritative source for all 31 control definitions, mandatory/advisory designations, architecture applicability, and attestation requirements |
| **SWIFT KYC-SA Portal guidance** | Annual attestation workflow, submission deadlines, counterparty visibility rules, attestation status options |
| **SWIFT Security Hardening Guides** | Alliance Access and Alliance Gateway application hardening requirements (Control 2.10) |
| **SWIFT incident reporting obligations** | 24-hour initial notification and 30-day full report requirements under Control 7.1 |
| **ISO/IEC 27001:2022 Annex A** | Cross-framework mapping of CSCF controls to ISO 27001 Annex A control identifiers |
| **PCI DSS v4.0.1** | Cross-framework mapping highlighting shared controls and SWIFT-specific gaps |
| **NIST CSF 2.0** | Functional category mapping for CSCF controls |
| **Regulatory references** | ECB TIBER-EU, EBA ICT/DORA, FFIEC, NY DFS 23 NYCRR 500, Bank of England/PRA, MAS TRM, HKMA CFI, APRA CPS 234 |
| **Assessment methodology** | Independent assessor qualification standards, community standard vs enhanced assessment criteria |

### Skill trigger phrases

`SWIFT CSP` · `SWIFT Customer Security Programme` · `CSCF` · `CSCF v2025` · `KYC-SA` · `KYC Security Attestation` · `SWIFT attestation` · `SWIFT security controls` · `SWIFT secure zone` · `Alliance Access security` · `Alliance Gateway security` · `SWIFT MFA` · `SWIFT architecture A1 A2 A3 A4 B` · `service bureau SWIFT` · `SWIFT gap analysis` · `SWIFT independent assessment` · `SWIFT incident response` · `SWIFT mandatory controls` · `SWIFT advisory controls` · `payment fraud prevention SWIFT` · `SWIFT compliance` · `SWIFT CSP assessment`

---

## 6. Author

**Hemant Naik**
[LinkedIn](https://www.linkedin.com/in/tanaji-naik/) · [hemant.naik@gmail.com](mailto:hemant.naik@gmail.com)
