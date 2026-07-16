# AGENTS.md

Guidance for agents working on the account-wide `.github` repository.

## Scope and inheritance

- `.github/` contains default community health files inherited by repositories that do not define their own versions.
- Root `CONTRIBUTING.md`, `SECURITY.md`, and `FUNDING.yml` are account-wide defaults.
- `gitignore/` and `gitattributes/` are reference templates copied manually; GitHub does not inherit them.
- `.github/linguist.yml` classifies build outputs as vendored and Nix files as documentation for language statistics.

## Rules

- Treat every change as potentially affecting many repositories. Keep defaults general and avoid stack-, license-, or project-specific claims.
- Security reporting instructions must use current private contact channels and must not encourage public vulnerability disclosure.
- Funding identifiers and links must be exact; never add payment secrets.
- Reference templates should be conservative: do not ignore source, fixtures, lockfiles, or required generated artifacts without a documented reason.
- Preserve line-ending/text normalization behavior in `.gitattributes` examples.
- Keep README inventory synchronized with actual files. At present it lists five ignore templates and the single default attributes template.

## Validation

Render and inspect all Markdown, validate YAML syntax, check links, and compare each template against the stack it claims to support. Verify no personal secrets, repository-specific commands, or contradictory contribution/security instructions are introduced. Because defaults inherit broadly, use a focused commit and review the complete diff before pushing.
