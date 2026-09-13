# Docusaurus documentation policy

This policy governs `supacharger-docs/`, the human-facing documentation for Supacharger Core. Apply it when changing Core, promoting reusable consumer work into Core, or editing the Docusaurus site. Ordinary consumer work does not require a Docusaurus update.

## Decide whether a page needs to change

Review whether the approved Core change affects a supported capability, public contract, setup, configuration or an action a developer must take. Update the relevant Docusaurus pages in the same change when their explanation would otherwise be incomplete or wrong. Describe the implemented Core behaviour; do not present consumer customisations or planned features as current Core functionality.

A review does not require an edit. Keep internal cleanup, repository maintenance and agent workflow details in contributor guidance or implementation reports unless they change how a reader uses a supported feature. Do not append maintenance notes merely because a page mentions a related command, and do not repeat the same note across unrelated pages.

Review the affected README and agent technical references separately for their own audiences. Keep shared facts consistent, but do not duplicate their content or require every documentation surface to change. Report an unaffected surface briefly in the task result, not on the documentation site.

## Write for application developers

Supacharger is an open-source library used by other developers. Write for a mid-level developer: explain the purpose, behaviour and necessary steps in clear British English. Use technical terminology where it makes the explanation precise, explain unfamiliar Supacharger concepts, and avoid both unexplained internal jargon and tutorials on basic programming.

Document supported usage and decisions readers need to make. Keep examples accurate, use descriptive headings and put information on the page where a developer would look for it. Preserve official names, identifiers and quotations. Do not turn documentation into a development diary or a report of agent activity.

## Verify

Check affected commands, paths and links against Core. Use the documentation site's relevant validation and build checks. No Docusaurus update is needed solely to record that this policy was followed.
