# OpenBastion Security Policy

OpenBastion is intended to help protect privileged access. Security reports are therefore treated seriously and should be handled responsibly.

## Reporting a vulnerability

**Please do not disclose suspected vulnerabilities in public GitHub issues, pull requests, discussions, or social media.**

Use GitHub's private vulnerability reporting feature for the affected repository, if enabled:

- [Report a vulnerability to the OpenBastion `.github` repository](https://github.com/openbastion/.github/security/advisories/new)

If private vulnerability reporting is not available for the affected repository, contact the organization maintainers privately through GitHub and ask for a secure reporting route. Do not publish exploit details while waiting for a response.

This repository-level link may not be the correct reporting destination for a vulnerability in another repository. Prefer the Security tab of the affected repository when available.

## What to include

Please provide as much of the following as you can safely share:

- A concise description of the issue and its potential impact.
- Affected repository, component, version, commit, or deployment configuration.
- Preconditions and steps to reproduce in a test environment.
- Proof-of-concept material sufficient to validate the issue, without accessing or modifying third-party data.
- Suggested mitigation, if known.
- Your preferred method for follow-up through GitHub.

Do not include real credentials, private keys, personal data, customer information, or data obtained from systems you do not own or have explicit permission to test.

## Coordinated disclosure

Please allow maintainers reasonable time to assess the report, reproduce the issue, develop a fix, and coordinate disclosure before making vulnerability details public.

We aim to:

1. Acknowledge a report within **5 business days**, where contact is possible.
2. Triage severity, scope, and affected versions.
3. Keep the reporter informed when practical.
4. Coordinate a fix, mitigation, and public advisory where appropriate.
5. Credit the reporter in a release note or advisory if they wish to be credited and it is safe to do so.

These are project goals, not a guaranteed service-level agreement. Response and remediation times may vary with severity, complexity, maintainer availability, and the project's maturity.

## Scope and safe testing

Only test systems you own or have explicit authorization to assess. Do not perform destructive testing, denial of service, social engineering, persistence, or access to data belonging to others.

If you discover an issue in a deployed OpenBastion instance, avoid accessing more data than is necessary to demonstrate the issue. Stop testing and report it privately.

## Supported versions

Until formal releases and a support policy are published:

- The latest development branch is assessed on a best-effort basis.
- No release should be assumed to be production-ready solely because it is publicly available.
- The affected repository's release notes and security advisories take precedence when they define a more specific support policy.

Supported versions and remediation status will be made explicit as the project establishes a release process.

## Security design is not a guarantee

Documentation may describe intended controls that are not yet implemented or independently validated. Do not treat planned functionality, experimental code, or an unreviewed deployment as a security guarantee. Review the actual release, configuration, threat model, and operational guidance before use.
