# How to Use Fantasia

Fantasia is the desktop control room for Faith's local AI work. It does not replace Codex, FVE, OpenClaw, or GitHub. It makes them easier to operate from one place while keeping risky actions gated, reversible, and receipted.

## What Fantasia Does

Fantasia helps you:

- Start a scoped local work session.
- See local services, queues, handoffs, and readiness states.
- Route work between Faith, Codex, OpenClaw, and local operator lanes.
- Use the FVE Workbench for image-review and website-change prep.
- Check COAI / WordPress publish readiness without printing credentials.
- Keep a receipt trail for checkpoints, patches, verification, rollback, and launch decisions.

Fantasia is intentionally local-first. It should not expose private queues, credentials, screenshots, or drafts to a public repo or a live website.

## Fastest Click Path

Use this when the goal is to prepare FVE website image work:

1. Open `Fantasia.exe`.
2. Click `Start Session`.
3. Open `FVE Workbench`.
4. Click `Run FVE Ready Path`.
5. Click `Check COAI Readiness`.
6. Open the FVE app only when you want the final guarded publish screen.
7. Publish only after FVE shows rollback, exact slug, target slots, production status, and `FVE_PRODUCTION_WRITE=true` are clean.

## Main Screens

### Home

Home shows the overall operating state: active local mode, active leases, queue counts, local services, quick links, recent handoffs, and next recommended actions.

### FVE Workbench

FVE Workbench is for local development and image-operation prep. It can refresh FVE status, create a checkpoint, create a task packet, apply an allowlisted local patch, run verification, show COAI / WordPress readiness, and open the FVE desktop app.

It should not directly write WordPress. Production publishing stays inside FVE's COAI guard.

### COAI / WordPress Publish Gate

This panel is read-only. It checks whether FVE has enough local proof to attempt a guarded publish later.

It shows whether a WordPress base URL is present, whether COAI or WordPress app-password auth is present, whether publish candidates exist, whether production status has been checked, whether the production write flag is intentionally on, and what blockers remain.

It redacts credential values. Seeing `present` does not mean the app will print or save the secret.

## Current FVE Status

The latest local quickstart receipt says:

- status: `needs-coai-guard-check`
- local publish candidates: `6`
- request-changes rows: `105`
- typed publish ready count: `0`
- production status checked count: `1`

Meaning: there are candidates worth reviewing, but Fantasia/FVE should not publish yet. The weak rows still need cleanup, and the typed publish guard is not clean.

## Production Safety Rules

Fantasia should stop before DNS changes, authentication changes, plugin activation or deactivation, social posting, public dashboard exposure, unaudited recursive writes, live WordPress writes outside FVE COAI, CAPTCHA/MFA bypass attempts, missing rollback, missing target keys, or credential leakage.

## Troubleshooting

### FVE Workbench says OpenClaw is blocked

Start or repair the OpenClaw loopback gateway, then refresh Fantasia. The FVE patch lane intentionally requires OpenClaw health before applying local patches.

### COAI readiness says credentials are missing

Set credentials in the local launch environment, not in chat and not in source files.

### Publish is blocked even with credentials

That is expected until FVE has clean production status, rollback snapshot, confirmed COAI target slots, typed slug confirmation, approved publish candidates, and `FVE_PRODUCTION_WRITE=true`.

### Local package is signed but Windows says untrusted

The current package uses a local self-signed development certificate. That proves local signing automation works. A public installer later needs a real code-signing certificate from a trusted certificate authority.
