# Incident Decision Log (Real-Time SEV-1 Simulation)

## T+0 — Signal detected
Ambiguous anomaly in monetization metrics.

Decision:
→ Wait for validation before escalation

Reason:
→ Avoid false SEV-1 noise

---

## T+8 — Signal strengthens
Multiple regions affected.

Decision:
→ Escalate immediately to SEV-1

Trade-off:
→ Speed over certainty

---

## T+20 — Conflicting hypotheses
Two possible root causes identified:
- pipeline failure
- reporting layer desync

Decision:
→ Investigate pipeline first

Reason:
→ Highest blast radius risk

---

## T+35 — Partial rollback suggested

Decision:
→ Approve rollback

Trade-off:
→ Lose recent changes vs restore revenue visibility

---

## T+60 — Stabilization confirmed

Decision:
→ Maintain monitoring before closure

Reason:
→ Avoid premature resolution declaration
