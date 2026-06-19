
# Product Surface Map

This map helps a GitHub visitor understand what parts of F@ntas1@ exist without exposing the private system.

| Surface | Visitor sees | Faith keeps private |
| --- | --- | --- |
| GitHub README | product promise, workflow, visuals, ownership | source code and operational internals |
| Docs folder | status, roadmap, feature matrix, architecture overview, policies | raw receipts, private runbooks, credentials |
| Assets folder | selected public-safe hero, banner, icon, social card, launch slides | private screenshots and dashboards |
| WordPress draft | project page copy and metadata for FaithCheltenham.com | live CMS access and publishing workflow |
| Website demo | static project-page preview | private routes and app runtime |
| Manifest | public export file list and hashes | private export source and release state |
| Launch checklist | human review and publishing steps | account credentials and final publish authority |

## Publishing Flow

1. Generate the public export from the private workspace.
2. Verify asset presence, secret scan, and manifest.
3. Overlay the export onto the existing GitHub repository clone.
4. Commit the public surface refresh.
5. Repair GitHub authentication.
6. Push the normal forward commit.
7. Publish the matching FaithCheltenham.com page after Faith review.
