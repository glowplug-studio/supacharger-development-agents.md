# Supacharger Core contributor instructions

Develop Supacharger Core for distribution to other developers; architecture and committed files must support reuse without depending on a contributor's local environment, private resources or personal tooling.

Follow the host's instruction entry point. For Core changes and work on the Docusaurus site, read [docusaurus-documentation-policy.md](docusaurus-documentation-policy.md). For an authorised Core commit or changelog request, read [core-changelog-policy.md](core-changelog-policy.md) and the host's `.agents/skills/changelog/SKILL.md`. If the skill is absent, install `general/changelog` with the CLI.

Installed skills and their installation records are local tooling in Core; do not commit them to Core. Applications choose their own skills and may commit them with their generated installation records. Maintain reusable skill source in its own repository.

## Icon conventions

Use `lucide-react` icons for shared concepts in Supacharger application interfaces and documentation. Use `<Brain />` for AI agents, agent setup, agentic development and AI-assisted actions. Use `<Wrench />` for manual setup, manual development and configuration work. Keep the same concept-to-icon mapping across navigation, cards and actions. Retain visible text labels; mark decorative icons with `aria-hidden="true"`.

This contributor repository is a separate Git submodule. Commit and publish its changes before recording a new revision in the host; ordinary Core updates do not update it.
