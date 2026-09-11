# Contributing

Thanks for considering a contribution to one of my projects.

These are the default contribution guidelines for repositories under [`@ewanc26`](https://github.com/ewanc26) that do not provide their own `CONTRIBUTING.md`. Repository-specific documentation always takes precedence over this file.

## Before you start

- Read the repository's `README.md`, `AGENTS.md` files, licence, manifests, and CI workflows before making changes.
- Follow the most specific `AGENTS.md` that applies to the files you are editing. Nested guidance overrides broader repository guidance.
- Search existing issues and pull requests before starting substantial work to avoid duplicating an existing change.
- Preserve the project's existing architecture, naming, formatting, error handling, and dependency choices unless the change intentionally requires otherwise.

## Making changes

Keep changes focused. Prefer the smallest complete change that solves the problem rather than unrelated cleanup or broad refactors at the same time.

- Use atomic, scoped commits: one logical change per commit with a clear subject line.
- Add or update tests when behaviour changes and useful automated coverage is practical.
- Update documentation when public behaviour, setup, commands, configuration, or compatibility changes.
- Avoid unrelated formatting churn, generated-file changes, dependency updates, or lockfile changes.
- Do not remove compatibility or defensive behaviour without understanding why it exists.
- Never commit credentials, private keys, access tokens, signing material, personal data, or other secrets.

## Verification

Use the repository's documented toolchain and scripts rather than guessing equivalent commands.

Run the formatter, linter, build, type checks, and tests relevant to your change where they exist. For platform-specific or monorepo changes, run the checks for every affected component.

Be precise about verification. Do not claim a test, build, device check, network check, or manual validation that you did not actually perform. If something cannot be run locally, say so clearly in the pull request and explain what remains unverified.

## Pull requests

Submit changes through a pull request unless the repository explicitly documents another workflow.

A useful pull request should:

- explain what changed and why;
- stay scoped to one coherent piece of work;
- link relevant issues when applicable;
- include the exact verification performed and its result;
- call out compatibility, migration, security, accessibility, or operational impact where relevant; and
- leave CI passing before merge.

Address review comments with additional focused commits where practical. Do not rewrite or force-push shared history unless there is a specific reason to do so.

## Issues and feature requests

For bug reports, include enough information to reproduce the problem: the affected version or commit, environment, expected behaviour, actual behaviour, and relevant logs or screenshots with sensitive information removed.

For feature requests, describe the use case rather than only the proposed implementation. Changes that significantly alter architecture, compatibility, storage formats, protocols, or project scope are best discussed in an issue before implementation.

## Accessibility

For user-facing changes, preserve the platform's native accessibility behaviour and existing accessibility support. Consider keyboard and assistive-technology use, text scaling, contrast, reduced motion, focus order, and touch-target size where relevant.

## Licensing and third-party material

By submitting a contribution, you agree to license it under the licence of the repository unless an alternative has been explicitly agreed beforehand.

You must have the right to submit the contribution. Do not include code, assets, datasets, generated material, or other third-party content whose terms are incompatible with the repository's licence or that you are not authorised to redistribute.

## AI-assisted contributions

AI tools may be used when contributing, but the contributor remains responsible for understanding, reviewing, testing, and licensing the resulting work.

Do not submit generated changes blindly. Verify them against the actual repository and relevant upstream specifications or documentation. When an AI agent materially contributes to a commit, use an accurate `Co-authored-by:` trailer where appropriate.

## Questions

If the repository does not document a better contact route, open an issue or reach out on [Bluesky](https://bsky.app/profile/ewancroft.uk).