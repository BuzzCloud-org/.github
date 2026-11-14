
# BuzzCloud Security Policy

Security is a fundamental part of BuzzCloud's local-first, proximity-based networking architecture.

This policy explains how to report suspected vulnerabilities responsibly.

## Reporting a Vulnerability

**Do not report security vulnerabilities through public GitHub Issues, Discussions, or pull requests.**

Please use GitHub's private vulnerability reporting feature when it is enabled for the affected repository.

For supported repositories:

1. Open the repository's **Security** tab.
2. Select **Report a vulnerability**, if available.
3. Provide the relevant technical details privately.

If private vulnerability reporting is unavailable, do not publish exploit details. Contact the BuzzCloud maintainers through an established private communication channel to request a secure reporting method.

## Information to Include

When submitting a report, provide:

- A description of the vulnerability
- Affected BuzzCloud component and software or firmware version
- Relevant hardware and device revision, if applicable
- Steps to reproduce the issue
- Potential security impact
- Suggested mitigation, if known

Avoid including actual credentials, private keys, or sensitive personal information.

## Security-Sensitive Components

Particular attention should be given to:

- **Cell:** Individual identity, stored information, and access permissions
- **Stinger:** Proximity credentials, authentication, and credential misuse
- **Honeycomb:** Edge-node communications and device authentication
- **Hive:** Network services, access controls, and connections between devices
- **Queen:** Update distribution, software integrity, and cloud infrastructure

Security reviews should consider how systems behave both online and offline.

## Responsible Disclosure

We ask security researchers and contributors to:

- Report suspected vulnerabilities privately
- Avoid accessing or modifying information belonging to others
- Avoid disrupting networks or physical devices
- Allow maintainers an opportunity to investigate and address reported issues
- Coordinate public disclosure with maintainers when practical

## Security Updates

Security fixes should be reviewed and tested before release.

Firmware updates should consider device compatibility, release integrity, and recovery procedures.

Published release artifacts must not be silently replaced. Corrected versions should be distributed as new releases.

## Project Status

BuzzCloud is under active development.

Security mechanisms, supported versions, and reporting procedures will evolve as the platform matures.

No component should be assumed suitable for security-critical production deployment without appropriate testing and validation.

