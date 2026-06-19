# Fantasia Public / Private Boundary

## Purpose

This boundary keeps Fantasia shareable while protecting Faith's ownership, leverage, security posture, and commercial options.

Commercial entity: `XXYYZZ Society LLC`

Creator/founder: `Faith Cheltenham`

## Public Surface

The public GitHub repo can be used as a product home page and due-diligence surface. It may include:

- Product README.
- How-to guide.
- Investor pitch deck.
- Drive links to investor materials.
- Brand kit overview.
- Public demo page copy.
- Commercial license notice.
- Security and responsible disclosure notes.
- Sanitized screenshots or videos.

## Private Core

The following should stay private unless Faith explicitly approves a reviewed release:

- Fantasia desktop app source and installer build system.
- FVE implementation code, production publish orchestration, and COAI/WordPress adapters.
- Any credentials, app passwords, API keys, worker tokens, signed URLs, or private server paths.
- Code-signing keys, certificate passwords, and release identities.
- Local queue state, worker packets, private receipts, rollback snapshots, and logs with local paths.
- Customer/project data, private screenshots, private assets, adult/held surfaces, and unpublished brand materials.

## Safe GitHub Pattern

Use `thefayth/fantasia` as a docs-first public product repo:

1. Keep the top-level README clear and commercial.
2. Add `LICENSE.md` with proprietary terms.
3. Add docs that explain what Fantasia does without revealing private implementation.
4. Link to investor materials only after confirming sharing settings.
5. Keep private code in a separate private repo or local source root.

## Release Gate

Before any source, binary, installer, screenshot pack, or generated asset is published:

- Run a secret scan.
- Run a private-path scan.
- Confirm no credentials or tokens are present.
- Confirm no signed/private URLs are present.
- Confirm no private local receipts are included.
- Confirm image rights and third-party licenses.
- Confirm Faith approval for the exact package.

## Current Boundary Status

Status: `docs-first-public-repo`

Known public repo: `thefayth/fantasia`

Drive sharing status: uploaded, but broad external sharing still needs confirmation in Google Drive UI or direct investor email sharing.
