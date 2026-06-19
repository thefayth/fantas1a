# Fantasia Launch README

**Local-first AI operations desktop for safe creative automation.**

Fantasia is a desktop control room for builders who want AI tools to operate with receipts, rollback, and clear authority boundaries. It coordinates local services, operator queues, Codex/OpenClaw handoffs, FVE visual-engine workflows, and COAI / WordPress publish-readiness checks without turning every action into an unsafe live write.

## Investor Share Pack

Google Drive folder:

- [Fantasia Investor Pack - 2026-06-19](https://drive.google.com/drive/folders/1U1Y4DqxW28w3nV1hJwACnqExh8ALKL_Z)

Key investor files:

- [Updated investor pack zip](https://drive.google.com/file/d/1-JutItFU37CcTG6TlfekBij_3zjaD20y/view?usp=drivesdk)
- [Pitch deck HTML](https://drive.google.com/file/d/1Dd4AbA1hH9l0gUlP8pts_0umWx3JdZi3/view?usp=drivesdk)
- [Brand board HTML](https://drive.google.com/file/d/1FTcDc_bMEkuA8MdaF9lBWZRDoejlo4MB/view?usp=drivesdk)
- [FaithCheltenham WordPress demo HTML](https://drive.google.com/file/d/1HuvAF0A0bjvXE4_B8hIciLwopLoe7x1j/view?usp=drivesdk)

Note: Drive upload succeeded. General sharing may still need to be turned on in Google Drive UI if investors are outside the account's permitted domain.

## What It Does

- Starts scoped local work sessions.
- Shows local service and queue state.
- Routes handoffs between Faith, Codex, OpenClaw, and local operator lanes.
- Provides an FVE Workbench for image-review and website-change prep.
- Checks COAI / WordPress readiness while redacting credentials.
- Records checkpoints, task packets, verification runs, patch receipts, and rollback paths.

## Why It Exists

AI work is becoming too important to live only in chat windows. Builders need a place where AI can help operate real workflows while preserving privacy, authorship, and production safety.

Fantasia is built around a simple rule:

> AI can move faster when the system has memory, receipts, and brakes.

## First Use Case: FVE Website Visual Operations

Fantasia's first focused workflow is helping operate the FAYTH Visual Engine:

- review live website images
- keep passing images in place
- find weak, repeated, broken, generic, or line-drawn assets
- prepare replacements
- map candidates to target slots
- check COAI / WordPress publish readiness
- keep production publish guarded until rollback, target slots, typed slug, and production status are clean

Fantasia does not bypass FVE. FVE remains the source of truth for visual decisions and guarded publishing.

## Safety Model

Fantasia is local-first by default:

- no direct WordPress publish from Fantasia
- no credential values in UI logs
- no DNS/auth/plugin changes by default
- no social posting without approval
- no public dashboard exposure by default
- no hidden cloud telemetry
- no production writes without a specific guarded adapter

## Current Status

Fantasia is in local preview. The current docs and deck describe the working product direction and investor story. Public release should happen after a final secret scan, private-path scan, and release review.

Current FVE quickstart truth:

- `6` local publish candidates
- `105` request-changes rows
- `1` production status check
- `0` typed publish-ready rows

## Docs

- [How to Use Fantasia](docs/HOW_TO_USE_FANTASIA.md)
- [Investor Pitch Deck](docs/INVESTOR_PITCH_DECK.md)
- [Fantasia Brand Kit](docs/FANTASIA_BRAND_KIT.md)
- [Canva Design Brief](docs/CANVA_DESIGN_BRIEF.md)
- [Drive Links](docs/DRIVE_LINKS.md)
- [GitHub Launch Plan](docs/GITHUB_LAUNCH_PLAN.md)
- [GitHub / Drive Links Manifest](docs/github-links-manifest.json)
- [FaithCheltenham WordPress Demo](website-demo/faithcheltenham-fantasia/index.html)

## Investor Story

Fantasia is not another AI chat app. It is an operations layer for owner-controlled AI work: a desktop cockpit that helps practical automation become inspectable, reversible, and commercially usable.
