# GitHub Launch Plan for Fantasia

## Current Launch Truth

Fantasia now has a docs-first public repository:

```text
thefayth/fantasia
```

The public repo should stay documentation-first until Faith approves a separate source release. Fantasia core, FVE production adapters, COAI publishing logic, credentials, signing material, private receipts, and customer/project data remain private.

Commercial entity:

```text
XXYYZZ Society LLC
```

Creator/founder:

```text
Faith Cheltenham
```

## Recommended Repo

Recommended docs-first public repo:

```text
thefayth/fantasia
```

Recommended product name:

```text
Fantasia - Local AI Operations Desktop
```

## Launch Positioning

Short description:

```text
Local-first AI operations desktop for safe creative automation, FVE website visual work, operator queues, and receipt-backed publishing readiness.
```

Long description:

```text
Fantasia is a local desktop conductor for practical AI operations. It coordinates local services, Codex/OpenClaw handoffs, FVE visual-engine workflows, COAI/WordPress publish readiness, scoped authority sessions, receipts, verification, and rollback. It is built for builders who need automation with proof, privacy, and control.
```

## Files to Include in First Repo Launch

Include:

- `README.md`
- `README_LAUNCH.md`
- install/run docs
- investor docs
- screenshots that contain no private data
- release manifest with private paths removed
- proprietary commercial license notice
- public/private boundary doc
- commercial use policy
- `.gitignore`
- security policy
- contribution policy if public

Exclude:

- app source until separately approved
- FVE production adapters
- COAI/WordPress publishing internals
- private queue files
- local receipts with sensitive paths if public
- environment files
- credentials
- screenshots containing private windows
- WordPress auth material
- server credentials
- paid API keys
- private project ledgers

## Pre-Launch Checklist

1. Run a secret scan.
2. Run a private-path scan.
3. Remove generated private state.
4. Confirm release package excludes `tools/fantasia/private`.
5. Confirm no `.env` or secret-like file is included.
6. Confirm screenshots are safe.
7. Confirm README does not claim production publishing has happened.
8. Confirm the repo target is `thefayth/fantasia`.
9. Publish docs only.
10. Review GitHub rendering.
11. Add topics.
12. Add release notes only after a clean package is attached.

## GitHub CLI Commands

Run these from the actual Fantasia source root only if Faith approves a private source mirror later:

```powershell
gh auth status
gh repo create thefayth/fantasia-core --private --description "Private Fantasia source root." --source . --remote origin --push
```

If a private source repo already exists:

```powershell
git remote add origin https://github.com/thefayth/fantasia-core.git
git branch -M main
git push -u origin main
```

## Suggested Topics

```text
local-first
ai-operations
desktop-app
electron
creative-automation
wordpress
visual-engine
receipts
rollback
operator-tools
```

## First Release Notes Draft

```markdown
# Fantasia v0.1 Local Preview

Fantasia is a local-first AI operations desktop for safe creative automation, FVE website visual work, operator queues, and receipt-backed publishing readiness.

This preview includes:

- scoped session control
- local service cockpit
- FVE Workbench
- COAI / WordPress readiness checks
- quickstart click path
- local package manifest
- development code-signing automation

Not included:

- live WordPress publishing from Fantasia
- public installer trust certificate
- hosted cloud dashboard
- telemetry
```

## Launch Status

Status: `docs-first-public-repo`

Next required action: keep the public repo polished as a commercial product surface, then prepare a private core repo only after secret/private-path scans and Faith approval.

Prepared local launch artifact:

```text
docs/fantasia/README_PUBLIC_DRAFT.md
```
