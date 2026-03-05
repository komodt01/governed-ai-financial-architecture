# Practical Control Alignment

This page maps control intent to architectural components in the reference payment platform.

The goal is to make compliance actionable — not abstract.

---

## Control-to-Architecture Mapping

| Architecture Domain | Control Intent | Example Evidence |
|--------------------|---------------|-----------------|
| **External Interface (Edge/API)** | Authentication, authorization, idempotency, rate limiting | API logs, auth provider logs, WAF rules |
| **Transaction Execution Engine** | Deterministic processing, replay protection | Workflow traces, test artifacts |
| **Ledger / System of Record** | Financial integrity, non-repudiation | Immutable logs, reconciliation reports |
| **Risk & Exception Operations** | Human approval, segregation of duties | Case records, approval history |
| **Data & Evidence Plane** | Monitoring, retention, alerting | SIEM logs, retention policies |
| **AI Advisory Plane** | Advisory outputs, decision traceability, drift monitoring | Model version records, drift metrics, review logs |
| **Governance Layer (Cross-Cutting)** | Oversight, change control, accountability | Governance meeting notes, change approvals |

---

## AI-Specific Alignment

AI integration introduces additional alignment considerations:

- AI must not bypass deterministic transaction controls  
- High-impact financial actions require documented human authorization  
- AI recommendations must be explainable where required  
- Model drift must be monitored and reviewed  
- Model updates must follow change governance procedures  

AI governance overlays existing control structures rather than replacing them.

---

## Architectural Principle

Compliance controls should be:

- Designed into workflows (not bolted on later)  
- Observable through evidence artifacts  
- Owned by defined roles  
- Testable during audits  

When controls are embedded at the architectural level, audit readiness becomes a byproduct of system design rather than a last-minute activity.