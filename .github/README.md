# OpenBastion — GitHub community configuration

This directory contains the GitHub configuration shared by the OpenBastion organization and its repositories.

OpenBastion is an open-source Privileged Access Management (PAM) project focused on controlled privileged access, credential protection, session accountability, and Zero Trust security. The organization uses this repository to keep community-facing guidance consistent across its projects.

## What belongs here

- **Issue templates** — structured bug reports, security-related reports where appropriate, and feature proposals.
- **Pull request templates** — contribution checklists and expectations for review.
- **Repository defaults** — shared contribution guidance and community health files.
- **Automation configuration** — reusable GitHub workflows or configuration only when their scope and permissions are clearly documented.

Repository-specific workflows and policies should remain in the relevant project repository when they depend on that project's build, test, release, or security requirements.

## OpenBastion contribution expectations

Contributions should:

1. Be original and compatible with the license of the target repository.
2. Preserve the project's security-first approach: least privilege, explicit authorization, protected credentials, and auditable changes.
3. Include focused tests or validation evidence when behavior changes.
4. Document security implications, operational impact, and configuration changes.
5. Keep pull requests reviewable, scoped, and linked to relevant issues or design decisions.
6. Follow the repository's contribution instructions and Developer Certificate of Origin (DCO) requirements wherever enforced.

Do not include credentials, private keys, access tokens, production secrets, personal data, or sensitive infrastructure details in issues, pull requests, logs, or test fixtures. Report suspected vulnerabilities using the private process described in [SECURITY.md](../SECURITY.md), not a public issue.

## License

The organization-wide default is **GNU AGPL-3.0-only**, unless a repository or file explicitly declares another license. See the canonical [LICENSE](../LICENSE) and [LICENSE.md](../LICENSE.md).

## Useful links

- [OpenBastion organization](https://github.com/openbastion)
- [Repositories](https://github.com/orgs/openbastion/repositories)
- [Contribution guide](../CONTRIBUTING.md)
- [Code of Conduct](../CODE_OF_CONDUCT.md)
- [Security policy](../SECURITY.md)

---

*OpenBastion — Secure privileged access. Protect every session. Trust nothing by default.*
