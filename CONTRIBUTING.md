# Contributing to OpenBastion

Thank you for your interest in OpenBastion. We welcome contributions that improve privileged access security, usability, reliability, documentation, and the contributor experience.

OpenBastion is an evolving project. Please check the status of a repository and its documented capabilities before assuming a feature is implemented or production-ready.

## Before you start

- Read the [Code of Conduct](CODE_OF_CONDUCT.md).
- Read the repository's `README.md`, `AGENTS.md` (if present), development guide, and security notes.
- Search existing issues and pull requests before opening a new one.
- For significant changes, open an issue or discussion first to agree on scope and approach.
- Do not include credentials, tokens, private keys, customer data, production logs, or other sensitive information in issues, commits, tests, or pull requests.

Repository-specific instructions take precedence for build commands and implementation details, provided they do not conflict with this organization-wide guidance or the project's security requirements.

## What you can contribute

Examples include:

- Bug fixes and regression tests.
- Security hardening and threat-model improvements.
- Architecture Decision Records (ADRs) and design proposals.
- Documentation, examples, and translations.
- Identity-provider, infrastructure, and protocol integrations.
- Performance, reliability, accessibility, and developer-experience improvements.

Please avoid bundling unrelated changes into one pull request.

## Report bugs and propose changes

When opening an issue, include only information that is safe to publish:

- A concise description and expected behaviour.
- Reproduction steps and actual behaviour.
- Relevant versions, operating system, deployment mode, and configuration with secrets removed.
- Logs or traces with tokens, passwords, personal data, and internal identifiers redacted.

For feature proposals, explain the problem, intended users, security implications, alternatives considered, and how success could be validated.

**Do not report exploitable security vulnerabilities in public issues.** Follow [SECURITY.md](SECURITY.md) instead.

## Development workflow

1. Fork the repository, or create a branch if you have write access.
2. Start from the repository's default branch and create a focused branch:
   - `feat/short-description`
   - `fix/short-description`
   - `docs/short-description`
   - `security/short-description`
3. Make the smallest coherent change that solves the problem.
4. Add or update tests for behaviour changes and regression fixes.
5. Update relevant documentation, API contracts, ADRs, and examples.
6. Run the checks documented by the repository.
7. Review your diff for secrets, generated files, unrelated changes, and accidental compatibility breaks.
8. Push your branch and open a pull request.

Keep commits focused. Conventional Commit prefixes are recommended:

- `feat:` new functionality
- `fix:` bug fix
- `docs:` documentation
- `test:` tests
- `refactor:` internal restructuring without intended behaviour change
- `security:` security improvement
- `build:` build or dependency tooling
- `ci:` continuous integration changes

## Quality expectations

Contributions should, where applicable:

- Follow the repository's established architecture and style.
- Include meaningful automated tests; do not remove or weaken tests merely to make a change pass.
- Handle errors explicitly and avoid leaking secrets through logs, errors, metrics, or traces.
- Validate and authorize inputs at trust boundaries.
- Preserve secure defaults and least-privilege permissions.
- Document configuration changes, operational impact, and migration requirements.
- Avoid introducing unnecessary dependencies or broad permissions.
- Keep APIs and data migrations backwards-compatible where practical, or clearly document breaking changes.

For security-sensitive changes, describe the threat addressed, the trust boundary affected, and how the change was tested. Do not claim a security guarantee that has not been implemented and validated.

## Pull request checklist

Before requesting review, confirm that:

- [ ] The change addresses one clear problem or proposal.
- [ ] Tests cover relevant behaviour and edge cases.
- [ ] Applicable tests, linting, formatting, and static checks pass.
- [ ] Documentation and examples are updated.
- [ ] No secrets or sensitive data are included.
- [ ] Security, compatibility, and operational impact are described.
- [ ] The pull request explains what changed, why, and how it was validated.

If a check cannot be run, state which check was skipped and why. Do not report a check as passing unless it actually passed.

## Review and merge

Maintainers may request changes, additional tests, a design discussion, or a security review. Please keep review discussions technical and respectful. A pull request may be closed if it is out of scope, unsafe, inactive, or inconsistent with the project's direction.

Opening a pull request does not guarantee acceptance. Maintainers are responsible for final decisions on scope, implementation, release timing, and project direction.

## Licensing

By submitting a contribution, you agree that it may be distributed under the license applicable to the target repository. OpenBastion's intended default license is Apache-2.0; always check the target repository's `LICENSE` file before contributing.

You retain copyright in your contributions. Do not submit material that you do not have the right to contribute. If a contribution includes third-party code or assets, disclose their origin and license before submission.

## Questions

For project-specific questions, use GitHub Discussions or Issues where enabled. For sensitive security matters, use the private reporting process in [SECURITY.md](SECURITY.md).
