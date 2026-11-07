# Repository release instructions

## Mandatory factual release changelog

This rule applies to every GitHub Release, build release, prerelease, and future automated publishing workflow in this repository. Both Codex and Claude must follow it.

1. Every release must describe **real, specific changes since the previous release**, based on actual commits and the code diff. Explain what changed and where; include issue/commit references and any known limitations. Do not claim untested fixes or unsupported capabilities.
2. Never use generic filler such as "bug fixes", "performance improvements", "misc updates", "new features", or a copied/static note as the entire changelog. If a release only rebuilds the same source, label it as a **rebuild only** and state exactly what packaging, toolchain, signing, or artifact metadata changed. Do not invent application changes.
3. Keep the GitHub Release description and root `CHANGELOG.md` aligned. The `Factual release changelog` workflow audits actual source commits, adds evidence-linked notes to the release, and records the release in `CHANGELOG.md`. A failed audit is a release-policy failure that must be corrected, not ignored or disabled.
4. Release-producing workflows must prepare truthful release notes before publication. Treat the post-publication audit as an additional check, not permission to publish placeholders; never bypass the check or mark it non-blocking.
5. When a release contains user-facing assets, ensure version numbers and repo feeds also match the release. Existing installed-version rules remain in effect.

These instructions apply to changes by humans, GitHub Actions, Claude, Codex, and any other automation.
