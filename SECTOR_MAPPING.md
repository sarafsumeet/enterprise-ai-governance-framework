# Regulatory Mapping: AI Governance Audit Framework

This document shows **how each control in the framework maps to specific regulatory requirements**.

---

## Overview

The framework is aligned with:
- **APRA CPS 234** (Australia) — Prudential supervision of AI/ML models in banking
- **Solvency II** (EU/UK) — Insurance governance and model validation
- **SOX 404** (USA) — Internal control over financial reporting
- **ISO 27001 & ISO/IEC 42001** — Information security and AI management

---

## APRA CPS 234: Prudential Supervision of AI/ML Models (Australia)

### Regulation Summary
APRA CPS 234 requires ADIs (Authorised Deposit-taking Institutions) to:
1. Identify material AI/ML models
2. Establish governance framework
3. Conduct independent validation
4. Assess and manage model risk
5. Document and report

### Control Mapping

#### **Data Governance ↔ CPS 234 Pillar 1: Model Input Data**

| CPS 234 Requirement | Our Framework Control | Evidence of Compliance |
|---|---|---|
| Data used must be fit for purpose | Data Quality & Validation | Quality SLAs; automated checks; alert thresholds |
| Data must be understood and documented | Data Lineage & Traceability | End-to-end lineage tracking; data dictionary |
| Data must be appropriate for use in models | Metadata Management | Data catalog; ownership; sensitivity classification |
| Data must remain fit for purpose over time | Retention & Archival Policy | Archival procedures; audit trail of data changes |

**Compliance Evidence to Gather:**
- Data quality dashboard with SLAs
- Data lineage diagram (dbt/Collibra)
- Data catalog with ownership
- Retention policy documentation

---

#### **Model Lifecycle ↔ CPS 234 Pillar 2: Model Development & Deployment**

| CPS 234 Requirement | Our Framework Control | Evidence of Compliance |
|---|---|---|
| Models must be developed using sound methodology | Model Development & Testing | Code review process; test coverage; documented methodology |
| Models must be independently validated | Model Validation (Independent) | Validation charter; third-party review; sign-off |
| Models must be deployed safely | Model Deployment & Version Control | Change management; deployment checklist; rollback procedures |
| Models must be monitored continuously | Model Monitoring & Drift Detection | Performance dashboards; alert thresholds; incident response |

**Compliance Evidence to Gather:**
- Model development process documentation
- Independent validation reports
- Change control register
- Model monitoring dashboards

---

#### **Risk & Compliance ↔ CPS 234 Pillar 3: Model Risk Management**

| CPS 234 Requirement | Our Framework Control | Evidence of Compliance |
|---|---|---|
| Model risk must be assessed (BCBS 239 equivalent) | Model Risk Assessment | Risk taxonomy; risk rating matrix; residual risk documentation |
| Models must be explainable | Explainability & Interpretability | SHAP/LIME reports; domain expert review; decision rationale documentation |
| Fair outcomes must be documented | Fairness & Bias Detection | Fairness testing report; protected attribute analysis; disparate impact assessment |
| Regulatory compliance must be demonstrated | Regulatory Compliance Mapping | CPS 234 compliance checklist; audit log; board reporting |

**Compliance Evidence to Gather:**
- Model risk register
- Explainability documentation
- Fairness testing reports
- Regulatory compliance sign-off

---

#### **Governance & Culture ↔ CPS 234 Pillar 4: Governance & Oversight**

| CPS 234 Requirement | Our Framework Control | Evidence of Compliance |
|---|---|---|
| Board must oversee AI governance | AI Ethics & Responsible AI Framework | Board AI governance charter; ethics framework documentation |
| Audit trails must be maintained | Change Management & Audit Trails | Versioning system; audit log; change history |
| Staff must be trained | Stakeholder Training & Communication | Training program; certification records; communication log |
| Third parties must be managed | Third-Party Model Governance | Vendor audit procedures; SLA documentation; ongoing monitoring |

**Compliance Evidence to Gather:**
- Board governance charter
- Audit logs (Git, model registry)
- Training attendance records
- Vendor compliance assessments

---

## Solvency II: Insurance Model Governance (EU/UK)

### Regulation Summary
Solvency II (Article 8.2) requires insurance undertakings to:
1. Identify material models
2. Conduct independent validation
3. Document model assumptions
4. Monitor model performance

---

### Control Mapping

#### **Data Governance ↔ Solvency II Article 8.2.1: Data Quality**

| Solvency II Requirement | Our Framework Control | Evidence of Compliance |
|---|---|---|
| Data must be accurate and complete | Data Quality & Validation | Data quality metrics; completeness checks; accuracy targets |
| Data lineage must be traceable | Data Lineage & Traceability | Source system documentation; transformation tracking |
| Metadata must be documented | Metadata Management | Data dictionary; sensitivity labels; quality tags |
| Data must be retained appropriately | Retention & Archival Policy | Retention schedules; archival procedures |

**Solvency II Context:**
- **Underwriting models:** Data on policyholders, claims history, risk factors
- **Reserving models:** Claims data, economic factors, lapse rates
- **Capital models:** Market data, credit exposure, operational risk factors

---

#### **Model Lifecycle ↔ Solvency II Article 8.2.2: Model Validation**

| Solvency II Requirement | Our Framework Control | Evidence of Compliance |
|---|---|---|
| Models must be validated independently | Model Validation (Independent) | Validation report; independence certificate; sign-off |
| Back-testing must occur regularly | Model Monitoring & Drift Detection | Back-test results; calibration reviews; recalibration triggers |
| Models must be appropriate for use | Model Development & Testing | Model scope document; assumption documentation; limitations documented |
| Model changes must be documented | Model Deployment & Version Control | Change log; version history; change impact assessment |

**Solvency II Context:**
- **Annual validation:** Formal revalidation of models
- **Quarterly back-testing:** Performance vs. actual outcomes
- **Trigger-based revalidation:** When assumptions no longer hold

---

#### **Risk & Compliance ↔ Solvency II Article 18: Risk Management**

| Solvency II Requirement | Our Framework Control | Evidence of Compliance |
|---|---|---|
| Underwriting risk must be assessed | Model Risk Assessment | Risk-of-ruin analysis; sensitivity testing; worst-case scenarios |
| Concentration risk must be tracked | Fairness & Bias Detection | Concentration limits; exposure by segment; stress testing |
| Models must be compliant with regulations | Regulatory Compliance Mapping | Compliance matrix; audit trail; insurance supervisor reporting |
| Explainability to supervisors | Explainability & Interpretability | Model documentation; key drivers report; assumptions transparency |

---

## SOX 404: Internal Control Over Financial Reporting (USA / Public Companies)

### Regulation Summary
SOX 404 requires:
1. Management to assess effectiveness of internal controls
2. Auditors to attest to those controls
3. Documentation and testing of IT controls

---

### Control Mapping

#### **Data Governance ↔ SOX 404 Section 302/906: Data Integrity**

| SOX 404 Requirement | Our Framework Control | Evidence of Compliance |
|---|---|---|
| Data accuracy controls must exist | Data Quality & Validation | Quality gates; validation rules; exception handling |
| Data must be recorded and retained | Data Lineage & Traceability | Audit trail; change log; data flow documentation |
| Metadata must be documented | Metadata Management | Data dictionary; ownership; sensitive data inventory |
| Data retention policy must be enforced | Retention & Archival Policy | Retention calendar; deletion procedures; compliance verification |

**SOX 404 Context:**
- Revenue recognition models (if AI is involved)
- Financial forecasting models
- Internal control testing models
- Fraud detection systems

---

#### **Model Lifecycle ↔ SOX 404 Section 302: IT Controls**

| SOX 404 Requirement | Our Framework Control | Evidence of Compliance |
|---|---|---|
| Code review and testing controls | Model Development & Testing | Peer review process; test cases; testing documentation |
| Change management controls | Model Deployment & Version Control | Change approval workflow; UAT; production handoff checklist |
| Access controls (who can deploy?) | Governance & Culture | Role-based access; segregation of duties; logging |
| Backup and recovery controls | Model Deployment & Version Control | Backup procedures; disaster recovery plan; RTO/RPO documentation |

---

## ISO 27001 & ISO/IEC 42001: Information Security & AI Management

### ISO 27001: Information Security Management (Global Standard)

#### Control Mapping

| ISO 27001 Control | Our Framework Control | Implementation |
|---|---|---|
| **A.6: Organizational Controls** | AI Ethics & Responsible AI Framework | AI governance structure; roles and responsibilities |
| **A.7: Human Resource Security** | Stakeholder Training & Communication | Security training; AI governance awareness |
| **A.9: Access Control** | Model Lifecycle (Deployment) | Access to model registry; code repositories; secrets management |
| **A.10: Cryptography** | Data Governance | Encryption at rest; in transit; key management |
| **A.12: Operations Security** | Model Monitoring & Drift Detection | Monitoring controls; incident response; change management |
| **A.13: Communications Security** | Data Lineage & Traceability | Secure data transmission; audit logs |
| **A.14: System Acquisition & Maintenance** | Model Lifecycle (Development) | Secure code practices; dependency management; vendor vetting |
| **A.18: Supplier Relationships** | Third-Party Model Governance | Vendor audits; SLAs; data processing agreements |

---

### ISO/IEC 42001: AI Management Systems (Draft/Recent Standard)

#### Control Mapping

| ISO 42001 Requirement | Our Framework Control | Implementation |
|---|---|---|
| **4.1: AI Risk Assessment** | Model Risk Assessment | Risk taxonomy; likelihood × impact; residual risk rating |
| **4.2: AI Governance** | Governance & Culture | Board oversight; governance charter; decision rights |
| **4.3: Data Governance** | Data Governance | Data quality; lineage; metadata; retention |
| **4.4: Model Development** | Model Lifecycle (Development) | Development process; code review; documentation |
| **4.5: Model Validation** | Model Lifecycle (Validation) | Independent validation; benchmarking; sign-off |
| **4.6: Monitoring & Control** | Model Monitoring & Drift Detection | Performance monitoring; alert thresholds; retraining triggers |
| **4.7: Transparency & Explainability** | Explainability & Interpretability | Model cards; SHAP/LIME reports; decision rationale |
| **4.8: Fairness & Bias** | Fairness & Bias Detection | Fairness testing; protected attribute analysis; monitoring |
| **4.9: Human Oversight** | Governance & Culture | Human-in-the-loop; override authority; accountability |
| **4.10: Third-Party AI** | Third-Party Model Governance | Vendor assessments; SLAs; ongoing audits |

---

## Regulatory Compliance Checklist by Framework

### Use This to Prepare for Audit

#### **For APRA CPS 234 (Banking)**

- [ ] Model inventory: All material models identified & documented
- [ ] Data governance: Quality SLAs; lineage tracking; metadata catalog
- [ ] Model validation: Independent validation charter & signed reports
- [ ] Risk assessment: Risk register with residual risk rating
- [ ] Explainability: SHAP/LIME reports; model documentation
- [ ] Fairness: Fairness testing report; protected attribute analysis
- [ ] Monitoring: Performance dashboards; alert thresholds; incident log
- [ ] Audit trail: Change log; version history; access logs
- [ ] Board reporting: AI governance summary for board review

#### **For Solvency II (Insurance)**

- [ ] Model scope: All underwriting & reserving models documented
- [ ] Validation: Independent validation report (annual minimum)
- [ ] Back-testing: Quarterly back-test results; recalibration log
- [ ] Data: Quality metrics; completeness assessment; assumptions documented
- [ ] Risk assessment: Underwriting risk; concentration risk; model risk
- [ ] Stress testing: Scenario analysis; worst-case outcomes
- [ ] Audit trail: Change log; model version history
- [ ] Regulatory reporting: Supervisor questionnaire responses

#### **For SOX 404 (Public Companies)**

- [ ] Model governance: IT controls documentation
- [ ] Code review: Peer review process; testing records
- [ ] Change management: Approval workflow; UAT records; sign-off
- [ ] Access control: Role-based access; segregation of duties
- [ ] Data integrity: Validation rules; quality controls; exception log
- [ ] Monitoring: System monitoring; audit logs
- [ ] Training: IT control training; certification records

---

## How to Use This Mapping

### **During Assessment:**
When scoring a control, reference this table to ensure you're capturing all regulatory requirements.

**Example:**
- Auditor asks: *"How do you comply with APRA CPS 234 around model risk?"*
- You reference: **Model Risk Assessment → BCBS 239 equivalent → Risk register + residual risk rating**
- You show: Risk register artifact + board-ready summary

### **Preparing for Audit:**
Use the checklists above to prepare your evidence:
- Compile artifacts (documentation, screenshots, reports)
- Identify gaps (controls not yet in place)
- Plan remediation (timeline + owner)

### **Stakeholder Communication:**
When speaking with:
- **Board:** *"We've assessed ourselves against APRA CPS 234 Pillar 1 (Data Governance). Score: 3.5/5."*
- **Auditors:** *"Our control evidence includes: [list artifacts from the checklist]"*
- **Regulators:** *"Here's how we map each CPS 234 requirement to our control framework."*

---

## Questions?

Refer to:
- **APRA CPS 234**: https://www.apra.gov.au/prudential-standards/prudential-standard-cps-234-models
- **Solvency II**: https://www.eiopa.europa.eu/tools-and-data/tools/solvency-ii-compass
- **SOX 404**: https://www.sec.gov/cgi-bin/viewer?action=view&cik=&accession_number=0001193125-07-015779&xbrl_type=v
- **ISO 27001**: https://www.iso.org/standard/54534.html
- **ISO/IEC 42001**: https://www.iso.org/standard/81230.html

---

**Framework Built By:** Sumeet Saraf | AI Governance Leader  
**Last Updated:** June 2026