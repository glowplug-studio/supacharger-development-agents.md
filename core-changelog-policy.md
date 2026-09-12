# Supacharger Core changelog policy

## Ownership and authorisation

The host repository's root `CHANGELOG.md` records reusable Supacharger Core changes for developers and maintainers. Application changes belong in `CHANGELOG.project.md`. Core contributors and contributors to Core forks maintain Core history through agents; ordinary application users do not.

Only a human request to maintain Core release notes or commit Core changes authorises edits. Copying upstream release notes unchanged during a Core update is not authoring new entries. The installed general changelog skill supplies the editorial procedure; installing the skill alone grants no permission to update Core history.

## Format and audience

Strictly follow [Keep a Changelog 1.1.0](https://keepachangelog.com/en/1.1.0/). Maintain `[Unreleased]`, use only relevant `Added`, `Changed`, `Deprecated`, `Removed`, `Fixed` and `Security` categories, and omit empty category headings. Released versions use `## [version] - YYYY-MM-DD`, newest first, with real comparison or release links. Use Semantic Versioning when making releases; never manufacture a release or version for an ordinary commit.

Use `.agents/skills/changelog/SKILL.md` in the host for evidence review and writing. Select a developer audience: public APIs, configuration, installation, security, compatibility, migrations and required upgrade actions can be notable. Internal agent housekeeping alone is not an entry; introducing a supported contributor workflow or installer is developer-visible. Explain outcomes and necessary actions without dumping Git logs.

## Review boundary

Read the latest `changelog-review` HTML comment. Its UTC `reviewed_at` is the last review timestamp; `base_commit` is the immutable commit immediately before the commit whose changes the review includes; `main_commit` records the inspected main tip. Inspect subsequent main history and the proposed commit, using ancestry as well as dates. Re-review the checkpoint-bearing commit and deduplicate it: this intentionally avoids a self-referential commit hash.

Review every authorised commit. If nothing notable changed, update only the review comment. Never record excluded working-tree changes as covered. Fail clearly if the required main history is unavailable; do not silently claim a complete review of stale remote history. A local-only review may proceed when labelled as such.

On first creation, record the inspected main tip as `history_start` and state that earlier history has not been retrospectively audited. Add only substantiated changes from the current change set, unless the human explicitly requests a historical backfill. Advance checkpoints only after successful review. Keep timestamps out of release headings except for standard release dates.
