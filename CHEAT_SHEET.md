# AI Governance Framework: One-Page Cheat Sheet

---

## 🎯 ASSESSMENT TEMPLATE
**[👉 Open in Excel](https://1drv.ms/x/c/8029e0f5e20b224c/IQAtzlhX8EX0To2nuEGL0SpVAc_9EyAq4gHp34siKYRvYSQ?e=Vvat1H)**

**6 Sectors:** Banking (APRA) | Insurance (Solvency II) | Manufacturing (ISO 9001) | Automobile (SOTIF) | Telecom (GDPR) | Utility (NERC)

**6 Governance Areas:**
1. Data Governance (quality, lineage, metadata, retention)
2. Model Lifecycle (dev, validation, deployment, monitoring)
3. Risk & Compliance (model risk, explainability, fairness, regulatory)
4. Governance & Culture (ethics, audit, training, third-party)
5. Infrastructure & Security (model serving, data pipelines, access)
6. Stakeholder & Transparency (board reporting, external audit, docs)

**Scoring:** 1=Ad Hoc | 2=Repeatable | 3=Defined | 4=Managed | 5=Optimized

**Time:** 2-4 hours to assess entire organization

---

## 📖 PLAYBOOK: AI SYSTEM REGISTRY (Section 2)

**Purpose:** Eliminate "Shadow AI" — catalog ALL AI systems company-wide

| AI System | Department | Data Type | Risk Tier | Controls |
|---|---|---|---|---|
| Customer Bot | Customer Ops | Confidential PII | **Tier 2 (High)** | PII masking, audit trail |
| Q1 Forecast | Finance | Internal | **Tier 3 (Limited)** | Access control, logging |
| Marketing Summarizer | Marketing | Public | **Tier 4 (Minimal)** | Standard access mgmt |

**Timeline:** 4-6 weeks  
**Owner:** CIO + Security team  
**Governance:** Monthly security review, quarterly steering committee

---

## 🚨 PLAYBOOK: RISK TIER MODEL (Section 3)

| Tier | Definition | Risk Level | Key Controls |
|---|---|---|---|
| **Tier 1** | Prohibited — Violates data/security rules | BLOCK | Immediate shutdown, escalate to CISO |
| **Tier 2** | High Risk — Customer PII, financials, critical decisions | HIGH | Real-time PII masking, encrypted pipelines, human review |
| **Tier 3** | Limited Risk — Internal productivity tools | MEDIUM | Privacy toggles enabled, identity logging, usage tracking |
| **Tier 4** | Minimal Risk — Public data on local infrastructure | LOW | Standard access management |

**Apply to:** Every AI system in your registry

---

## 🔒 PLAYBOOK: LLM GATEWAY (Section 4)

**Three-Layer Architecture:**

```
User Prompt
    ↓
[Layer 1: PII Masker]
  Strip: SSN, Credit Cards, Emails, Names
  Example: "Jane Smith's SSN 123-45-6789" → "Jane Smith's SSN [REDACTED]"
    ↓
[Layer 2: Topic Blocker]
  Block: Code repos, financial models, customer databases
  Prevent exfiltration of company-specific data
    ↓
[Layer 3: Secured API]
  Rate-limit | Zero Data Retention (ZDR) | Audit logging
  Local VPC storage only (no cloud training)
    ↓
Audited Response + Provenance Tracking
```

**For Engineering:** Build gateway with all 3 layers  
**For Security:** Monitor logs daily for blocked prompts  
**For Compliance:** Evidence for audit trail requirements

---

## 📊 REGULATION MAP

| Regulation | Sector | Assessment Control | Playbook Action |
|---|---|---|---|
| APRA CPS 234 | Banking | Model Risk Assessment | AI System Registry + Risk Tiers |
| Solvency II | Insurance | Model Validation | LLM Gateway + Topic Blocking |
| ISO 9001 | Manufacturing | Data Quality | Registry + Classification |
| SOTIF | Automobile | Safety-Critical Validation | Risk Tier engineering gates |
| GDPR | All | Data Privacy | PII Masking Layer 1 |
| NIST AI RMF | All | Governance | Full framework compliance |
| ISO 42001 | All | AI Management System | Assessment + Playbook ops |

---

## 🎯 QUICK REFERENCE: SCORING CONTROLS

**Score 1 (Ad Hoc):**
- No formal process
- Inconsistent execution
- No documentation

**Score 2 (Repeatable):**
- Basic process exists
- Partially documented
- Hit-or-miss execution

**Score 3 (Defined):**
- Process documented
- Widely followed
- Regular monitoring

**Score 4 (Managed):**
- Metrics tracked
- Proactive improvement
- Data-driven decisions

**Score 5 (Optimized):**
- Continuous improvement
- Innovation & automation
- Industry-leading practices

---

## 📋 90-DAY IMPLEMENTATION ROADMAP

| Phase | Weeks | Focus | Deliverables |
|---|---|---|---|
| **Assess** | 1-2 | Current state | Baseline score (typically 2-3/5) |
| **Plan** | 3-4 | Identify gaps | Implementation plan for top 3 gaps |
| **Build Gap #1** | 5-8 | Execute highest priority | AI System Registry v1.0 |
| **Build Gap #2** | 8-10 | Execute medium priority | Risk Tier classification |
| **Build Gap #3** | 10-12 | Plan lowest priority | LLM Gateway design (build in Month 2) |
| **Measure** | 9-12 | Re-assess & report | Improved score (3.5+/5), board presentation |

**Expected Outcome:** Score improvement from ~2.6/5 → 3.4/5 (30% in 90 days)

---

## ⚡ IMMEDIATE ACTIONS (Today/This Week)

1. **[Open Assessment Template](https://1drv.ms/x/c/8029e0f5e20b224c/IQAtzlhX8EX0To2nuEGL0SpVAc_9EyAq4gHp34siKYRvYSQ?e=Vvat1H)** (5 min to open)
2. **Pick your sector** (Banking, Insurance, Mfg, Auto, Telecom, Utility)
3. **Score 3-4 controls** to get a feel for the assessment (15 min)
4. **Read Playbook Section 1** (Executive Summary) (15 min)
5. **Identify your top 3 gaps** (30 min)

**Total Time: 1.5 hours to understand where you stand**

---

## 📞 DOCUMENT MAP

| Question | Go To |
|---|---|
| How do I score? | IMPLEMENTATION_GUIDE.md + Examples |
| How do I deploy? | QUICK_START_GUIDE.md (90-day roadmap) |
| What's my regulation? | SECTOR_MAPPING.md (Banking/Ins) or EXTENDED_SECTOR_MAPPING.md |
| How do I implement registry? | QUICK_START_GUIDE.md + AI_PLAYBOOK.md Section 2 |
| How do I build LLM gateway? | AI_PLAYBOOK.md Section 4 + Technical specs |
| What do I tell the board? | QUICK_START_GUIDE.md + Example scorecard |

---

## 🎓 LEARNING PATH BY ROLE

**CIO/Chief AI Officer:**
1. Assessment (2h) → Playbook Sections 1-3 (1h) → Implementation Plan (1h)

**Security/Compliance:**
1. Playbook Sections 2-4 (1.5h) → Registry Design (2h) → Gateway Specs (2h)

**Engineering:**
1. Playbook Section 4 (1h) → LLM Gateway Architecture (3-4h) → Testing (2h)

**Audit/Risk:**
1. Assessment (2-4h) → Regulatory Mapping (1-2h) → Evidence Prep (2h)

---

## 🏆 SUCCESS METRICS (Track Weekly)

- [ ] AI Systems Cataloged (target: 20+ by Week 8)
- [ ] Systems Classified (target: 100% by Week 9)
- [ ] Governance Meetings (1/month starting Week 9)
- [ ] Assessment Score Improvement (target: +0.8 points in 90 days)
- [ ] Board Reporting (monthly scorecard)

---

## 🚀 THREE WAYS TO START

**Option A: Quick (1 hour)**
1. Take assessment (interactive template)
2. Get baseline score
3. Identify top 3 gaps

**Option B: Medium (4 hours)**
1. Complete assessment
2. Read Playbook Sections 1-3
3. Draft implementation plan
4. Assign owners

**Option C: Deep (8 hours)**
1. Complete assessment
2. Read full Playbook
3. Read regulatory mapping (your sector)
4. Create detailed 90-day plan
5. Set up governance committee

**Pick one. Start today.** ✅

---

**Framework Version:** 2.0 Extended (6 Sectors, 110+ Controls)  
**Playbook Version:** 1.0 (Operational Framework)  
**Last Updated:** June 2026  
**Author:** Sumeet Saraf | AI Governance Leader  
📧 saraf.sumeet@gmail.com | 📱 +61 470 701 263
