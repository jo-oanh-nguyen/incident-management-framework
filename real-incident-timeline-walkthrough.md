# Real Incident Walkthrough (SEV-1 Monetization Disruption)

## T+0 — Detection
- Alert triggered: revenue reporting anomaly detected
- Initial hypothesis: data pipeline delay vs system failure

## T+5 — Incident declared
- SEV-1 triggered
- Incident bridge opened
- Roles assigned

## T+15 — First triage decision
- Decision: isolate reporting layer vs ingestion layer
- Trade-off: speed vs accuracy

## T+30 — Root cause narrowing
- Engineering identifies likely pipeline failure after deploy
- Rollback considered

## T+45 — Mitigation
- Rollback executed
- Monitoring confirms partial recovery

## T+90 — Full resolution
- Data consistency restored
- Stakeholder update sent

## Postmortem trigger
- Why detection lagged 12 minutes
- Why escalation was delayed between regions
