# Compliance Scope & Baseline

Financial payment platforms operate in regulated environments where correctness, auditability, and accountability are mandatory.

This baseline defines the minimum control expectations assumed throughout this reference architecture. It is framework-informed (NIST / ISO), but written in operational language to guide architecture decisions.

---

## Baseline Assumptions

The following are treated as non-negotiable requirements:

- Payment execution must be deterministic
- Financial records must be tamper-evident
- Sensitive data must be protected in transit and at rest
- All critical actions must be traceable and attributable
- Privileged access must be restricted and monitored
- Production changes must be reviewed and documented
- AI-assisted decisions must be reviewable and overrideable

---

## Core Control Outcomes

Rather than listing control IDs, this baseline defines expected outcomes:

### Identity & Access
- Strong authentication for system and human actors  
- Least-privilege authorization  
- Segregation of duties for approval workflows  

### Data Protection
- Encryption in transit and at rest  
- Key management with defined ownership  
- Controlled data retention and deletion  

### Integrity & Auditability
- Immutable or tamper-evident financial records  
- Time-synchronized logging  
- End-to-end transaction traceability  

### Monitoring & Detection
- Centralized logging and alerting  
- Anomaly detection (behavioral and operational)  
- Alert escalation procedures  

### Change & Release Governance
- Documented approval processes  
- Version traceability  
- Rollback capability  

### AI Governance (Baseline Expectation)
- AI outputs are advisory-by-default  
- High-impact decisions require human authorization  
- Model scope and usage are documented  
- Model updates are reviewed and approved  

---

## Framework Alignment (High-Level)

This baseline aligns conceptually with:

- **NIST 800-53**: Access Control, Audit & Accountability, Configuration Management, System Integrity  
- **ISO 27001 Annex A**: Access, Cryptography, Operations Security, Incident Management  
- **NIST AI Risk Management Framework**: Govern, Map, Measure, Manage  

This document does not replace formal compliance assessments but establishes the architectural expectations assumed across this site.