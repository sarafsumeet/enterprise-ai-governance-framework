# AI Governance Audit Framework

An open-source, **sector-specific governance assessment tool** for financial services, insurance, and SaaS organizations building and deploying AI/ML systems at scale.

## Overview

This framework provides a **scored audit matrix** aligned with regulatory and industry standards, enabling organizations to:

- **Assess** current governance maturity across four critical areas: Data, Model Lifecycle, Risk & Compliance, and Culture
- **Benchmark** against industry best practices (APRA CPS 234, Solvency II, SOX 404, ISO 27001)
- **Identify gaps** in AI governance and prioritize remediation
- **Generate board-ready reports** that translate technical governance into business language

## The Problem

Most AI governance frameworks are either:
- **Too academic** — hundreds of pages, hard to operationalize
- **Too generic** — don't map to specific regulatory contexts
- **Too abstract** — lack concrete assessment criteria

This framework bridges that gap with **scored, sector-specific checklists** that hiring managers, auditors, and executives can actually use today.

## Who This Is For

- **CIOs & AI Governance Leads**: Assess your organization's governance maturity in 2-4 hours
- **Risk & Compliance Officers**: Map your controls to APRA CPS 234, Solvency II, SOX 404, ISO 27001
- **Hiring Managers & Board Members**: Quickly evaluate AI governance maturity at a target company
- **Open source contributors**: Fork, adapt, and extend for your industry

## What's Included

### 1. **Assessment Template** (`AI_Governance_Audit_Framework_Extended.xlsx`)
- **Interactive Version:** [👉 Open Workbook in Excel for Web](https://1drv.ms/x/c/8029e0f5e20b224c/IQAtzlhX8EX0To2nuEGL0SpVAc_9EyAq4gHp34siKYRvYSQ?e=Vvat1H)
- **Six sector-specific sheets:** Banking, Insurance, Manufacturing, Automobile, Telecom, and Utility.
- **16 scored controls** across 4 governance areas with a summary dashboard.

### 2. **Documentation**
- **This README**: Overview and getting started
- **IMPLEMENTATION_GUIDE.md**: Step-by-step assessment walkthrough
- **SECTOR_MAPPING.md**: Regulatory alignment (CPS 234, Solvency II, SOX, ISO 27001)

### 3. **Sample Report** (Included in outputs folder)
- Pre-filled audit with realistic scores
- Narrative summary suitable for board presentation
- Gap analysis and remediation roadmap

---

## Quick Start (15 minutes)

### Step 1: Download & Open
1. Download `AI_Governance_Audit_Framework.xlsx`
2. Open in Excel, Google Sheets, or LibreOffice
3. Go to the **README sheet** for orientation

### Step 2: Choose Your Sector
Click into one of three tabs:
- **Banking** (APRA CPS 234 aligned)
- **Insurance** (Solvency II aligned)
- **SaaS** (SOX 404 / ISO 27001 aligned)

### Step 3: Score Your Controls
For each control (rows 4–19), enter a **maturity level 1–5**:

| Level | Definition | Example |
|-------|-----------|---------|
| **1 — Ad Hoc** | No formal process; inconsistent application | Data quality checks are manual and irregular |
| **2 — Repeatable** | Basic process exists; followed by some teams | Data validation rules exist but not automated |
| **3 — Defined** | Documented process; widely followed | Formal data quality SLA with monitoring |
| **4 — Managed** | Metrics tracked; proactive improvement | Dashboard alerts on data drift; monthly reviews |
| **5 — Optimized** | Continuous improvement; integrated with strategy | Automated quality gates in CI/CD; AI-driven anomaly detection |

### Step 4: Review Summary
1. Go to the **Summary** sheet
2. Copy your average scores from the sector sheet
3. Read your **Overall Governance Score** (auto-calculated)
4. Identify lowest-scoring areas for remediation

### Step 5: Generate Narrative (Optional)
Use the template in `IMPLEMENTATION_GUIDE.md` to draft a board-ready report from your scores.

---

## Control Areas

### 1. **Data Governance**
Ensures the data feeding your AI models is high-quality, traceable, and compliant.

**Key Controls:**
- Data Quality & Validation (completeness, accuracy, timeliness)
- Data Lineage & Traceability (end-to-end source tracking)
- Metadata Management (data dictionary, ownership, sensitivity)
- Retention & Archival Policy (legal hold, deletion)

**Why It Matters:** Poor data = poor models. Regulators now focus on data quality as a foundational AI governance component.

---

### 2. **Model Lifecycle**
Governs AI models from development through retirement, ensuring they're validated, deployed safely, and monitored continuously.

**Key Controls:**
- Model Development & Testing (methodology, code review, unit tests)
- Model Validation (independent testing, performance benchmarks, edge case analysis)
- Deployment & Version Control (change management, audit trail, rollback procedures)
- Monitoring & Drift Detection (live performance tracking, alert thresholds)

**Why It Matters:** Most model failures happen in production, undetected. Lifecycle governance catches drift early.

---

### 3. **Risk & Compliance**
Addresses AI-specific risks: explainability, fairness, bias, regulatory alignment.

**Key Controls:**
- Model Risk Assessment (BCBS 239 for banks; residual risk rating)
- Explainability & Interpretability (LIME, SHAP, or domain-expert review)
- Fairness & Bias Detection (protected attribute analysis, disparate impact testing)
- Regulatory Compliance Mapping (APRA CPS 234, GDPR, Solvency II, SOX)

**Why It Matters:** Regulators care about fairness, explainability, and documented risk. This is where AI governance turns into AI *ethics*.

---

### 4. **Governance & Culture**
Embeds AI governance into organizational culture, roles, and accountability.

**Key Controls:**
- AI Ethics & Responsible AI Framework (principles, decision-making)
- Change Management & Audit Trails (versioning, rollback, accountability)
- Stakeholder Training & Communication (AI literacy, transparency)
- Third-Party & Vendor Risk (model audit, SLA enforcement)

**Why It Matters:** Governance isn't a compliance checkbox—it's a culture shift. This area drives adoption and sustainability.

---

## Regulatory Alignment

### Banking: APRA CPS 234
Aggregated Prudential Supervision 234 (Australia) requires:
- Model governance framework
- Independent validation
- Board oversight
- Remediation of model defects

**This framework maps to:**
- CPS 234 pillar 1: Model development & validation
- CPS 234 pillar 2: Data governance
- CPS 234 pillar 3: Risk management
- CPS 234 pillar 4: Compliance & reporting

### Insurance: Solvency II
Solvency II (EU/UK) requires:
- Own Risk and Solvency Assessment (ORSA)
- Model validation in underwriting & claims
- Data quality for reserving models
- Governance framework (8.1, 8.2)

**This framework maps to:**
- Art. 8.1: Governance system
- Art. 8.2: Model governance
- Art. 18: Own funds; Risk management

### SaaS / Tech: SOX 404 & ISO 27001
SOX 404 requires effective internal controls; ISO 27001 requires information security.

**This framework maps to:**
- SOX 404: IT controls over AI model development/deployment
- ISO 27001: Data governance, access control, encryption
- NIST AI RMF: Risk management framework for AI

---

## How to Extend This Framework

### Add Your Own Sector
1. Copy the Banking sheet
2. Rename to your sector (e.g., "Healthcare", "Manufacturing")
3. Replace sub-controls with sector-specific governance areas
4. Update the Summary sheet to reference new control areas

### Customize Controls
- Keep the **4 main areas** (Data, Model, Risk, Culture)
- Add/remove **sub-controls** based on your industry
- Document your rationale in a comment cell

### Export for Third-Party Audit
1. Fill in scores for your sector
2. Export to PDF (Print → Save as PDF in Excel)
3. Share with auditors/consultants
4. Iterate based on their feedback

---

## How This Was Built

This framework is based on:
- **APRA CPS 234** (prudential supervision of AI/ML models)
- **DAMA DMBOK 2** (Data Management Body of Knowledge)
- **NIST AI Risk Management Framework**
- **ISO/IEC 42001** (AI Management Systems)
- **10+ years of enterprise AI governance implementation** across banking, insurance, and SaaS

It's opinionated—we've prioritized the controls that actually matter in production environments, not theoretical best practices.

---

## Sample Assessment

A pre-filled example is available: **sample_audit_report.pdf**

This shows:
- A banking organization scoring itself (average: 3.2 / 5)
- Gaps in specific areas (Model Monitoring = 2, Fairness Testing = 1)
- Remediation priorities (30/60/90 day roadmap)
- Board-ready narrative summary

---

## License

MIT License. Feel free to use, modify, and distribute this framework in your organization.

---

## Contributing

Found a gap? Want to add a sector? Submit a pull request or open an issue.

---

## Questions?

- **Getting Started**: See `IMPLEMENTATION_GUIDE.md`
- **Regulatory Mapping**: See `SECTOR_MAPPING.md`
- **Scoring Help**: Refer to control definitions in each sector sheet

---

**Built by:** Sumeet Saraf | AI Governance & Data Governance Leader  
**Contact:** saraf.sumeet@gmail.com | +61 470 701 263  
**Last Updated:** June 2026

---

## Quick Reference: Scoring Your Controls

### What Does a 1 Look Like?
- No formal data quality process
- Models deployed without validation
- No explainability documentation
- Audit trail incomplete or missing

**Remediation:** This is urgent. You're exposed to regulatory and reputational risk.

### What Does a 3 Look Like?
- Defined process; followed by most teams
- Models validated, but not independently
- Some explainability work; not systematic
- Audit trail exists but incomplete

**Remediation:** You're baseline. Now focus on standardization and automation.

### What Does a 5 Look Like?
- Fully automated data quality gates in CI/CD
- Independent model validation; third-party review
- Explainability baked into model selection
- Complete audit trail; compliance-ready

**Remediation:** Maintain and refine. Look for emerging risks.

---

## Testimonials

*"This framework got us from vague AI governance to a scored, auditable maturity model in 3 hours."* — CIO, Banking

*"We used this to prepare for APRA CPS 234 audit. Regulators asked for exactly this level of detail."* — Head of Risk, Insurance

*"It's opinionated in a good way. Doesn't have 200 controls; just the ones that matter."* — Engineering Lead, SaaS
