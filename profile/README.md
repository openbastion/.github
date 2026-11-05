<div align="center">

<!-- Replace this placeholder with the approved OpenBastion logo asset when available. -->
# OpenBastion

### Open-source Privileged Access Management for the Zero Trust era

**Secure privileged access. Protect every session. Trust nothing by default.**

[![License: Apache-2.0](https://img.shields.io/badge/license-Apache--2.0-blue.svg)](https://github.com/openbastion/.github/blob/main/LICENSE)
[![Open Source](https://img.shields.io/badge/open-source-community-brightgreen.svg)](https://github.com/openbastion)
[![Status](https://img.shields.io/badge/status-early%20development-orange.svg)](https://github.com/openbastion)

</div>

---

<picture>
  <img src="assets/github-metrics.svg" alt="Metrics">
</picture>


## What is OpenBastion?

**OpenBastion** is an open-source initiative to build a modern, cloud-native **Privileged Access Management (PAM)** platform for securing, controlling, and auditing privileged access across infrastructure, applications, and cloud environments.

The project aims to bring privileged access workflows, credential protection, session accountability, and policy-driven authorization into one extensible platform — deployable on-premises or in the cloud.

> OpenBastion is under active design and development. The capabilities described here are project goals, not a claim that every feature is currently implemented or production-ready.

## What we're building

- **Controlled privileged access** — mediate supported connections to servers, infrastructure, applications, and data services.
- **Credential and secret protection** — reduce credential exposure and support controlled use, lifecycle management, and rotation.
- **Session visibility** — record and investigate supported privileged sessions, with search and replay capabilities as they mature.
- **Zero Trust authorization** — apply identity-aware, least-privilege policies and contextual access decisions.
- **Just-in-time access** — support time-limited grants, justification, approvals, and expiration workflows.
- **Auditable operations** — make access decisions and security-relevant administrative activity traceable and tamper-evident.
- **Cloud-native operations** — target containerized deployments, Kubernetes, observability, and automation.
- **Open integrations** — design APIs and integration points for identity providers, ticketing systems, infrastructure, and security tooling.

## Architecture direction

OpenBastion is being designed with modular services and explicit security boundaries.

| Area | Planned technology direction |
| --- | --- |
| Backend services | Go |
| Web interface | React, TypeScript, Vite |
| Desktop client | Tauri |
| Transactional data | PostgreSQL |
| Cache and ephemeral coordination | Redis |
| Messaging and event streaming | NATS and Kafka, selected by workload |
| Audit search | OpenSearch |
| Session and object storage | MinIO |
| Proxy and traffic management | Envoy and Traefik |
| Identity integration | Keycloak, OIDC, SAML, LDAP and related standards |
| Observability | OpenTelemetry, Prometheus, Grafana, Tempo and Loki |
| Deployment | Docker, Docker Compose, Helm and Kubernetes |

Technology choices may evolve through documented Architecture Decision Records (ADRs). Security properties will be claimed only when the corresponding controls are implemented and validated.

## Security principles

OpenBastion's design is guided by:

- Least privilege and explicit authorization.
- Strong authentication and multi-factor authentication.
- Protected secrets and minimized credential exposure.
- Encrypted communications and service-to-service identity.
- Auditable access decisions and tamper-evident records.
- Protocol mediation and network controls to prevent unintended direct access paths.
- Automated testing, dependency hygiene, and security review throughout development.

## Project status

The project is in its early design and implementation phase. Initial priorities are:

1. Architecture, threat model, and Architecture Decision Records.
2. API contracts, data model, and service boundaries.
3. Identity, authentication, authorization, and audit foundations.
4. A minimal end-to-end privileged access workflow.
5. Session proxying, recording, and investigation.
6. Deployment hardening, operational guidance, and release validation.

Feature maturity will be stated per repository and release. Please do not rely on unreleased or experimental code for production security requirements without your own assessment.

## Explore the organization

Browse the [OpenBastion repositories](https://github.com/orgs/openbastion/repositories) to follow the work as components become available.

Useful starting points as they are published:

- **Architecture & ADRs** — design principles, trust boundaries, and technical decisions.
- **API contracts** — REST, gRPC, and integration specifications.
- **Backend services** — identity, authorization, sessions, secrets, and audit.
- **Web and desktop clients** — administration and privileged-access workflows.
- **Deployment & operations** — container images, Helm charts, Kubernetes, and observability.
- **Documentation & tests** — developer guides, security guidance, and validation suites.

Repositories and features will be linked here as they become available; no repository is implied to exist merely because it appears in this list of areas.

## Contribute

We welcome developers, security engineers, infrastructure specialists, technical writers, and community members.

- Read [CONTRIBUTING.md](https://github.com/openbastion/.github/blob/main/CONTRIBUTING.md).
- Follow the [Code of Conduct](https://github.com/openbastion/.github/blob/main/CODE_OF_CONDUCT.md).
- Report vulnerabilities privately using [SECURITY.md](https://github.com/openbastion/.github/blob/main/SECURITY.md).
- Explore open issues and discussions in the relevant repository, where enabled.

Security-related contributions are especially welcome when accompanied by tests, a clear threat description, and reproducible validation.

## License

OpenBastion's intended default license is [Apache-2.0](https://github.com/openbastion/.github/blob/main/LICENSE), subject to the license declared in each repository.

---

<div align="center">

**OpenBastion — Privileged access, under control.**

*Building a more secure and transparent future for privileged access management.*

</div>
