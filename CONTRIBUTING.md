# Contributing to 2048

Thank you for contributing!

Before contributing, please read our [Code of Conduct](CODE_OF_CONDUCT.md).

Please follow these guidelines to keep the project organized and secure:

## Reporting Issues

### Bug Reports
- Use the **Bug Report template**: `.github/ISSUE_TEMPLATE/bug_report.md`
- Include:
  - Steps to reproduce
  - Expected and actual behavior
  - Environment (OS, Java version, Maven version)
- **Do not report security issues here**. See [SECURITY.md](SECURITY.md) for responsible disclosure.

### Feature Requests
- Use the **Feature Request template**: `.github/ISSUE_TEMPLATE/feature_request.md`
- Describe:
  - Feature description
  - Problem it solves
  - Proposed solution
  - Alternatives considered

## Branch Management

- **Branches**:
  - **Main branch**:
    - `main`
    - Always protected
    - Only merge via PR
  - **Feature branches**:
    - `feature/<short-description>`
    - For new features
  - **Bugfix branches**:
    - `bugfix/<short-description>`
    - For bug fixes
  - **Release branches**:
    - `release/<version>`
    - For preparing a release
  - **Hotfix branches**:
    - `hotfix/<version>`
    - For urgent fixes to `main`
- **Conditions for merging into** `main`:
  - Only via Pull Request (PR)
  - Must pass all unit tests and CI workflow
  - Reviewed via PR and approved by at least one maintainer
- Delete branches after merge to keep the repo clean
- Tag releases following semantic versioning: `vMAJOR.MINOR.PATCH` (e.g., `v1.0.0`)

## Pull Requests
- Use the **Pull Request template**: `.github/PULL_REQUEST_TEMPLATE.md`
- Ensure your branch is up to date with `main` before submitting
- All tests must pass and build must succeed
- Include documentation updates if relevant
- **PR Types** :
    - Bug fix
    - New feature
    - Refactoring
    - Documentation update


## Commit Message Convention

Use the **Conventional Commits** style:  

```
[<scope>]<type>: <subject>
```

Examples:
- `[game]fix: correct score calculation`
- `[ui]feat: add keyboard controls`
- `[readme]docs: update instructions`
- `[maven]chore: update dependencies`

Types:
- `feat`: new feature
- `fix`: bug fix
- `docs`: documentation only
- `style`: formatting, missing semi-colons, white-space
- `refactor`: refactoring code
- `test`: adding or updating tests
- `chore`: build process or auxiliary tools

## Coding Standards
- **Java 11+** compatible
- 4-space indentation
- Maximum line length: 120 characters
- Braces required for all control structures
- No tab characters
- CamelCase for classes, lowerCamelCase for methods/variables
- Javadoc comments for public classes/methods
- Imports must be ordered and separated
- No unused imports
- Use **Maven** for build and dependency management
- Include unit tests for new functionality

## Release Policy
- Releases follow **semantic versioning**: `vMAJOR.MINOR.PATCH`
- **Release pattern**:
  - `main` as primary branch (trunk)
  - `feature/<name>` and `bugfix/<name>` branches for development
  - `release/<version>` branch for final fixes before tagging
  - Tags (`vMAJOR.MINOR.PATCH`) applied on `main`
  - CI must pass before merging any branch
- **Release requency**:
  - Patch releases: bug fixes -> as needed
  - Minor releases: new features -> monthly or bi-monthly
  - Major releases: breaking changes -> rare, announced in advance
- **Release Steps**:
  1. Ensure all features and bugfixes are merged into main
  2. Create a `release/<version>` branch from `main` to finalize the release and apply any last-minute bug fixes
  3. Run all tests and CI workflow on the release branch
  4. Update documentation if needed
  5. Merge the release branch back into `main`
  6. Tag the release on `main` with `vMAJOR.MINOR.PATCH`
  7. Delete the `release/<version>` branch

## Security
- If you discover a security vulnerability, **do not open a public issue**
- Follow the process in [SECURITY.md](SECURITY.md) to report security issues responsibly


## Additional Notes
- Keep PRs focused and small
- Reference related issues in your PR description
- Respect commit message conventions
- Add tests for any new functionality
- Update documentation when necessary