
# GitHub Publishing Handoff

## Target

- Repository: https://github.com/thefayth/fantas1a
- Public page: https://faithcheltenham.com/projects/fntas1a/
- Export folder: _github_public_export
- Publish clone: local publish clone

## Current Local State

The public package is generated locally from the private workspace export generator. A publish clone is used so the existing GitHub repository history can receive a normal forward commit instead of a force push.

## Publishing Status

GitHub authentication was repaired and the public package was pushed to the existing repository by normal forward commit. Future refreshes should use the same publish-clone flow instead of force-pushing over remote history.

## Safe Push Path For Future Refreshes

1. Open a shell in the local publish clone.
2. Confirm git status is clean except for the intended public-surface commit.
3. Confirm the remote is https://github.com/thefayth/fantas1a.
4. Run a secret scan against the publish clone.
5. Push the normal forward commit.
6. Verify the README, assets, workflow diagrams, docs, and ownership files render on GitHub.

## Do Not Push

- private tool state directories
- bus queue files
- telemetry/state logs
- raw coursework
- credentials or tokens
- private receipts
- local binaries
- private project workspaces
- unpublished sensitive material
