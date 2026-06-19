
# Architecture Overview

F@ntas1@ is designed as a conductor rather than an uncontrolled autonomous agent. The public architecture is intentionally high level.

## Operating Layers

1. Intake layer: desktop task entry, OpenClaw phone lane, local queues, and project signals.
2. Conductor layer: F@ntas1@ classifies work, checks boundaries, builds recommendations, and selects a lane.
3. Authority layer: scoped session leases, pause/revoke controls, and high-impact blocks.
4. Worker layer: AI Desk packets, local workers, GitTools, browser checks, Tool Doctor, and approved free tools.
5. Receipt layer: review packets, audit summaries, rollback notes, release readiness, and public-safe status.
6. Public surface: GitHub docs, visual assets, diagrams, WordPress draft, and ownership policy.

## Local-First Rules

- Loopback/private access before public exposure.
- Registry-approved tools before arbitrary commands.
- Scoped authority before local mutation.
- Review packets before implementation claims.
- Git state and rollback posture before development work.
- Explicit Faith approval before high-impact actions.

## Codex-Optional Shape

F@ntas1@ can operate in a Codex-assisted mode or a standalone operator mode. Public docs may describe both, but the private implementation, local queues, receipts, and worker code stay excluded.

## Phone Support Shape

OpenClaw is the preferred private phone lane. Phone work is not treated as separate from implementation work: meaningful phone/OpenClaw results return as Operator Inbox, AI Desk, or Codex-visible packets so implementation and review remain visible.

## Dev Mode Shape

Dev Mode is for registered projects. GitTools are the control surface: status, branch, diff, verification, commit preview, local commit, and rollback readiness. Push, PR, publish, deploy, DNS, credentials, payments, and public posting remain separately gated.
