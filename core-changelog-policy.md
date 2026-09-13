# Core changelog policy

Use the host's `CHANGELOG.md` for Core developers and maintainers; application changes belong in `CHANGELOG.project.md`. Select Keep a Changelog 1.1.0 and use the installed changelog skill for the self-contained formatting, evidence review and writing procedure.

A request to update Core release notes or commit Core changes authorises the review. An ordinary application commit does not. A changelog request alone does not authorise a commit or publication; copying published upstream release notes is not authoring new entries.

Review each authorised Core commit and keep its changelog checkpoint in that commit. Use the existing `changelog-review` comment: `reviewed_at` is UTC, `base_commit` is the commit preceding the reviewed change, and `main_commit` is the inspected main tip. Preserve `history_start`, which marks the beginning of audited history. Record the remote tip when inspected and identify excluded or local-only scope. Follow the skill when advancing the checkpoint; do not repeat its general procedure here.
