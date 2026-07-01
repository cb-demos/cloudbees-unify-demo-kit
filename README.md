# CloudBees Unify Candidate Demo YAML Assets

This repo is a lightweight starter kit for SE candidates building a CloudBees Unify demo. It assumes the candidate has access to a CloudBees Unify organization and will fork this repository, connect it to Unify, and adapt the workflows for one of the provided customer scenarios.

## What is included

- `.cloudbees/workflows/ci.yaml` - CloudBees Unify CI workflow starter
- `.cloudbees/workflows/deploy.yaml` - component deploy workflow starter
- `.cloudbees/workflows/deployer.yaml` - reusable application deployer workflow starter
- `.cloudbees/workflows/release-finsure-bank.yaml` - staged release workflow for FinSure Bank
- `.cloudbees/workflows/release-horizon-health.yaml` - staged release workflow for Horizon Health Systems
- `.github/workflows/ci.yml` - GitHub Actions CI workflow alternative for candidates who want to show external toolchain integration
- `k8s/` - Kubernetes manifests for a simple demo application
- `helm/unify-demo-app/` - basic Helm chart for deployment storytelling
- `manifests/` - sample release manifests for demo scenarios
- `policies/` - mock governance, approval, and change-control YAML
- `mock-data/` - mock Jira, ServiceNow, security, and release evidence data

## Suggested candidate demo path

1. Fork this repository.
2. Connect the forked repository to CloudBees Unify.
3. Create or select an Application in Unify, such as `Customer Portal`.
4. Create or select a Component, such as `orders-api`.
5. Use `.cloudbees/workflows/ci.yaml` to show a build/test/security workflow.
6. Use `.cloudbees/workflows/deploy.yaml` to show component deployment logic.
7. Use `.cloudbees/workflows/deployer.yaml` to explain reusable deployment orchestration.
8. Pick one scenario:
   - FinSure Bank: governance, auditability, risk, approvals
   - Horizon Health Systems: developer experience, release standardization, healthcare compliance
9. Use the matching staged release workflow to tell the end-to-end story from build to staging to production.
10. Use `mock-data/` and `policies/` as evidence during the presentation.

## Important note

These files are intentionally starter assets. Candidates should tailor the story, names, environments, and demo flow to match the selected customer scenario.
