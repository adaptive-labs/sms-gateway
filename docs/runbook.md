---
category: runbook
title: SMS Gateway runbook
description: On-call runbook for SMS Gateway.
related_entities:
  - sms-gateway
related_teams:
  - notifications
---

# SMS Gateway runbook

On-call guide for `sms-gateway` (Notifications, tier medium).

## Alerts

- **sms-gateway-high-error-rate** — 5xx over 2% for 5m. Check upstream dependencies.
- **sms-gateway-latency** — p99 over SLO. Check resource saturation.

## Common issues

- **Pod OOMKilled** — check memory limits and recent traffic spikes.
- **Crashloop** — check the last deploy and roll back if needed.

## Escalation

Page the Notifications on-call rotation.

