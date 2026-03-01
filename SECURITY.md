# Security Policy

## Reporting a vulnerability

Please **do not** open a public GitHub issue for security vulnerabilities.

Instead, report them privately using [GitHub's private vulnerability reporting](https://github.com/getloko/loko/security/advisories/new) in the relevant repository.

Include:
- A description of the vulnerability and its impact
- Steps to reproduce or a proof-of-concept
- Any suggested fix or mitigation (optional)

You'll receive an acknowledgement within 5 business days. We aim to release a fix within 30 days of confirmation.

## Scope

| Repository | In scope |
|------------|----------|
| [loko](https://github.com/getloko/loko) | CLI, generator, runner, plugins |
| [catalog](https://github.com/getloko/catalog) | Helm chart configurations |

LoKO is designed for **local development only** and should never be exposed to untrusted networks. Security issues relevant to local-only use cases (e.g., requiring physical access to the machine) are considered low severity.
