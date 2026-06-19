# Fantasia Commercial Use Policy

## Recommendation Locked In

Keep Fantasia core proprietary while the product, installer, FVE integration, COAI publishing, and customer workflows are still being shaped. Use the public GitHub repository as a polished product surface, not as a full source release.

Commercial entity: `XXYYZZ Society LLC`

Creator/founder: `Faith Cheltenham`

Brand/product layer: `Fantasia`, `TheFAYTH`, and FVE.

## Business Model Paths

- Desktop Pro License: paid local desktop app for builders and operators.
- Implementation Services: setup Fantasia, FVE, COAI, website image workflows, and local automation.
- Managed Creative Operations: recurring image review, replacement, publish-readiness, and rollback support.
- Enterprise / Agency Pilot: private deployment with onboarding, training, adapters, and support.
- Brand / Website Refresh Packages: fixed-scope visual cleanup for WordPress and owned sites.
- White-Label / Partner License: only after core IP, support scope, and attribution terms are clear.

## Public Repo Strategy

Public-safe now:

- README and product story.
- How-to documentation.
- Investor deck and share links.
- Brand kit overview.
- WordPress demo page copy.
- License notice, security policy, and public/private boundary.

Keep private:

- Fantasia core source.
- FVE production publishing logic that contains private adapters or operational details.
- COAI credentials, tokens, app passwords, signed URLs, and private endpoints.
- Code-signing keys, certificate passwords, installer secrets, and build identities.
- Private receipts, local queue state, customer data, screenshots with private windows, and unpublished assets.

## License Matrix

| Area | Recommended Status |
| --- | --- |
| Fantasia desktop core | Proprietary / commercial license required |
| FVE publish adapters | Proprietary / private |
| COAI production workflow | Proprietary / guarded |
| Public docs | All rights reserved unless a specific file says otherwise |
| Brand kit and marks | XXYYZZ Society LLC / TheFAYTH / Fantasia brand assets reserved |
| Low-risk SDK/helpers later | Consider Apache-2.0 after review |
| Third-party dependencies | Follow their own licenses |

## Customer Terms Checklist

Before selling a paid license or pilot, prepare:

- Order form or statement of work.
- Scope of use: seats, machines, sites, brands, and publishing adapters.
- Support terms and response times.
- Data handling and privacy language.
- No credential sharing in tickets or chat.
- No guarantee of platform acceptance, ad approval, SEO result, or social account outcome.
- Ownership of customer content versus XXYYZZ Society LLC / TheFAYTH tooling.
- Termination, refund, and export terms.

## Investor / Partner Sharing

Before NDA:

- Share product story, deck, demo screenshots, public repo, and Drive folder.
- Avoid private source, credentials, local queue state, unpublished customer data, and sensitive screenshots.

After NDA:

- Share selected architecture diagrams, guarded demo recordings, and sanitized receipts.
- Keep signing keys, passwords, tokens, and production credentials out of all shared packs.

## Decision

Do not add MIT, Apache-2.0, GPL, or AGPL to the Fantasia core repo right now. That would weaken commercial control before the business model is ready. Use a proprietary notice now, then selectively open-source helper pieces later if doing so creates distribution, trust, or developer adoption without giving away the engine.
