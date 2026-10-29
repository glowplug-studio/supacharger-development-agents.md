# Supacharger Core contributor instructions

Develop Supacharger Core for distribution to other developers; architecture and committed files must support reuse without depending on a contributor's local environment, private resources or personal tooling.

Follow the host's instruction entry point. For Core changes and work on the Docusaurus site, read [docusaurus-documentation-policy.md](docusaurus-documentation-policy.md). For an authorised Core commit or changelog request, read [core-changelog-policy.md](core-changelog-policy.md) and the host's `.agents/skills/changelog/SKILL.md`. If the skill is absent, install `general/changelog` with the CLI.

Installed skills and their installation records are local tooling in Core; do not commit them to Core. Applications choose their own skills and may commit them with their generated installation records. Maintain reusable skill source in its own repository.

## Icon conventions

Use `lucide-react` icons for shared concepts in Supacharger application interfaces and documentation. Use `<Brain />` for AI agents, agent setup, agentic development and AI-assisted actions. Use `<Wrench />` for manual setup, manual development and configuration work. Keep the same concept-to-icon mapping across navigation, cards and actions. Retain visible text labels; mark decorative icons with `aria-hidden="true"`.

This contributor repository is a separate Git submodule. Commit and publish its changes before recording a new revision in the host; ordinary Core updates do not update it.

## Canonical checkout for edits and publication

Make, review, commit and push each project's changes from its canonical local checkout. Identify the human-designated primary Core checkout before writing; use the established primary checkout for every other project. Being in a different chat does not authorise using a different checkout.

Do not create or use temporary clones, linked worktrees, alternate checkouts, cloud workspaces or GitHub/API file edits to author, commit, merge or push project changes unless the human explicitly requests that exception. Read-only clones for comparison are allowed but must never publish changes. Do not push another checkout's branch to the project's main branch.

Before editing, committing or pushing, verify the current directory, `git rev-parse --show-toplevel`, branch, remote and `git worktree list`. Coordinate agents on the canonical working tree; preserve other agents' changes and do not commit their work without authorisation. Never use an isolated release checkout to publish around a dirty canonical checkout. A submodule is a separate repository: edit and publish it from its established checkout, then record its revision in the parent.

If the remote is ahead, inspect and explain the incoming commits, then reconcile them in the canonical checkout when authorised. Do not overwrite remote history or force-push to conceal divergence. These instructions govern agent behaviour; they do not prevent a human or external system from updating the remote.
