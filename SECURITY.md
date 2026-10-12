# Security policy

## Reporting a vulnerability

Please report suspected vulnerabilities **privately**, not as a public issue.

- Use GitHub's **Report a vulnerability** button on this repository's Security tab (private vulnerability reporting), or
- email <connect@graphowl.app> with the subject line `SECURITY`.

Please include what you found, how to reproduce it, and what you think the impact is. A proof of concept helps; it is not required.

## What to expect

- We acknowledge a report **within 5 working days**.
- We tell you whether we consider it a vulnerability, and keep you informed until it is fixed or closed.
- We do not run a paid bug-bounty programme.
- With your agreement we credit you in the release notes once the issue is fixed.

## Scope

In scope: the live demo at `demo.graphowl.app` and the website at `graphowl.app`.

Out of scope: social engineering of anyone involved with the project, denial-of-service or load testing, physical attacks, and vulnerabilities in third-party services we depend on (for example the hosting, DNS and mail providers) — please report those to the provider.

Please do not access, change or delete data that is not yours, and do not degrade the service for others. The demo contains synthetic data only, and a shared login, so findings that rely on having that login are in scope but expected to be low impact.

## Supported versions

GraphOWL is in early access. Only the version running at `demo.graphowl.app` is supported.

## Disclosure

We prefer coordinated disclosure: please give us a reasonable time to fix an issue before you discuss it publicly. We will not treat good-faith research that follows this policy as hostile.

## Keys and machine-readable contact

There is no PGP key yet. A `security.txt` file will be published at `https://graphowl.app/.well-known/security.txt` once the website is updated.
