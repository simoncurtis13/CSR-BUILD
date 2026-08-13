# CSR/Alembee Repository Evidence Baseline

**Evidence date:** 13 August 2026  
**Rule:** This is a planning and static-inspection baseline, not build, deployment or production evidence.

## Connected estate

### `simoncurtis13/CSR-BUILD`

- Access confirmed: private repository with administrative read/write access.
- Role: independent CSR/Alembee build-control, traceability, handover and evidence repository.
- Boundary: holds planning and cross-repository control; it is not implementation proof, the customer runtime, or an ownership transfer mechanism.

### `mattrose271/Alembee-cdhq`

- Access confirmed: read/write.
- Default branch: `main`.
- Planning base: `4202737abf87cc7890e2e684dc8438482bd38098`.
- Observed: React/TypeScript/Vite client; Express server; Postgres/Drizzle schema; session/auth/RBAC/tenant features; candidates, clients, lead marketplace, payments/credits, interviews and integrations; GPTO proxy/submodule scripts; npm and Node 20; CI declarations for typecheck, lint, formatting, security and tests.
- Important static findings: `shared/schema.ts` is a very large mixed-domain schema; current package scripts reference adjacent/nested GPTO repositories; current server contains fixed external GPTO render/proxy assumptions; the README describes an ATS/lead marketplace, not the target CSR CRM.
- Planning disposition: primary product and CRM transformation line. Every module and table receives RETAIN, REMODEL, REMOVE, ADD or VERIFY status. No feature-development claim is made.

### `mattrose271/far`

- Access confirmed: read/write.
- Corpus baseline: `493bf59a0630f271d47ae47d30d3d2fe54fef3fe`; repin at W0.
- Observed from repository README/corpus: Next.js and Prisma web app; quote/admin/telemetry; rules orchestrator; Google Ads dry-run; Meta and LinkedIn stubs; shared packages.
- Planning disposition: donor of mobility, quote, orchestration, telemetry, Stripe and operator patterns. No stub or dry-run path is treated as production integration.

### `Conversion-Interactive-Agency/conversionai-system`

- Access confirmed: read/write; source-use authority remains contractual.
- Observed: pnpm monorepo; Fastify TypeScript API; Next.js web; Postgres migrations; worker; canonicalisation, source-of-truth, context, governance, execution, ledger, artifacts, RBAC, connectors and interface libraries.
- Planning disposition: authorised parent-adjacent CSR derivative. CSR receives separate repositories/deployments, cloud, identity, secrets, billing, communications, model accounts and data. Donor code ownership does not silently transfer.

### GPTO evidence lines

- `npgaring/GPTO`: read access; observed pnpm monorepo with Next.js dashboard, black-box runtime, shared packages and Drizzle/Postgres tooling.
- Corpus additionally registers current and prior GPTO code lines, including conversion-gpto and GPTO Insights pins. Their provenance must be reconciled in W0 before source selection.
- Planning disposition: preserve useful scanning, aggregation, caching, staged appraisal, report, export and telemetry components; transform them into the internal AISO service. Existing behavior cannot override the locked nine-stage contract.

### GIA and CIG

- Separate repositories contain build-ready plans and implementation scaffolds.
- Neither is represented as a production-ready dependency.
- CSR integrates versioned contracts and an explicit interim seam. Production switch-over needs conformance, divergence, replay, tenancy and operational evidence from the respective repository.

## Required W0 evidence

For every affected repository record:

- full repository URL and immutable SHA;
- file inventory and dependency graph;
- license, owner and permitted derivative/use boundary;
- build toolchain, environment requirements and secret classes;
- clean install/build/typecheck/lint/test result;
- database and migration assumptions;
- external accounts, APIs, webhooks and deployment dependencies;
- data classes, tenants, retention and deletion obligations;
- target disposition per file/module;
- source-to-target mapping and rollback tag; and
- unresolved access, provenance or rights issue with owner.

## Claims deliberately not made

- No current repository has been proven to implement the unified Alembee route.
- No README or CI declaration proves that checks pass at the pinned head.
- FullSteam capability, API rights and sandbox behavior have not been independently verified here.
- The donor repositories do not prove CSR ownership or derivative rights.
- GIA/CIG scaffold presence does not prove production admissibility or transition governance.
- GPTO-generated outputs do not prove deployment or commercial outcome.

