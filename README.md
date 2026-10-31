OpenBastion

Open-source Privileged Access Management for the Zero Trust era.

Secure privileged access. Protect every session. Trust nothing by default.

OpenBastion is an open-source initiative to build a modern, cloud-native Privileged Access Management (PAM) platform designed to secure, control, and audit privileged access across infrastructure, applications, and cloud environments.

Our mission is to make enterprise-grade privileged access security more transparent, accessible, extensible, and deployable — whether on-premises, in private clouds, or in Kubernetes environments.

Open source. Security by design. Built for modern infrastructure.

Why OpenBastion?

Privileged accounts remain one of the most critical attack surfaces in modern information systems. Shared credentials, uncontrolled administrative access, insufficient session visibility, and fragmented audit trails increase operational and security risks.

OpenBastion aims to address these challenges through a unified platform built around least privilege, identity-centric security, and complete session accountability.

Centralized privileged access — manage access to servers, databases, applications, and infrastructure from a unified control plane.

Credential protection — retrieve and use privileged credentials through controlled workflows without exposing secrets to administrators.

Session management — proxy, record, audit, and investigate privileged sessions.

Zero Trust architecture — enforce identity verification, authorization policies, and contextual access controls.

Just-in-time access — grant time-limited privileges with approvals and mandatory justification.

Comprehensive auditing — maintain traceable, tamper-evident records of privileged operations.

Cloud-native deployment — support containerized deployments, Kubernetes, on-premises infrastructure, and cloud environments.

Open and extensible architecture — integrate with existing identity providers, security tools, and automation platforms.

Core capabilities

OpenBastion is being designed around the following capability areas:

Capability

Scope

Identity & authentication

OIDC, SAML, LDAP, MFA, WebAuthn and enterprise identity providers

Authorization

RBAC, ABAC, least privilege and contextual policies

Privileged sessions

Proxied SSH, RDP, HTTP(S) and other supported protocols

Secrets management

Secure storage, controlled access, rotation and lifecycle management

Session recording

Terminal and graphical session recording, indexing and replay

Approval workflows

Multi-step approvals, access windows, expiration and ticket integration

Audit & compliance

Signed audit events, searchable activity trails and reporting

Threat detection

Risk scoring and detection of suspicious privileged activity

Developer experience

REST API, gRPC, CLI, SDKs and automation integrations

Deployment & operations

Docker, Kubernetes, Helm, observability and high availability

These capabilities represent the project vision and roadmap. Their implementation and maturity will be documented explicitly as development progresses.

Architecture principles

OpenBastion is being designed around a modular, service-oriented architecture with clear security boundaries.

Go for backend services and security-sensitive infrastructure components.

React, TypeScript and Vite for the web interfaces.

PostgreSQL for transactional data and durable application state.

Redis for caching and ephemeral coordination where appropriate.

NATS and Kafka for asynchronous messaging and event streaming, according to workload requirements.

OpenSearch for audit search and session indexing.

MinIO for encrypted session recordings and object storage.

Envoy and Traefik for proxying and traffic management.

Keycloak for identity federation and authentication integration.

OpenTelemetry, Prometheus, Grafana, Tempo and Loki for observability.

Security is a foundational architectural requirement, not an optional feature. The design prioritizes encrypted communications, mutual TLS between trusted services, strong authentication, least privilege, secrets isolation, and verifiable audit trails.

The architecture and technology choices will evolve through documented Architecture Decision Records (ADRs).

Security by design

OpenBastion aims to follow these principles:

Never trust by default. Every privileged access request must be authenticated, authorized, and evaluated against applicable policies.

Minimize credential exposure. Privileged credentials and cryptographic material must remain protected throughout their lifecycle.

Control the access path. Supported privileged protocols must be mediated by their designated security enforcement points, with direct-access paths restricted by network and infrastructure policy.

Record security-relevant activity. Access grants, session lifecycle events, policy decisions, and administrative changes must produce auditable records.

Protect audit integrity. Audit events should be tamper-evident, attributable, and verifiable.

Build security into delivery. Automated tests, dependency scanning, static analysis, container scanning, and security reviews should be part of the development lifecycle.

Security guarantees will be documented and validated against implemented controls and tested deployment configurations.

Project status

OpenBastion is an evolving open-source project.

The initial focus is to establish a sound architectural foundation before implementing the platform incrementally.

Our development priorities are:

Architecture, security boundaries, and ADRs.

API contracts and service interfaces.

Identity, authentication, authorization, and audit foundations.

A first end-to-end privileged access workflow.

Session proxying, recording, and investigation.

Production-ready deployment, observability, and operational documentation.

Features will be marked as planned, in progress, experimental, or stable according to their actual implementation and validation status.

Repository

Explore the organization to follow development across the project's components.

Key areas include:

Architecture & ADRs — system design, technical decisions, and security boundaries.

API & SDKs — contracts, developer interfaces, and integrations.

Backend services — identity, authorization, sessions, secrets, and audit.

Web & desktop clients — administration, access requests, and session workflows.

Deployment & operations — container images, Helm charts, Kubernetes, and observability.

Documentation & testing — developer guides, security guidance, and validation suites.

See the individual repositories for their current scope, status, and contribution instructions.

Get involved

OpenBastion welcomes contributions from developers, security engineers, infrastructure specialists, technical writers, and open-source enthusiasts.

You can help by:

Reviewing architecture proposals and ADRs.

Improving documentation and threat models.

Contributing code, tests, and security hardening.

Building identity-provider and infrastructure integrations.

Testing deployment scenarios and reporting reproducible issues.

Proposing improvements through GitHub Issues and Discussions, where enabled.

Before contributing, review the relevant repository's contribution guidelines, coding standards, and security policy.

Responsible security disclosure

Please do not publish exploitable vulnerabilities, credentials, private keys, or sensitive infrastructure details in public issues.

Follow the security reporting instructions published in the relevant repository's SECURITY.md. If a repository does not yet provide a disclosure channel, contact the maintainers privately before sharing sensitive details.

License

OpenBastion is intended to be distributed under the Apache License 2.0, subject to the license declared in each repository.

The Apache 2.0 license supports open collaboration, modification, and redistribution while providing an explicit framework for contributions and patent rights.

OpenBastion — Privileged access, under control.

Building a more secure and transparent future for privileged access management.