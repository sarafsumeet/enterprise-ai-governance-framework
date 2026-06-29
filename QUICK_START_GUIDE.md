# Quick Start Guide: Assessment to Playbook Implementation

**Get from "I have a governance framework" to "We have working AI governance" in 90 days.**

---

## 🎯 Your 90-Day Roadmap

### **Week 1-2: Assess Your Current State**

**Time Required:** 6-8 hours (can be done in 2 sessions)

#### **Step 1: Complete the Assessment (2-4 hours)**
1. Open **[Excel Template](https://1drv.ms/x/c/8029e0f5e20b224c/IQAtzlhX8EX0To2nuEGL0SpVAc_9EyAq4gHp34siKYRvYSQ?e=Vvat1H)** in your browser
2. Pick your **primary sector** (Banking, Insurance, Manufacturing, Automobile, Telecom, or Utility)
3. For each control, score 1-5:
   - **1** = Ad hoc (inconsistent, informal)
   - **2** = Repeatable (some process, not documented)
   - **3** = Defined (documented, widely followed)
   - **4** = Managed (metrics tracked, proactive)
   - **5** = Optimized (continuous improvement)
4. Add brief evidence in Notes column
5. Check **Summary** sheet for your overall governance score

**Example Score:**
```
Data Governance: 2.5 (Need improvement)
Model Lifecycle: 3.0 (Adequate)
Risk & Compliance: 2.0 (Critical gap)
Governance & Culture: 2.8 (Needs work)
Infrastructure & Security: 3.2 (Acceptable)
Stakeholder & Transparency: 2.2 (High risk)
──────────────────────────
Overall: 2.6/5 (Below Industry Standard)
```

#### **Step 2: Identify Top 3 Gaps (1-2 hours)**
From your assessment:
1. Find controls scoring 1-2 (lowest priority)
2. Circle your top 3 governance gaps
3. Write them down:
   - Gap 1: _______________________
   - Gap 2: _______________________
   - Gap 3: _______________________

#### **Step 3: Understand Your Regulatory Requirements (2-4 hours)**

**If Banking:** Read `SECTOR_MAPPING.md` → APRA CPS 234 section  
**If Insurance:** Read `SECTOR_MAPPING.md` → Solvency II section  
**If Manufacturing/Auto/Telecom/Utility:** Read `EXTENDED_SECTOR_MAPPING.md` → Your sector

**Key Question:** Which controls map to your regulatory requirements?

**Example:**
```
Regulatory Requirement: APRA CPS 234 - Model Risk Assessment
Our Assessment Gap: Model Risk Assessment scored 1.5/5
Required Playbook Action: Implement AI System Registry (Playbook Section 2)
```

---

### **Week 3-4: Design Your Playbook Implementation**

**Time Required:** 8-10 hours (divide across 2 weeks)

#### **Step 4: Read the AI Playbook (2-3 hours)**
1. Read **AI_PLAYBOOK.md** Section 1 (Executive Summary)
2. Skim all sections to understand structure
3. Focus on sections matching your top 3 gaps

#### **Step 5: Map Playbook to Your Gaps (3-4 hours)**

Create a simple table:

| Your Gap | Playbook Section | Implementation Task | Owner | Timeline |
|---|---|---|---|---|
| No AI System Registry | Section 2 | Create registry template + survey | CIO | Week 4 |
| Weak risk classification | Section 3 | Apply risk tiers to all AI systems | Security | Week 4-5 |
| No LLM Gateway | Section 4 | Design gateway architecture | Engineering | Week 5-6 |

#### **Step 6: Draft Implementation Plan (2-3 hours)**

**For Each Gap:**
```
Gap: "No AI System Registry"
Playbook Reference: Section 2

Current State: 
- No centralized tracking of AI systems
- Marketing deployed chatbot without approval
- No visibility into "Shadow AI"

Desired State (Score 4/5):
- Registry captures all AI systems
- Monthly governance committee reviews
- Metrics tracked and reported

Implementation:
1. Use Playbook Section 2 template
2. Survey all departments for AI systems
3. Classify by data type and risk tier
4. Create dashboard for ongoing tracking
5. Establish quarterly review cadence

Timeline: 4-6 weeks
Owner: CIO
Resources: 1 FTE + stakeholders from 5 departments
```

---

### **Week 5-8: Build & Implement**

**Time Required:** 20-30 hours over 4 weeks

#### **Step 7: Implement Gap #1 (Highest Priority)**

**Example: AI System Registry**

**Deliverables:**
- [ ] Registry template (spreadsheet or database)
- [ ] Department survey (identify all AI systems)
- [ ] Classification framework (data types, risk tiers)
- [ ] First version of registry with 10+ AI systems
- [ ] Governance committee review process

**Weekly Milestones:**
```
Week 5:
- [ ] Create registry template
- [ ] Draft survey questions
- [ ] Brief department heads

Week 6:
- [ ] Collect responses (due end of week)
- [ ] Classify systems by risk tier
- [ ] Create preliminary registry

Week 7:
- [ ] Review with security team
- [ ] Identify gaps/missing systems
- [ ] Finalize registry v1.0

Week 8:
- [ ] Present to governance committee
- [ ] Establish quarterly review cadence
- [ ] Document process in playbook
```

**How to Use Playbook:**
- Section 2: Use matrix template to structure registry
- Add columns: System Name, Owner, Data Types, Risk Tier, Controls
- Reference Section 3 for risk tier definitions
- Store in shared location (spreadsheet, database, or wiki)

#### **Step 8: Implement Gap #2 (Medium Priority)**

Repeat Step 7 for your second gap (typically: multi-tier risk model or LLM Gateway design).

**Time:** Weeks 5-10

#### **Step 9: Implement Gap #3 (Foundation for Later)**

Plan implementation but may not fully execute in 90 days.

**Time:** Weeks 8-12 (plan), Execution in Month 2+

---

### **Week 9-12: Measure, Document & Report**

**Time Required:** 8-10 hours

#### **Step 10: Re-Assess Your Governance (2-4 hours)**

Same as Step 1, but now:
1. Open Excel template
2. Score same sector/controls again
3. Compare to baseline (Week 1-2)

**Expected Improvement:**
```
Week 1-2 Score: 2.6/5
Week 9-12 Score: 3.4/5
Improvement: +0.8 (31% increase)

Data Governance: 2.5 → 3.5 (better registry, lineage tracking)
Model Lifecycle: 3.0 → 3.2 (updated validation procedures)
Risk & Compliance: 2.0 → 3.2 (new registry, risk tiers implemented)
Governance & Culture: 2.8 → 3.4 (governance committee established)
Infrastructure & Security: 3.2 → 3.3 (LLM gateway designed)
Stakeholder & Transparency: 2.2 → 3.0 (board reporting created)
```

#### **Step 11: Document Your Implementation (2-3 hours)**

Create a **Governance Implementation Playbook** for your organization:

```
Our AI Governance Implementation (Jan-Mar 2026)

1. AI System Registry
   Status: ✓ Complete (v1.0)
   Evidence: Spreadsheet with 25+ AI systems classified
   Governance: Quarterly review by steering committee
   
2. Risk Tier Classification
   Status: ✓ Complete (initial)
   Evidence: All 25 systems classified as Tier 1-4
   Governance: Monthly security review of Tier 1-2 systems
   
3. LLM Gateway
   Status: 🔄 In Progress (design complete, building)
   Evidence: Architecture document, technical specifications
   Timeline: Deployment in April 2026
   
Next Steps:
- Implement LLM Gateway (weeks 12-16)
- Build audit trail procedures (weeks 12-20)
- Establish incident response (weeks 16-20)
```

#### **Step 12: Report to Board / Executive Team (2-3 hours)**

Use **Assessment Summary** to create board presentation:

```
Q1 2026 AI Governance Report
───────────────────────────

Maturity Scorecard:
Current State (End of Q1): 3.4/5
Baseline (Start of Q1): 2.6/5
Progress: +0.8 (31% improvement)

Key Initiatives Completed:
✓ AI System Registry (24 systems cataloged)
✓ Risk Tier Classification (Tier 1-4 model)
✓ Governance Committee (quarterly meetings established)

Next Quarter Priorities:
🔄 LLM Gateway implementation
🔄 Audit trail procedures
🔄 Incident response plan

Regulatory Status:
✓ APRA CPS 234 progress tracking (Banking sector)
✓ Ready for Q2 compliance assessment

Board Action Items:
- Approve LLM Gateway architecture
- Allocate resources for Month 2 initiatives
- Review quarterly governance updates
```

---

## 📊 Playbook Sections at a Glance

### **When to Use Each Section**

| Playbook Section | Your Use Case | Implementation Timeline |
|---|---|---|
| **Section 1: Executive Summary** | Understanding AI governance risks | Day 1 (1 hour) |
| **Section 2: AI System Registry** | Eliminating "Shadow AI" | Week 4-8 (implement) |
| **Section 3: Multi-Tier Risk Model** | Classifying AI applications | Week 5-9 (implement) |
| **Section 4: LLM Gateway & Guardrails** | Securing data boundaries | Week 8-12 (design) → Month 2 (build) |
| **Section 5+: Security & Audit** | Establishing controls | Month 2+ (ongoing) |

### **By Governance Maturity Level**

**If your score is 1-2/5 (Ad Hoc):**
→ Start with Section 2 (AI System Registry)
→ Focus: Get visibility into all AI systems

**If your score is 2.5-3.5/5 (Defined):**
→ Move to Section 3 & 4 (Risk Tiers + LLM Gateway)
→ Focus: Formalize risk management & data security

**If your score is 3.5-4.5/5 (Managed):**
→ Implement Sections 5+ (Audit, Incident Response)
→ Focus: Automation, monitoring, continuous improvement

**If your score is 4.5-5/5 (Optimized):**
→ Extend framework (add sectors, customize controls)
→ Focus: Industry leadership, community contribution

---

## 🛠️ Sample Implementation: AI System Registry

**Here's exactly how to implement Playbook Section 2 in your organization:**

### **Phase 1: Design (Week 4, 4 hours)**

**Create Registry Template:**
```
AI System Name | Department | Owner | Data Classification | Risk Tier | Controls Required | Status
───────────────────────────────────────────────────────────────────────────────────────────────
Customer Support Bot | Customer Ops | Jane Smith | PII | Tier 2 (High) | PII masking, audit trail | Active
Q1 Forecaster | Finance | Bob Jones | Internal | Tier 3 (Limited) | Access control, usage tracking | Pilot
Marketing Summarizer | Marketing | Alice Chen | Public | Tier 4 (Minimal) | Standard access mgmt | Active
```

**Send Survey to Departments:**
```
AI System Registry Survey (Due: End of Week 5)

For each AI system deployed in your department, please provide:
1. System name & brief description
2. Who owns/maintains it
3. What data does it use? (Public/Internal/Confidential/Restricted)
4. Who are the users? (count)
5. Is it approved by governance/security?
6. When was it deployed?

Examples: ChatGPT integration, Copilot usage, custom ML models, etc.
```

### **Phase 2: Execute (Week 5-7, 12 hours)**

**Collect Responses:**
- Email survey to 10-15 department heads
- Follow up 2x during collection period
- Consolidate responses into registry

**Classify Systems:**
- Apply Playbook Section 3 risk tier definitions
- Work with security team on edge cases
- Document classification rationale

**Create v1.0:**
- Compile 15-25 systems with full details
- Identify gaps (missing systems, unclear ownership)
- Create executive summary

### **Phase 3: Operationalize (Week 8, 4 hours)**

**Establish Governance Process:**
- Schedule monthly security review (Tier 1-2 systems)
- Schedule quarterly steering committee review (all systems)
- Assign registry owner & update process
- Create dashboard for ongoing tracking

**Integrate with Assessment:**
- Map registry to Control: "AI System Cataloging"
- Score as "Defined" (3/5) for having documented process
- Plan for "Managed" (4/5) by adding automation/monitoring

---

## 🎯 Success Metrics (Track These)

### **During Implementation (Monthly)**

| Metric | Target | Owner |
|---|---|---|
| AI Systems Cataloged | 20+ by Week 8 | CIO |
| Systems Classified | 100% by Week 9 | Security |
| Governance Committee Meetings | 1/month starting Week 9 | CIO |
| Audit Trail Logging | Active by Week 12 | Engineering |
| Board Reporting | Scorecard monthly by Week 12 | CIO |

### **By End of 90 Days**

| Milestone | Success Criteria |
|---|---|
| Assessment Score | Improved from 2.6 → 3.4+ (1 point increase) |
| AI System Registry | 20+ systems cataloged, classified, actively monitored |
| Risk Classification | All Tier 1-2 systems have documented controls |
| Governance Cadence | Monthly security reviews, quarterly steering committee |
| Board Reporting | Maturity scorecard presented & tracked |
| Regulatory Alignment | Gap analysis completed, compliance plan drafted |

---

## 📋 Implementation Checklist

### **Week 1-2: Assessment**
- [ ] Assessment completed (all controls scored)
- [ ] Summary sheet shows your baseline score
- [ ] Top 3 gaps identified
- [ ] Regulatory requirements understood

### **Week 3-4: Planning**
- [ ] AI_PLAYBOOK.md read (at least Sections 1-4)
- [ ] Playbook mapped to your 3 gaps
- [ ] Implementation plan drafted
- [ ] Budget & resources allocated

### **Week 5-8: Implementation (Gap #1)**
- [ ] Deliverable #1 completed
- [ ] Deliverable #2 completed
- [ ] Process documented
- [ ] Governance committee aware

### **Week 8-10: Implementation (Gap #2)**
- [ ] Design phase complete
- [ ] Execution underway
- [ ] Stakeholders engaged
- [ ] Progress tracked

### **Week 9-12: Measurement & Reporting**
- [ ] Re-assessment completed
- [ ] Improvement documented (score increased)
- [ ] Implementation playbook created
- [ ] Board presentation prepared
- [ ] Next quarter priorities defined

---

## 📞 If You Get Stuck

| Question | Reference |
|---|---|
| **"How do I score a control?"** | IMPLEMENTATION_GUIDE.md → Scoring Rubric |
| **"What's my risk tier?"** | AI_PLAYBOOK.md Section 3 → Risk Tier Definitions |
| **"How do I implement the registry?"** | This guide → "Sample Implementation" section |
| **"Which regulations apply to me?"** | SECTOR_MAPPING.md or EXTENDED_SECTOR_MAPPING.md |
| **"How do I build an LLM Gateway?"** | AI_PLAYBOOK.md Section 4 → Technical Specifications |
| **"What should I tell the board?"** | This guide → "Board Reporting" example |

---

## 🚀 Ready to Start?

1. **Today:** Open [Excel Template](https://1drv.ms/x/c/8029e0f5e20b224c/IQAtzlhX8EX0To2nuEGL0SpVAc_9EyAq4gHp34siKYRvYSQ?e=Vvat1H) and review your sector
2. **Week 1:** Complete assessment (Steps 1-3)
3. **Week 3:** Draft implementation plan (Steps 4-6)
4. **Week 5:** Start building (Steps 7-9)
5. **Week 12:** Measure progress & report (Steps 10-12)

**This is achievable. You've got this.** 🎯

---

**Last Updated:** June 2026  
**Author:** Sumeet Saraf | AI Governance Leader
