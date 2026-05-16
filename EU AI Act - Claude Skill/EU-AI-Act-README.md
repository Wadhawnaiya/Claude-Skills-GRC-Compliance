# EU AI Act Skill for Claude

> **Disclaimer:** This skill provides informational guidance based on Regulation (EU) 2024/1689
> (the EU AI Act) and related implementing measures. It does not constitute legal advice. AI
> system classification, conformity assessment pathways, and compliance obligations with material
> legal or commercial consequences should be reviewed by a qualified EU law specialist or notified
> body. This skill covers the Act as published; delegated acts, harmonised standards, and Codes
> of Practice are evolving — guidance on these items is flagged as subject to update.

---

## 1. What Does the Skill Do?

This skill gives Claude deep expertise in **Regulation (EU) 2024/1689** — the EU AI Act —
the world's first comprehensive horizontal AI regulatory framework. Published in the EU Official
Journal on 12 July 2024, the Act applies in phases from February 2025 through August 2027, with
prohibited practices enforceable from 2 February 2025, GPAI model obligations from 2 August 2025,
and high-risk system obligations from 2 August 2026 (Annex III) and 2 August 2027 (Annex I
safety components).

The skill implements an eight-step compliance workflow: identifying the user's role under the
Act (provider, deployer, importer, distributor, authorised representative per Art. 3); classifying
AI systems against the Art. 3(1) definition; screening against all eight prohibited practices
under Art. 5; determining the risk tier (prohibited, high-risk Path A under Art. 6(1), high-risk
Path B under Art. 6(2)/Annex III, limited-risk under Art. 50, or minimal risk); walking through
all mandatory high-risk obligations under Arts. 8–17 and 26; determining conformity assessment
pathways and CE marking requirements under Arts. 43–48; assessing GPAI model obligations under
Arts. 53–55 including the systemic risk threshold (≥10²⁵ FLOPs); and covering post-market
monitoring and serious incident reporting obligations.

Every response cites the governing Article, Annex, or Recital. The skill covers all eight Annex
III high-risk use case areas (biometric identification, critical infrastructure, education,
employment, access to services, law enforcement, migration, administration of justice), maps the
full penalty regime under Art. 99 (up to €35M or 7% of global turnover for prohibited practice
violations), and cross-maps to ISO 42001, NIST AI RMF, and GDPR for organisations managing
multiple compliance frameworks simultaneously.

---

## 2. Intended Audiences

| Role | How They Use the Skill |
|------|----------------------|
| AI Providers & Developers | Risk classification, prohibited practice screen, Arts. 8–17 obligation gap analysis, conformity assessment pathway determination |
| AI Deployers | Art. 26 deployer obligation review, instructions compliance, human oversight design, 6-month log retention, incident notification |
| Legal & Compliance Teams | Article citations, penalty exposure analysis, cross-framework mapping (GDPR, ISO 42001) |
| GPAI Model Developers | Arts. 53–55 universal vs systemic risk obligations, Annex XI/XII documentation, open-source exception scope |
| Product Managers | Risk tier determination, CE marking requirements, EU AI database registration (Arts. 49, 60) |
| CISOs & Security Teams | Art. 15 accuracy/robustness/cybersecurity requirements, adversarial testing for systemic risk GPAI |
| DPOs & Privacy Teams | GDPR alignment with Art. 10 data governance, Art. 22 automated decision-making intersection |
| Notified Bodies & Auditors | Conformity assessment paths (Annex VI self-assessment vs Annex VII third-party), post-market monitoring |

---

## 3. Common Use Cases

### AI System Classification

- "Classify our CV-screening tool — is it prohibited, high-risk, limited-risk, or minimal risk?"
- "We use a chatbot for customer service. What transparency obligations apply under Art. 50?"
- "Our AI system makes creditworthiness assessments. Is this Annex III high-risk under Point 5(b)?"
- "We're building a real-time biometric identification system for a shopping centre. Is this prohibited?"
- "What is the Art. 3(1) definition of an AI system and does our rules-based system qualify?"

### Prohibited Practices Screen (Art. 5 — enforceable from 2 February 2025)

- "Does our emotion recognition system at workplace entry points violate Art. 5(1)(f)?"
- "We build social scoring tools for an employer. Does this fall under the Art. 5 prohibition?"
- "Our marketing tool uses subliminal techniques to influence purchasing behaviour. Is this prohibited?"
- "What is the narrow law enforcement exception to the real-time remote biometric identification prohibition?"
- "Screen our AI product portfolio against all eight prohibited practices in Art. 5."

### High-Risk System Obligations (Arts. 8–17, 26)

- "Generate a gap assessment for our high-risk AI system against all Arts. 8–17 obligations."
- "What does a risk management system under Art. 9 require? What are the five mandatory steps?"
- "Draft the technical documentation content required by Art. 11 and Annex IV."
- "What automatic logging must our high-risk AI system implement under Art. 12?"
- "Our deployer obligations under Art. 26 — how do we document compliance?"
- "What does human oversight under Art. 14 mean in practice for our clinical decision support system?"

### Conformity Assessment and CE Marking

- "Our AI system is under Annex III Point 1 (biometrics). Must we use a notified body or can we self-assess?"
- "Walk me through the EU Declaration of Conformity requirements under Art. 47."
- "When must our system be registered in the EU AI database under Art. 49?"
- "We applied harmonised standards in our conformity assessment. How does this affect our notified body obligation?"

### GPAI Model Obligations (enforceable from 2 August 2025)

- "We're developing a foundation model trained on 8×10²⁴ FLOPs. Do we cross the systemic risk threshold in Art. 51?"
- "What documentation must we provide under Arts. 53 and Annex XI/XII as a GPAI provider?"
- "We release our GPAI model under an open-source licence. What obligations still apply?"
- "What additional obligations apply to systemic risk GPAI models under Art. 55?"
- "We use a third-party GPAI model to build our product. What are our downstream provider obligations?"

### Penalties and Governance

- "What is the penalty for deploying a prohibited AI practice under Art. 99?"
- "Which authority enforces the EU AI Act in Germany? How does the AI Office relate to national authorities?"
- "What is the role of the European AI Board versus the AI Office versus national market surveillance authorities?"

### Cross-Framework Mapping

- "Map our Art. 9 risk management system to ISO 42001 controls."
- "How does the NIST AI RMF map to EU AI Act high-risk obligations?"
- "Where does Art. 10 data governance intersect with GDPR Art. 5 data minimisation?"

---

## 4. How to Use the Skill

### Installation

1. Download `eu-ai-act.skill` from this folder.
2. In Claude, go to **Settings → Skills**.
3. Click **Upload Skill** and select `eu-ai-act.skill`.
4. The skill is now active across your Claude sessions.

### Triggering the Skill

The skill activates automatically when EU AI Act topics arise. No special command is needed.
Example phrases that trigger it:

- *"EU AI Act compliance"* or *"Regulation (EU) 2024/1689"*
- *"high-risk AI system"*, *"Annex III"*, *"prohibited AI practices Art. 5"*
- *"GPAI model obligations"*, *"systemic risk AI"*, *"10²⁵ FLOPs threshold"*
- *"CE marking AI"*, *"EU AI database registration"*, *"notified body AI"*
- *"AI Act conformity assessment"*, *"Art. 9 risk management"*, *"Art. 26 deployer"*
- *"AI Act penalties"*, *"AI Office"*, *"AI system classification"*

### Example Prompts

```
Classify our AI system: it analyses job applicants' CVs and ranks them for shortlisting.
The system was trained on historical hiring data. We deploy it as an HR tool sold to
enterprise customers across the EU. Apply the full 8-step EU AI Act workflow — start
with role identification, run the Art. 5 prohibited practice screen, determine risk tier,
and list all applicable obligations.
```

```
We are a GPAI model provider. Our model was trained using 3×10²⁵ FLOPs of compute.
We release it under a commercial licence (not open-source). Identify:
(1) whether we cross the Art. 51 systemic risk threshold,
(2) all Art. 53 universal GPAI obligations,
(3) all Art. 55 systemic risk additional obligations,
(4) what the Codes of Practice pathway means for our compliance timeline.
```

```
Produce a comprehensive gap analysis for our high-risk AI system (Annex III Point 4 —
employment and workers management) against all mandatory Arts. 8–17 and Art. 26 obligations.
Use a table with: Requirement | Article | Status (Met/Partial/Gap) | Action Required.
```

```
Our AI system performs real-time remote biometric identification for access control at
our company premises. Is this prohibited under Art. 5(1)(h)? What is the scope of
the law enforcement exception and does a private employer benefit from it?
```

```
Map the EU AI Act high-risk obligations to ISO 42001:2023 controls and NIST AI RMF
functions. Produce a three-column mapping table showing: EU AI Act Article | ISO 42001
Control | NIST AI RMF Function/Category.
```

---

## 5. Skill Implementation Details

### Architecture

```
eu-ai-act/
├── SKILL.md                              # Core skill — 8-step workflow, risk tier framework,
│                                         #   prohibited practices (Art. 5), compliance timeline,
│                                         #   penalty schedule (Art. 99), response formats
└── references/
    ├── risk-classification.md            # Full Annex III use case areas (8 points), Annex I
    │                                     #   sectoral laws, Art. 6 classification rules,
    │                                     #   prohibited practices detail, limited-risk
    │                                     #   transparency obligations (Art. 50)
    ├── obligations-high-risk.md          # Detailed Arts. 9–17 and 26 requirements,
    │                                     #   conformity assessment paths (Arts. 43–48),
    │                                     #   EU AI database (Arts. 49, 60, 71)
    └── gpai-governance.md                # GPAI model obligations (Arts. 51–55), governance
                                          #   structure (AI Office, AI Board, scientific panel),
                                          #   market surveillance, post-market monitoring,
                                          #   serious incident reporting, cross-framework
                                          #   mapping (ISO 42001, NIST AI RMF, GDPR),
                                          #   key Art. 3 definitions
```

### What's in SKILL.md

- **Identity and scope**: Expert EU AI Act compliance advisor with knowledge of Regulation (EU) 2024/1689, all Annexes, and Recitals
- **8-Step Workflow**: Scope/role identification → AI system classification → prohibited practices screen → risk tier determination → high-risk obligations → conformity assessment → GPAI obligations → post-market monitoring
- **Response format guidance**: Structured formats for classification questions, obligation questions, gap assessments, GPAI questions
- **Compliance timeline**: Phase-in dates for each obligation cluster (Feb 2025, Aug 2025, Aug 2026, Aug 2027)
- **Penalty schedule (Art. 99)**: Three penalty tiers by violation type with SME/startup provisions

### What's in the reference files

| File | Contents |
|------|----------|
| `risk-classification.md` | Full Annex III — all 8 high-risk use case areas with specific examples; Annex I sectoral product safety laws; Art. 6(1) Path A and 6(2) Path B classification rules; non-high-risk exceptions; all 8 prohibited practices (Art. 5) with narrow exceptions; limited-risk transparency obligations (Art. 50) for chatbots, synthetic media, and emotion recognition |
| `obligations-high-risk.md` | Detailed implementation guidance for Arts. 9–17 (risk management system, data governance, technical documentation, logging, transparency, human oversight, accuracy/robustness/cybersecurity, provider obligations, QMS); Art. 26 deployer obligations; conformity assessment pathways (Annex VI self-assessment, Annex VII notified body); EU AI database registration (Arts. 49, 60, 71); Declaration of Conformity and CE marking |
| `gpai-governance.md` | GPAI model Art. 3(63) definition; Art. 51 systemic risk threshold (10²⁵ FLOPs); Art. 53 universal obligations (Annex XI/XII documentation, copyright policy, training data summary); open-source exception scope; Art. 55 systemic risk obligations (model evaluation, adversarial testing, incident reporting, cybersecurity); AI Office, AI Board, and scientific panel governance structure; market surveillance authorities; post-market monitoring (Art. 72); serious incident reporting (Art. 73); ISO 42001, NIST AI RMF, and GDPR cross-framework mapping |

### Inputs used to build the skill

| Source | Description |
|--------|-------------|
| Regulation (EU) 2024/1689 (EU AI Act) | Full text including all 113 Articles, 13 Annexes, and 180 Recitals |
| Annex I — EU product safety legislation | Sectoral laws triggering high-risk Path A classification |
| Annex III — High-risk AI use cases | All 8 use case areas with sub-points |
| Annex IV — Technical documentation | Required content for high-risk system documentation |
| Annex VI/VII — Conformity assessment | Self-assessment and notified body procedures |
| Annex XI/XII — GPAI documentation | Technical documentation and downstream provider information for GPAI models |
| EU AI Act Codes of Practice (draft) | GPAI compliance pathway guidance |
| ISO 42001:2023 | AI management system standard for cross-framework mapping |
| NIST AI RMF 1.0 | AI risk management framework for cross-framework mapping |
| GDPR (EU) 2016/679 | Cross-reference for Art. 10 data governance and automated decision-making |

### Skill trigger phrases

`EU AI Act`, `Regulation (EU) 2024/1689`, `AI Act compliance`, `high-risk AI system`,
`Annex III AI`, `prohibited AI practices`, `Art. 5 AI Act`, `Art. 6 risk classification`,
`Art. 9 risk management system`, `Art. 10 data governance`, `Art. 14 human oversight`,
`Art. 26 deployer obligations`, `Art. 50 transparency`, `Art. 99 AI Act penalties`,
`GPAI model`, `general purpose AI`, `systemic risk AI`, `10²⁵ FLOPs`, `AI Office`,
`European AI Board`, `notified body AI`, `CE marking AI system`, `EU AI database`,
`conformity assessment AI`, `AI Act gap analysis`, `AI system classification`,
`biometric AI prohibited`, `social scoring EU`, `real-time RBI`

---

## 6. Author

**Hemant Naik**
[LinkedIn](https://www.linkedin.com/in/tanaji-naik/) · [hemant.naik@gmail.com](mailto:hemant.naik@gmail.com)

Skill version: 1.0.0 — May 2026
