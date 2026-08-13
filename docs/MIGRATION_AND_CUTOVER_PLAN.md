# CSR/Alembee Migration and Cutover Plan

## 1. Freeze and provenance

Pin and tag each donor before transformation. Record repository, full SHA, owner/licence, file inventory, dependencies, data stores, external accounts, environment/secret classes, build/test outcome and intended disposition. Do not rewrite donor history or treat a copy as a rights instrument.

## 2. CSR technical independence

Provision CSR-controlled repositories/branches, cloud projects, domains, identity, databases, storage, queues, model/AI accounts, billing, email/communications, secret storage, monitoring, incident access and supplier accounts. Document any time-bounded dependency and exit date. Customer data and CSR policies do not reside in Conversion-controlled accounts by default.

## 3. Substrate transformation

Create the authorised CGS derivative from the pinned baseline. Preserve neutral canonicalisation, state, context, governance, bounded execution, ledger/replay, RBAC and connector patterns that pass review. Remove recruiting identity and domain packages from the CSR build graph. Establish compatibility packages rather than copying divergent contracts into every repo.

## 4. cdHQ ATS-to-CRM migration

1. Inventory every table, field, file/object store, route, role, permission, report, seed, integration and retention dependency.
2. Classify each RETAIN, REMODEL, REMOVE, ADD or VERIFY.
3. Create target CRM schemas alongside ATS schemas.
4. Define field-level mapping, source/target IDs, tenant, purpose, lawful basis, retention and transformation version.
5. Run dry-run reports; no writes.
6. Run shadow-tenant migrations and reconcile counts, ownership, consent, relationships and timeline order.
7. Archive or delete excluded recruitment data with receipts.
8. Disable ATS writes and integration ingress.
9. Switch reads/UI to CRM models behind a reversible flag.
10. Remove ATS routes, roles, permissions, navigation, reports and seeds from the CSR release.
11. Retain a bounded compatibility/read-only window only if approved.
12. Rehearse rollback and verify no orphaned relationships or cross-tenant data.

## 5. GPTO-to-AISO migration

Reconcile current/prior GPTO lines before choosing source. Snapshot prompts, schemas, rubrics, stages, reports, tests and external dependencies. Reproduce builds/tests in isolation. Map existing sites, prompts, observations, telemetry and reports into tenant/site/source objects while preserving raw provenance.

Migrate the donor stage flow to the locked nine-stage contract. Backfill core/pack/profile/rubric/prompt/model/catalogue and source-hash bindings where supportable; unresolved legacy runs remain read-only and explicitly legacy. Shadow old/new outputs and reconcile scores, claims, lineage, package rationale and contamination before cutover.

## 6. FAR integration

Pin FAR and inventory web, orchestrator, database/shared/telemetry packages, quote/admin/operator routes, Stripe and deployment configuration. Map its concepts behind `MobilityRequest`, `MobilityOption`, `Quote`, `BookingProjection`, `PaymentProjection`, `DispatchObservation` and `ProviderReceipt`. Stubs and dry-run connectors remain disabled and labelled. Integrate through versioned contracts rather than merging databases by convenience.

## 7. Provider, payment, communication and CMS adapters

For each adapter: discover capabilities and rights; configure sandbox identity; map commands/events; implement idempotency, acknowledgement, observation and reconciliation; run shadow mode; verify rollback/disable; then grant the minimum live capability. Credentials are tenant/environment scoped and rotatable. Unsupported operations never fall through to a generic action.

## 8. GIA and CIG cutover

Implement versioned ports with current CSR state and policy mappings. Run GIA and CIG in shadow against labelled interim decisions. Review all divergence, latency, availability, tenancy and replay results. Switch only by approved policy version and feature flag, with immediate rollback. A failed/unavailable gate follows declared behavior and cannot become silent allow.

## 9. Data reconciliation

Every migration batch records source/target identity, tenant, row/object counts, relationship counts, mapping version, excluded/held records, error/discrepancy owner, start/end time and receipt hash. Reconciliation covers totals and semantics: ownership, consent, status, timeline order, currency, provider identifiers and current truth. Sampling alone cannot close high-risk PII or financial migration.

## 10. Cutover gates

- source and rights freeze accepted;
- independent infrastructure ready;
- migrations reproducible and rollback rehearsed;
- tenant/security/adversarial tests pass;
- connector sandbox/shadow observations reconcile;
- ATS and recruiting contamination absent;
- AISO old/new route reconciles and exact lineage passes;
- provider/payment/comms exceptions have operational owners;
- backup/restore and incident procedures pass;
- pilot scope, capacity and support are approved; and
- named owners sign the release decision.

## 11. Rollback triggers

Rollback or hold occurs on cross-tenant exposure, unbounded authority, unreconciled material data, payment/provider truth conflict without containment, unavailable critical provider without safe mode, recruitment data leak, broken AISO lineage, missing evidence/receipt, consent failure, unowned P0 exception, or observed load beyond the supported envelope.


