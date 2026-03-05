## Principles (TOGAF-aligned, but not academic)

# Architecture Principles

These principles guide the reference architecture and keep AI integration aligned with regulated payment system requirements.

They are informed by enterprise architecture practices commonly associated with TOGAF (e.g., clear domain boundaries, governance, and traceability), but expressed in practical system-design terms.

---

## 1. Deterministic Financial Execution

Financial state changes must be deterministic, repeatable, and policy-bound.

AI may assist operations, but **must not be the default authority** for financial state transitions.

---

## 2. Ledger as the System of Record

The ledger is authoritative.

All material transaction outcomes must be traceable to the system of record and reconstructable for audit and reconciliation.

---

## 3. AI is Advisory by Default

AI produces recommendations and context, not final decisions.

High-impact actions require deterministic policy enforcement or explicit human authorization.

---

## 4. Explicit Decision Rights and Accountability

For every AI-assisted workflow, decision ownership must be clear:

- Who owns the policy?
- Who owns the model?
- Who approves changes?
- Who is accountable under audit?

No ambiguous “the system decided” outcomes.

---

## 5. Evidence is a First-Class Architectural Output

Audit evidence is not an afterthought.

Every critical action (including AI inference outputs) must generate traceable, time-synchronized evidence:

- correlation IDs
- actor identity
- model version (where applicable)
- decision outcome and rationale pathway

---

## 6. Separation of Duties is Preserved

Approval boundaries must remain intact.

AI cannot collapse segregation of duties by enabling one workflow to initiate and approve materially sensitive actions.

---

## 7. Governed Change and Controlled Evolution

Models, thresholds, routing logic, and operational policies evolve.

Changes must follow controlled release and governance practices:

- documented rationale
- validation/impact assessment
- controlled rollout
- rollback capability

---

## 8. Vendor Neutrality and Portability

The architecture is capability-driven and designed to support hybrid environments.

Avoid “hard coupling” that prevents cloud exit, portability, or regulatory-driven deployment changes.

---

## 9. Secure-by-Design Defaults

Security controls are embedded into the architecture:

- least privilege access
- encryption in transit/at rest
- monitoring and alerting
- incident response readiness

AI inherits these controls; it does not bypass them.

---

## 10. Operational Excellence and Cost Discipline

Reliability and cost are architecture concerns:

- observability is required for systems and models
- AI usage must be measurable and defensible
- design for resilience and predictable cost profiles