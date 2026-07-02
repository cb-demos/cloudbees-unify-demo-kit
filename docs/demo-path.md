# Suggested Demo Path

## Opening story

"In discovery, we learned that your teams already have tools they like: GitHub, Jenkins, GitLab, Jira, ServiceNow, Kubernetes, and security scanners. The problem is not that these tools are bad. The problem is that leadership lacks end-to-end visibility, release coordination is manual, and governance is inconsistent. CloudBees Unify helps connect and orchestrate the toolchain without forcing a rip-and-replace migration."

## Suggested flow

1. Show the repo structure and explain that teams can keep their existing tools.
2. Show `.github/workflows/ci.yml` as an example of existing external CI.
3. Show `.cloudbees/workflows/ci.yaml` as a standardized CloudBees workflow pattern.
4. Show `deploy.yaml` as a reusable component deployment workflow.
5. Show `deployer.yaml` as the application-level deployer that orchestrates multiple components.
6. Pick one staged workflow:
   - `release-finsure-bank.yaml` for regulated financial services
   - `release-horizon-health.yaml` for healthcare/platform engineering
7. Use `policies/` to explain governance and approvals.
8. Use `mock-data/` to explain release evidence and auditability.
9. Close with business outcomes: visibility, governance, orchestration, developer productivity, and preserving existing tool investments.
