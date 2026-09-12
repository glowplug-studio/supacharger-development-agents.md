# Supacharger Core contributor instructions

This optional repository supplies contributor policies. Follow the host's root `AGENTS.md`, `.agents/supacharger/guidance.md` and `.agents/project/AGENTS.md`; use `docs/agents/` for Supacharger technical conventions. This file does not replace project instructions or duplicate the technical references.

Before an authorised Core commit, or when the human asks to update the Core changelog (including "do the changelog", "release notes" or "version history"), read `core-changelog-policy.md` beside this file and the host's `.agents/skills/changelog/SKILL.md`. If the skill is missing, install the public `general/changelog` skill with `supacharger skills install general/changelog` before continuing.

A request to commit Core changes authorises the accompanying Core changelog review; do not ask for that permission again. An application commit does not authorise Core changelog edits. A changelog request does not authorise committing or publishing.

Keep the changelog review and its checkpoint in the same commit as the reviewed changes. Preserve unrelated work and do not mark excluded changes as covered. Commit changes in this guidance repository separately before recording its submodule revision in the host. Never imply a local commit has been published.

This optional guidance is not CLI-managed. Update it deliberately through Git. Instruction-routing rules belong in the host's `.agents/supacharger/guidance.md`.
