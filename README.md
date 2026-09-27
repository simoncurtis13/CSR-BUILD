# CSR-BUILD — Beem by CSR Build Control

This repository is the independent build-control home for Beem by CSR.

## Current operative Beem developer documents

Read these first and treat them as the controlling Beem product/build documents:

1. [`BEEM_FULL_PRODUCT_CANON_v1_0.md`](./docs/BEEM_FULL_PRODUCT_CANON_v1_0.md) — current product canon: what Beem is, product laws, boundaries, customer experience and required capability surface.
2. [`BEEM_FULL_BUILD_SPECIFICATION_v1_0.md`](./docs/BEEM_FULL_BUILD_SPECIFICATION_v1_0.md) — current implementation authority: architecture, contracts, modules, sequencing, tests, gates and acceptance criteria.

These two documents supersede the older planning package for deriving Beem implementation requirements. Older files remain in the repository as provenance until deliberate cleanup; they must not be used to create competing product semantics or build requirements.

The current canonical scope explicitly includes the governed marketing execution surface across web, SEO/AI search, paid search, paid social, organic social, email, written content, visual creative/art, CRM and measurement.

## Provenance / earlier planning package

The following files are retained for history, traceability, evidence and migration context only unless a current canonical document explicitly calls them back into scope:

- [`PRODUCT_CONSTITUTION.md`](./docs/PRODUCT_CONSTITUTION.md)
- [`PLAN_SOT.md`](./docs/PLAN_SOT.md)
- [`IMPLEMENTATION_PLAN.md`](./docs/IMPLEMENTATION_PLAN.md)
- [`REPOSITORY_EVIDENCE_BASELINE.md`](./docs/REPOSITORY_EVIDENCE_BASELINE.md)
- [`CROSS_REPOSITORY_HANDOVER.md`](./docs/CROSS_REPOSITORY_HANDOVER.md)
- [`TRACEABILITY_MATRIX.md`](./docs/TRACEABILITY_MATRIX.md)
- [`OPEN_OBJECT_REGISTER.md`](./docs/OPEN_OBJECT_REGISTER.md)
- [`CAPABILITY_AND_USE_CASE_SPEC.md`](./docs/CAPABILITY_AND_USE_CASE_SPEC.md)
- [`ACCEPTANCE_TEST_CATALOGUE.md`](./docs/ACCEPTANCE_TEST_CATALOGUE.md)
- [`MIGRATION_AND_CUTOVER_PLAN.md`](./docs/MIGRATION_AND_CUTOVER_PLAN.md)

Runtime and donor code remains in its own repositories. `CSR-BUILD` controls scope, traceability, dependencies, migrations, acceptance gates, evidence and release coordination; it does not silently transfer source ownership or collapse repositories into one codebase.

The documentation defines product/build authority. It does not by itself certify implementation, deployment, rights clearance, production readiness or commercial validation.
