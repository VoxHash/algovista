# Security Policy

## Supported versions

| Version | Supported |
|---------|-----------|
| 1.0.x   | Yes       |
| < 1.0   | No        |

## Reporting a vulnerability

Email **[contact@voxhash.dev](mailto:contact@voxhash.dev)** with:

- A description of the issue and impact
- Steps to reproduce (or a proof-of-concept if safe)
- Affected version / commit if known

Please do **not** open a public GitHub issue for security-sensitive reports.

We aim to acknowledge reports within 7 days and provide a remediation timeline after triage.

## Scope notes

AlgoVista is primarily a client-side educational Next.js application. There is no authentication or database in the core product. Still report:

- XSS or content injection in rendered UI
- Dependency vulnerabilities with a practical exploit path
- Misconfiguration that could leak optional env secrets in builds
