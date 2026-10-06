<!-- repository-standard: schema=1; standard=Repository Standards; version=1.1.0; scope=local-required; source=local -->
# Repository Settings Policy

## Important Boundary

GitHub does not inherit repository or organization settings from an account-level `.github` repository. This file publishes the approved policy. GitHub administration, configuration audits, & approved automation must apply and verify the actual settings.

## Fixed Defaults

| Area | Required Setting |
| --- | --- |
| Default Branch | `main` |
| Important Changes | Pull request with all applicable checks passing |
| Merge Methods | Squash only by default; rebase & merge commits disabled |
| Branch Cleanup | Delete merged branches automatically |
| Main Protection | Require pull requests, current checks, & resolved conversations; block force pushes & deletion |
| Actions Token | Read-only by default |
| Actions Pull Requests | Workflows cannot create or approve pull requests without an approved exception |
| Dependency Security | Dependency graph, Dependabot alerts, security updates, & local version-update configuration enabled |
| Secret Protection | Secret scanning & push protection enabled wherever supported |
| Vulnerability Reporting | Private Vulnerability Reporting enabled for public repositories |
| Unused Features | Disabled unless a documented purpose & owner exist |
| Private Runners | Approved Windows/Linux pair; selected private repositories only; never public or untrusted-fork accessible |
| Web Commit Signoff | Required where GitHub supports it |

## Profile-Selected Settings

Human approval counts, auto-merge, branch-update controls, code scanning, Issues, Projects, Discussions, Pages, webhooks, deploy keys, environments, secrets, variables, & allowed-actions restrictions depend on the repository purpose. Each enabled optional surface must have a documented purpose & owner.

## Organization Defaults

- Require two-factor authentication after access readiness review.
- Require owner review for ordinary-member repository creation.
- Require web commit signoff.
- Default Actions to read-only & prevent Actions pull-request approval.
- Enable dependency graph, Dependabot alerts, & security updates for new repositories.
- Review access, collaborators, runner groups, rulesets, & security configurations periodically.

## Approved Exceptions

- `RQG-PRIVATE-PLAN-001` permits compensating procedural controls only while a GitHub plan rejects native protection for a private repository.
- `terryrogers/DCC_LabStation_LS8` permits squash for routine pull requests & merge commits for governed milestones; rebase remains disabled & merged branches are deleted automatically.

Every other deviation requires a named owner, reason, compensating control, explicit approval, & review or expiry condition.
