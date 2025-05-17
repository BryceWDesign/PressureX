# PressureX Version Control Policy

## Purpose

This document defines the version control strategy for the PressureX project to ensure clear traceability, collaboration, and code quality.

---

## Branching Model

- **main**: Production-ready stable releases.
- **develop**: Integration branch for completed features.
- **feature/**: Feature-specific branches, named by feature (e.g., feature/sensor-update).
- **hotfix/**: For urgent fixes to main.

---

## Commit Guidelines

- Use **imperative mood** (e.g., "Add sensor calibration", "Fix power issue").
- Include clear, concise commit messages.
- Reference related issues or pull requests if applicable.

---

## Versioning Scheme

- Follow [Semantic Versioning 2.0.0](https://semver.org/):
  - MAJOR version when you make incompatible API changes,
  - MINOR version when you add functionality in a backwards-compatible manner,
  - PATCH version when you make backwards-compatible bug fixes.

---

## Releases

- Tagged in Git with version number (e.g., `v1.0.0`).
- Include release notes summarizing changes.

---

## Code Review

- All merges to `main` must be reviewed and approved by at least one team member.
- Use Pull Requests for all merges.

---

## Backup and Security

- Repository backups are maintained weekly.
- Access is restricted to authorized personnel.

---

Maintaining a disciplined version control policy ensures project integrity and audit readiness, critical for aerospace project credibility.

