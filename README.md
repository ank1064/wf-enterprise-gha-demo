# WF Enterprise GHA Demo

Enterprise-shaped GitHub Actions samples for **Harness Unified Migrator + GHA Mapper** live demos.

## Live demo identity

| Item | Value |
|------|-------|
| **Repo** | [`ank1064/wf-enterprise-gha-demo`](https://github.com/ank1064/wf-enterprise-gha-demo) |
| **Primary pipeline name** | **WF Showcase Consumer Payments** |
| **Primary pipeline ID** | `wf_showcase_consumer_payments` |
| **Harness** | `nglabs` / `CSETest1` |

### Also published in Harness

| Name | Identifier | Notes |
|------|------------|-------|
| WF Showcase Consumer Payments | `wf_showcase_consumer_payments` | Migrator INLINE |
| WF Showcase Payments via Template | `wf_showcase_payments_via_template` | Mapper → `wf_java_payments_ci` |
| WF Showcase Payments Gap Filled | `wf_showcase_payments_gap_filled` | Gap-fill story |
| WF Showcase Payments Remote Vars | `wf_showcase_payments_remote_vars` | REMOTE + variable mapping |

Templates: `wf_java_payments_ci` (INLINE) · `wf_java_payments_ci_remote` (REMOTE GitX)

## Workflows

| Workflow | Demo story |
|----------|------------|
| `java-payments-ci.yml` | Primary convert + save pipeline/template |
| `java-payments-ci-gap.yml` | Mapper gap-fill |
| `digital-web-ci.yml` | Node web CI |
| `terraform-platform.yml` | Terraform guardrails |
| `card-services-ci.yml` | Reusable workflow caller |
| `reusable-enterprise-ci.yml` | Org reusable |
| `.github/actions/enterprise-security-scan` | Composite action |

## Migrator

1. Open Migrator → **GitHub Actions → Migration**
2. Select this repo on branch `main`
3. Migrate `java-payments-ci.yml`
4. Save as Pipeline / Template (Inline or Remote)
5. Use **Mapper** for template binding, gaps, and variables
