# Development Workflow

This document describes the branching strategy, pull request process, and CI/CD expectations.

## Branching Strategy
*   `main`: The stable, production-ready branch. Direct commits are forbidden.
*   `develop`: The active integration branch. Feature branches merge here.
*   `feature/feature-name`: Branch for developing a specific feature. Branch off `develop`.
*   `bugfix/bug-name`: Branch for fixing a bug.
*   `release/vX.Y.Z`: Branch for preparing a release.

## Pull Requests
*   All changes must be submitted via a Pull Request (PR) to the `develop` (or target) branch.
*   PR titles should follow conventional commits (e.g., `feat: add login screen`, `fix: resolve crash on startup`).
*   PR descriptions should detail what was changed and why.
*   All automated checks (CI) must pass before merging.

## CI/CD Pipeline
*   The pipeline should automatically run detekt/ktlint, unit tests, and build an APK for every PR.
*   Merging to `develop` triggers a snapshot build.
*   Merging to `main` (via release branch) triggers a production build.
