# Incident Timeline with Decision Points (SEV-1 Monetization Incident)

## T+0 — Detection

* Monitoring detects revenue inconsistency across dashboards
* Initial assumption: reporting delay vs pipeline failure
* Decision: **Do not escalate yet — validate signal first**

---

## T+10 — Signal confirmed

* Multiple regions show inconsistent monetization data
* Creator complaints begin increasing
* Decision: **Escalate to SEV-1 immediately**

Reasoning: potential revenue impact outweighs false-positive risk

---

## T+15 — Incident declared

* Incident bridge created
* Roles assigned
* Engineering + Ops + Comms activated

Decision: **Centralize communication in one channel to avoid fragmentation**

---

## T+25 — First divergence in hypotheses

Two competing theories:

* A: ingestion pipeline failure
* B: reporting layer desync

Decision:
→ Prioritize ingestion layer investigation first (highest blast radius)

---

## T+40 — Partial mitigation option appears

Engineering suggests partial rollback

Decision:

* Choose rollback over patch
* Reason: faster restoration > perfect root cause understanding

Trade-off accepted:
→ Temporary loss of recent changes vs restoring revenue visibility

---

## T+60 — Recovery initiated

* Rollback executed
* Metrics begin stabilizing
* Monitoring confirms partial recovery

Decision:
→ Continue monitoring before closing incident

---

## T+90 — Full resolution

* System stabilizes globally
* Revenue reporting restored

Decision:
→ Keep incident open for postmortem analysis before closure

---

## Key Decision Learnings

* Early escalation reduces downstream impact
* Partial rollback is often better than delayed perfect fix
* Coordination speed matters more than technical certainty
* Clear ownership reduces decision paralysis
