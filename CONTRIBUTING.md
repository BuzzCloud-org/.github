
# Contributing to BuzzCloud

Thank you for your interest in contributing to BuzzCloud.

BuzzCloud is a local-first, proximity-based community networking platform. These guidelines establish a consistent engineering workflow while preserving the project's architectural principles.

## 1. Guiding Principles

All contributions should support the following goals:

- **Local-first operation:** Core functionality should not depend on continuous Internet access.
- **Proximity-based trust:** Physical proximity plays an important role in establishing relationships and authentication.
- **Individual and community autonomy:** Users and communities maintain meaningful control over their infrastructure and participation.
- **Modular architecture:** Components should have clearly defined responsibilities and interfaces.
- **Realistic hardware constraints:** Designs must account for the capabilities of embedded devices.
- **Incremental development:** Prioritize a narrow, working implementation over unnecessary complexity.

The architecture consists of Cell, Stinger, Honeycomb, Hive, and Queen. Changes to their responsibilities or trust boundaries require architectural review.

## 2. Issues and Planning

GitHub Issues is our primary engineering task tracker.

Before beginning substantial work:

1. Search for existing issues.
2. Create a Bug Report or Feature Request when appropriate.
3. Define the expected outcome and acceptance criteria.
4. Associate the issue with the relevant GitHub Project when available.

Architecture proposals and exploratory discussions may begin in GitHub Discussions before becoming actionable issues.

## 3. Branching Workflow

The default branch is `main`, which is protected.

Create short-lived branches for individual changes.

Suggested naming conventions:

- `feature/short-description`
- `fix/short-description`
- `docs/short-description`
- `chore/short-description`
- `test/short-description`

Keep changes focused and avoid mixing unrelated modifications.

## 4. Pull Requests

All normal development changes should be submitted through pull requests.

Pull requests should:

1. Clearly describe what changed and why.
2. Reference related GitHub issues when applicable.
3. Identify relevant testing and verification.
4. Document architectural or protocol impacts.
5. Avoid including secrets or sensitive information.

Use the organization's pull request template.

Prefer squash merging to maintain a readable `main` branch history.

Delete feature branches after successful merges.

## 5. Testing and Validation

Contributions should include testing appropriate to their scope.

For software changes:

- Confirm the project builds successfully.
- Run applicable automated tests.
- Verify that existing functionality remains intact.

For embedded firmware and hardware changes:

- Identify the target device and hardware revision.
- Document firmware and relevant dependency versions.
- Test on physical hardware when required.
- Record important limitations or unverified behavior.

Passing CI does not automatically establish that a feature works on physical hardware.

## 6. Architecture and Documentation

Changes affecting communication protocols, authentication, identity, security, or responsibilities between BuzzCloud components require additional review.

Significant architectural decisions should be documented with:

- Context and problem
- Decision
- Alternatives considered
- Consequences and trade-offs

Documentation should be updated alongside relevant implementation changes.

## 7. Security

Never commit passwords, private keys, access tokens, credentials, or other secrets.

Do not disclose suspected exploitable vulnerabilities through public issues.

Follow the repository's security reporting policy when available.

## 8. Releases

Release artifacts should be versioned and reproducible where practical.

Firmware releases should identify supported hardware, compatibility requirements, and validation status.

Published release artifacts must not be silently replaced. Corrections should use a new release version.

## 9. Collaboration

Technical discussions should remain respectful, focused, and documented when they influence project direction.

Contributors should communicate blockers early, keep issues current, and seek review when changes affect shared interfaces or architectural boundaries.

These guidelines will evolve as BuzzCloud grows.
