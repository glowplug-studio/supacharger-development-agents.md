# Supacharger Core development guidance

Optional contributor policies for Core and Core forks. These files are not needed by application developers and are not managed by the Supacharger CLI.

From a Core checkout, install this repository with:

```bash
git submodule add git@github.com:glowplug-studio/supacharger-development-agents.md.git .agents/supacharger/core-development
supacharger skills install general/changelog
```

If `.gitmodules` already registers it, use `git submodule update --init .agents/supacharger/core-development` instead. Ordinary clones do not initialise it automatically. Updates are deliberate: fetch and check out a reviewed revision inside the submodule, then commit the parent gitlink. Contributor changes must be published before others can retrieve a newly pinned revision.

See [Contributing to Supacharger](https://supacharger.dev/docs/contributing) and [Agent guidance](https://supacharger.dev/docs/agents). The general changelog skill is maintained separately in [Glowplug skills](https://github.com/glowplug-studio/glowplug-skills/tree/main/general/changelog).

Contributor policies: [Docusaurus documentation](docusaurus-documentation-policy.md) and [Core changelog](core-changelog-policy.md). Installed skills remain local to a Core checkout; maintain their reusable source in the public skills repository.
