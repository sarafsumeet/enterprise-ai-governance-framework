# AI Governance Audit Framework & Enterprise AI Governance Playbook

**A complete, production-ready governance solution for enterprises deploying AI at scale.**

---

## 📋 Quick Navigation

- **[Interactive Assessment Template](#-interactive-assessment-template)** — Evaluate your governance in 2-4 hours
- **[Enterprise AI Playbook](#-enterprise-ai-governance-playbook)** — Operational framework for AI risk management
- **[Get Started](#-quick-start)** — Choose your path based on your role
- **[Regulatory Alignment](#-regulatory-alignment)** — APRA, Solvency II, SOTIF, GDPR, NERC

---

## 🎯 What This Is

This is a **dual-layered AI governance solution** combining:

1. **Assessment Framework** — Measure your governance maturity across 6 sectors & 110+ controls
2. **Operational Playbook** — Execute governance in production (AI system registry, risk tiers, LLM gateways)

**Use Case:** Organizations deploying Generative AI, LLMs, and autonomous agents need to eliminate "Shadow AI," classify risks, and maintain audit-ready governance without slowing delivery.

---

## 🎬 Interactive Assessment Template

### 👉 **Open in Excel for Web (No Installation Required)**

**[👉 Open Workbook in Excel for Web](https://1drv.ms/x/c/8029e0f5e20b224c/IQAtzlhX8EX0To2nuEGL0SpVAc_9EyAq4gHp34siKYRvYSQ?e=Vvat1H)**

No download, no installation. Works in any browser. Assess your governance maturity in real-time.

### 📊 Template Details

**Six sector-specific sheets:**
- 🏦 **Banking** (APRA CPS 234) — Credit models, AML/KYC, lending AI
- 🏢 **Insurance** (Solvency II) — Underwriting, reserving, claims prediction  
- 🏭 **Manufacturing** (ISO 9001) — Predictive maintenance, quality control, supply chain
- 🚗 **Automobile** (SOTIF, Safety) — Autonomous driving, safety-critical systems, insurance pricing
- 📡 **Telecom** (GDPR, Churn) — Customer churn, fraud detection, network optimization
- ⚡ **Utility** (NERC, Forecasting) — Demand prediction, grid optimization, load management

**What you'll assess:**
- ✅ Data Governance (quality, lineage, metadata, retention)
- ✅ Model Lifecycle (development, validation, deployment, monitoring)
- ✅ Risk & Compliance (model risk, explainability, fairness, regulatory)
- ✅ Governance & Culture (ethics, audit trails, training, third-party risk)
- ✅ Infrastructure & Security (model serving, data pipelines, access control)
- ✅ Stakeholder & Transparency (board reporting, external audit, documentation)

**Maturity Scale:** 1 (Ad Hoc) → 5 (Optimized)

**Time Required:** 2–4 hours to assess your entire organization

---

## 📖 Enterprise AI Governance Playbook

### What It Covers

The **AI Playbook** provides operational procedures for implementing AI governance in production environments. It's designed for:
- **AI Steering Committees** — Defining governance policies
- **Security & Compliance Teams** — Enforcing controls and audit trails
- **Engineering Teams** — Building LLM gateways and guardrails
- **Risk Management** — Classifying AI systems and managing risk

### Core Playbook Sections

#### **1. AI System Registry Matrix**
Eliminate "Shadow AI" by requiring all departments to register AI deployments:
- AI System Name & Business Unit
- Data Classification (Public, Internal, Confidential, Restricted)
- Risk Tier (Prohibited, High, Limited, Minimal)
- Governance Controls Required

**Example:**
```
Customer Support Bot | Customer Operations | Confidential PII | High Risk
→ Requires: Real-time prompt interception, daily drift auditing

Q1 Marketing Summarizer | Marketing | Public/Internal | Minimal Risk
→ Requires: Basic access management, vendor monitoring
```

#### **2. Multi-Tiered AI Risk Classification**

**Tier 1: Prohibited Risk (Immediate Block)**
- Uploading unmasked source code to consumer AI
- Processing raw employee records in untrusted systems
- Actions: Immediate shutdown, escalation to CISO

**Tier 2: High Risk (Strict Engineering Gates)**
- Systems handling customer PII, protected financials, or making business-critical automated decisions
- Controls: Real-time API-layer redaction, encrypted pipelines, human-in-the-loop validation

**Tier 3: Limited Risk (Standard Guardrails)**
- Internal productivity tools (note-takers, summarizers, document processors)
- Controls: Privacy toggles enabled (opt-out of training), identity logging, usage monitoring

**Tier 4: Minimal Risk (Permissive)**
- Open-source models on local infrastructure processing public materials
- Controls: Standard access management

#### **3. LLM Gateway & Guardrail Specifications**

All third-party AI API calls flow through a centralized **LLM Gateway** with three layers:

```
User App Prompt
    ↓
[Layer 1: Regex/Pattern Scanner] ← Strips PII (SSN, credit cards, emails)
    ↓
[Layer 2: Prohibited Topic Evaluator] ← Blocks sensitive business topics
    ↓
[Layer 3: Secured LLM API Call] ← Rate-limited, logged, audited
    ↓
Response (with provenance tracking)
```

**Example Controls:**
- **PII Masking:** `SSN: 123-45-6789` → `SSN: [REDACTED]`
- **Prohibited Topics:** Code repositories, financial models, customer databases
- **API Constraints:** Zero Data Retention (ZDR), local VPC storage only
- **Audit Trail:** Every prompt logged with timestamp, user, data classification

#### **4. Additional Playbook Sections (Included)**

- **Security Incident Response** — Procedures for AI data breaches or prompt injection attacks
- **Audit Trail & Compliance Logging** — Maintaining evidence for regulatory exams
- **Vendor Model Monitoring** — Assessing third-party AI tool governance
- **Data Retention & Deletion** — Compliance with GDPR, privacy laws
- **Training & Awareness** — Governance literacy for all departments

---

## 🚀 Quick Start

### **For CIOs / Governance Leads**

1. **Assess:** Open the [Excel template](https://1drv.ms/x/c/8029e0f5e20b224c/IQAtzlhX8EX0To2nuEGL0SpVAc_9EyAq4gHp34siKYRvYSQ?e=Vvat1H) and score your organization (2-4 hours)
2. **Read:** Review the AI Playbook to understand operational procedures
3. **Implement:** Use Playbook sections to build your AI governance program
4. **Report:** Generate board-ready maturity scorecard from assessment

### **For Security / Compliance Teams**

1. **Catalog:** Create AI System Registry from Playbook Section 2
2. **Classify:** Apply multi-tier risk model (Playbook Section 3) to each AI system
3. **Build:** Implement LLM Gateway using Playbook Section 4 specifications
4. **Monitor:** Establish audit trail procedures and incident response

### **For Engineering Teams**

1. **Understand:** Review LLM Gateway specifications (Playbook Section 4)
2. **Design:** Architecture for API-layer guardrails and redaction patterns
3. **Implement:** Build gateway with three-layer control architecture
4. **Test:** Validate PII masking, topic blocking, rate limiting

### **For Audit / Risk Teams**

1. **Use Assessment:** Track governance maturity scores over time
2. **Document Controls:** Map Playbook procedures to audit requirements
3. **Prepare Evidence:** Build audit-ready documentation from Playbook checklists
4. **Report:** Demonstrate regulatory alignment (APRA, GDPR, NIST AI RMF, ISO 42001)

---

## 🔍 How These Work Together

### **Assessment Framework → Governance Playbook**

```
Assessment Score: 2.8/5 (High Risk) for AI Systems
    ↓
Identified Gap: "No formal AI System Registry"
    ↓
Playbook Section 2: AI System Registry Matrix
    ↓
Action: Create registry with AI System Name, Business Unit, Data Classification, Risk Tier
    ↓
Implementation: Deploy using Playbook templates
    ↓
Re-assess: Score should improve to 3.5+
```

### **Risk Tiers → Governance Controls**

```
Customer Support Chatbot identified as Tier 2 (High Risk)
    ↓
Playbook mandates: Real-time prompt interception, daily drift auditing
    ↓
Engineering team implements LLM Gateway (Section 4)
    ↓
Security team monitors audit logs daily
    ↓
Assessment confirms control is "Defined" (score: 3)
```

---

## 📊 Regulatory Alignment

### **Assessment → Regulatory Proof Points**

| Regulation | Sector | Framework Control | Playbook Implementation |
|---|---|---|---|
| **APRA CPS 234** | Banking | Model Risk Assessment | AI System Registry + Risk Tier classification |
| **Solvency II** | Insurance | Model Validation | LLM Gateway specifications (Layer 2: Topic Blocking) |
| **GDPR** | All | Data Privacy | PII Masking (Layer 1 of LLM Gateway) |
| **SOTIF** | Automobile | Safety-Critical Validation | Multi-tier risk model (Tier 1-2 engineering gates) |
| **NIST AI RMF** | All | Governance Framework | Full Playbook compliance structure |
| **ISO 42001** | All | AI Management System | Assessment + Playbook operational procedures |

### **How to Use for Audit Prep**

1. **Self-Assessment:** Complete governance audit using template
2. **Gap Analysis:** Identify missing controls vs. regulatory requirements
3. **Remediation:** Use Playbook to implement missing controls
4. **Documentation:** Build evidence package from Playbook procedures
5. **Audit:** Present maturity scorecard + implemented controls

---

## 📁 What's Included

### **Assessment Tool**
- **Interactive Excel Template** — 6 sectors, 110+ controls, scored maturity model
- Shared link (no download needed)
- Works in Excel, Google Sheets, or browser

### **Documentation** (Download PDF or Read Online)
1. **IMPLEMENTATION_GUIDE.md** — Step-by-step assessment walkthrough
2. **SECTOR_MAPPING.md** — Banking & Insurance regulatory alignment
3. **EXTENDED_SECTOR_MAPPING.md** — Manufacturing, Automobile, Telecom, Utility alignment
4. **DEPLOYMENT_CHECKLIST.md** — Pre/post-implementation verification
5. **AI_PLAYBOOK.md** — Operational governance procedures (included)

### **For GitHub Users**
Repository: [AI Governance Audit Framework](https://github.com/sumeetsaraf/ai-governance-audit-framework)
- Open source (MIT License)
- Contribute improvements & sector-specific templates
- Fork for your organization

---

## 💡 Use Cases

### **Scenario 1: Shadow AI Risk**
**Problem:** Marketing deployed a chatbot without governance approval; it's processing customer emails.

**Solution:**
1. Use Playbook Section 2 to register the chatbot in AI System Registry
2. Classify as Tier 2 (High Risk) due to customer PII handling
3. Implement Playbook Section 4 LLM Gateway with PII masking
4. Document control in assessment framework
5. Re-assess governance score

---

### **Scenario 2: Regulatory Audit Preparation**
**Problem:** APRA is examining AI governance; you need to prove compliance with CPS 234.

**Solution:**
1. Run assessment using Banking template (2-4 hours)
2. Score your maturity across all controls
3. Use SECTOR_MAPPING.md to map scores to APRA requirements
4. Use Playbook sections to document implemented controls
5. Present maturity scorecard + evidence to auditors

---

### **Scenario 3: LLM Gateway Implementation**
**Problem:** Engineering team needs specifications for building an AI governance gateway.

**Solution:**
1. Provide Playbook Section 4 (LLM Gateway Specifications)
2. Engineering team builds three-layer architecture:
   - Layer 1: PII masking (regex/pattern scanning)
   - Layer 2: Prohibited topic blocking
   - Layer 3: Secured API calls with audit logging
3. Security team validates controls
4. Update assessment to reflect "Managed" control status

---

## 🎯 Key Takeaways

### **Assessment Framework**
- ✅ **Measure:** Scored maturity model (1-5 scale)
- ✅ **Sector-Specific:** Banking, Insurance, Manufacturing, Automobile, Telecom, Utility
- ✅ **Regulatory-Mapped:** APRA, Solvency II, ISO 9001, SOTIF, GDPR, NERC
- ✅ **Board-Ready:** Auto-calculated governance score for executive reporting

### **Operational Playbook**
- ✅ **Actionable:** Specific procedures, not abstract concepts
- ✅ **Defense-in-Depth:** Multi-tier risk classification + LLM gateways
- ✅ **Audit-Ready:** Enables compliance with international standards
- ✅ **Production-Grade:** Designed for enterprises deploying AI at scale

### **Together**
- ✅ **Eliminate Shadow AI:** Registry + Risk Tiers
- ✅ **Secure Data Boundaries:** LLM Gateways + Guardrails
- ✅ **Maintain Visibility:** Audit trails + Compliance logging
- ✅ **Pass Audits:** Assessment proves regulatory alignment

---

## 👥 Who This Is For

| Role | Primary Use | Time Commitment |
|---|---|---|
| **CIO / Chief AI Officer** | Governance strategy + board reporting | 4-6 hours |
| **Security / Compliance Lead** | Risk classification + control implementation | 8-12 hours |
| **AI Program Manager** | Framework deployment + stakeholder communication | 6-8 hours |
| **Engineering Lead** | LLM gateway design + architecture | 4-6 hours |
| **Audit / Risk Manager** | Maturity assessment + regulatory alignment | 3-5 hours |
| **Board Member** | Understanding AI governance maturity | 1 hour (scorecard) |

---

## 📈 Expected Outcomes

### **After 30 Days**
- ✅ AI System Registry created
- ✅ All AI systems classified (Tier 1-4)
- ✅ Governance assessment completed
- ✅ Executive summary for board

### **After 90 Days**
- ✅ LLM Gateway implemented
- ✅ Audit trails operational
- ✅ Governance maturity improved 1–2 points
- ✅ Audit-ready documentation

### **After 6 Months**
- ✅ Governance embedded in all AI projects
- ✅ Continuous monitoring automated
- ✅ Board-level governance dashboard
- ✅ Regulatory examination-ready

---

## 🤝 Contributing

Found an issue? Want to add a sector or control? 

**GitHub:** [Contribute to the framework](https://github.com/sumeetsaraf/ai-governance-audit-framework)

**Feedback:** [saraf.sumeet@gmail.com](mailto:saraf.sumeet@gmail.com)

---

## 📞 Support & Questions

### **Assessment Questions**
- Read: **IMPLEMENTATION_GUIDE.md** (includes scoring examples)
- Contact: [saraf.sumeet@gmail.com](mailto:saraf.sumeet@gmail.com)

### **Playbook Implementation**
- Reference: **AI_PLAYBOOK.md** (full operational procedures)
- Contact: [saraf.sumeet@gmail.com](mailto:saraf.sumeet@gmail.com)

### **Regulatory Alignment**
- Banking/Insurance: **SECTOR_MAPPING.md**
- Manufacturing/Auto/Telecom/Utility: **EXTENDED_SECTOR_MAPPING.md**

---

## 📜 License & Copyright

**Assessment Framework:** MIT License (Open Source)
**AI Playbook:** © 2026 Sumeet Saraf. All Rights Reserved.

---

## 🚀 Get Started Now

### **Step 1: Take the Assessment**
**→ [Open Excel Template](https://1drv.ms/x/c/8029e0f5e20b224c/IQAtzlhX8EX0To2nuEGL0SpVAc_9EyAq4gHp34siKYRvYSQ?e=Vvat1H)** (5 minutes to open, 2-4 hours to complete)

### **Step 2: Read the Playbook**
**→ Review AI_PLAYBOOK.md** (30 minutes for overview)

### **Step 3: Implement**
**→ Use Playbook sections to deploy controls** (timeline depends on complexity)

### **Step 4: Report**
**→ Generate governance scorecard for executive team** (1 hour)

---

## 👤 About the Author

**Sumeet Saraf** | AI Governance & Responsible AI Leader  
📧 [saraf.sumeet@gmail.com](mailto:saraf.sumeet@gmail.com)  
📱 +61 470 701 263  
🔗 [linkedin.com/in/sumeetsaraf](https://linkedin.com/in/sumeetsaraf)

**Expertise:** AI/ML lifecycle governance, Responsible AI assessments, data lineage & metadata, model risk, regulatory alignment (APRA CPS 234, ISO 27001, NIST AI RMF, GDPR).

**Background:** 24+ years in banking, insurance, government, and SaaS. Led multi-stream AI governance programs at Accenture, ANZ, Police Bank, and Resolution Life.

---

## 📊 Framework at a Glance

```
Assessment Framework              Enterprise AI Playbook
├─ 6 Sectors                      ├─ AI System Registry
├─ 110+ Controls                  ├─ Multi-Tier Risk Model
├─ Scored Maturity (1-5)          ├─ LLM Gateway Specs
├─ 6 Governance Areas             ├─ Security Procedures
├─ Regulatory Mapped              ├─ Audit Trails
└─ Board-Ready Reporting          └─ Incident Response
```

**Together:** A complete AI governance solution for enterprises.

---

**Last Updated:** June 2026  
**Framework Version:** 2.0 Extended (6 Sectors, 110+ Controls)  
**Playbook Version:** 1.0 (Operational Framework)
