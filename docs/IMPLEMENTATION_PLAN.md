# Alembee by CSR — Repository Implementation Plan

**Status:** Corpus-aligned implementation plan; no phase completion implied  
**Target:** Controlled staging vertical slice in eight weeks after PD0

## Evidence and phase rules

A phase is complete only when its named code and migrations are merged on a named SHA; required positive, negative, tenancy, security and replay tests pass; evidence is stored at the declared location; the responsible owner records pass/fail; and rollback or remediation is proven. Narrative, source presence, a rendered page, an API `200`, a generated report or a self-authored status statement is not completion evidence.

Each implementation issue must state: controlling source, repository and component, dependency, owner, object/contract changes, migration, acceptance tests, at least one negative scenario, evidence location, evidence label, rollback and open-object dependency.

Evidence labels are `PLANNED`, `SPECIFIED`, `IMPLEMENTED`, `TESTED`, `STAGED`, `OBSERVED`, `RECONCILED` and `PRODUCTION`. Labels are earned independently; later labels require evidence and do not arise automatically from earlier ones.

## PD0 — Development start gate

- [ ] Approve `PLAN_SOT.md`, `PRODUCT_CONSTITUTION.md` and this plan.
- [ ] Freeze repository heads and record source inventories.
- [ ] Approve the cross-repository dependency, authority and migration map.
- [ ] Name technical, product, commercial, data/privacy, security, finance, provider and operations owners.
- [ ] Link every epic to acceptance, negative, migration and rollback evidence.
- [ ] Create one GitHub Project with W0–W8 milestones and Backlog/Ready/In progress/Review/Evidence/Done/Blocked states.
- [ ] Resolve or explicitly gate every open object.

**PD0 done:** repository-specific plans and cross-repository handover are accepted by relevant owners. This authorises implementation planning and controlled development only—not migration or release.

## W0 — Evidence freeze, rights and independence

### E00 IP, licence and independence

- Inventory donor code, data, brands, deployments, domains, model accounts, billing, secrets, communications, improvements and inventions.
- Execute or place a legal hold on the source-use/asset schedule before derivative code transfer.
- Establish CSR-controlled accounts and name credential owners.

**Done:** every source and operational dependency has a named owner, permitted-use decision and independence route; prohibited transfers are documented and blocked.

### E01 Repository estate and baselines

- Pin Alembee-cdhq, FAR, Conversion CGS, all GPTO evidence lines, GIA and CIG.
- Capture file inventories, dependency graphs, database assumptions, environments and build/test results.
- Record immutable rollback tags and unresolved access/provenance.
- Reconcile adjacent/nested GPTO paths referenced by Alembee-cdhq.

**Done:** all baselines are reproducible or have an exact blocker; no donor repository is mutated without authority.

### E01A Transformation registers

- Produce file/module RETAIN/REMODEL/REMOVE/ADD/VERIFY maps for cdHQ and FAR.
- Produce the ATS data and PII disposition register.
- Produce provider capability and connector registers.

**Done:** no component enters the target architecture by assumption or name similarity.

## W1 — Neutral substrate, identity and canonical state

### E02 Neutral platform namespace

- Create the authorised CSR derivative of CGS at the pinned source SHA.
- Remove recruiting product semantics from packages, routes, configuration and UI.
- Publish neutral contracts only where two repositories require them.

**Done:** CSR runtime, accounts, data and deployments have no mandatory production dependency on Conversion; provenance remains intact.

### E03 Tenant/RBAC and inherited security repair

- Bind tenant and environment at request, repository, worker, event, prompt, connector and replay layers.
- Replace wildcard CORS and privileged tenant-bypass behavior.
- Implement service identity, least privilege, MFA/session controls where applicable, secret management and negative tenant tests.

**Done:** cross-tenant read/write/replay/hydration fail closed; missing service identity or authority never defaults to allow.

### E04 CSR state registry

- Implement versioned canonical objects from `PLAN_SOT.md` section 6.
- Add lifecycle, provenance, source/target identity, environment and attribution.
- Introduce outbox/event publication and idempotent consumers.

**Done:** all v1 objects and lifecycle transitions have schemas, migrations, repositories and contract tests.

## W2 — Governed route and evidence kernel

### E05 Commercial state and WorkPacket

- Implement WorkPacket v1, versions, transition table and explicit missing/conflicting state.
- Bind every handoff to tenant, identity, purpose, evidence, payload digest, correlation/causation and idempotency.

**Done:** proposal, approval, attempted, acknowledged, observed, discrepant, unknown, reconciled and failed states cannot collapse into each other.

### E06 Patent-aligned execution path

- Implement TransitionDecision, ComputeDecision, exact ExecutionGrant, capability envelope, expiry, kill/rollback and adapter binding.
- Preserve legal caveats: implementation mapping does not assert patent grant or freedom to operate.

**Done:** altered payload/target/environment/tenant/operation invalidates a grant; an agent cannot widen its own authority.

### E17 GIA seam and E17A CIG seam

- Define versioned request/response ports and health/divergence behavior.
- Label interim decisions `CGS_INTERIM`.
- Shadow GIA/CIG decisions and reconcile divergence before any switch.

**Done:** unavailable GIA/CIG follows declared fail-closed/interim policy; no silent allow and no false GIA/CIG attribution.

### E19 RouteLog, evidence and replay

- Store ordered route events, decisions, grants, attempts, acknowledgements, observations, discrepancies, exceptions and re-entry.
- Implement deterministic read-side reconstruction and adapter-safe replay.

**Done:** replay reproduces decisions and views without invoking production adapters; every material state is traceable to source and owner.

## W3 — cdHQ ATS-to-CRM transformation

### E07 CRM domain transformation

- Create Account, Contact, Consent/Contactability, Opportunity, Activity, Relationship, Owner and Timeline schemas beside donor ATS schemas.
- Remodel approved client/candidate/recruiter/application/activity/source semantics through explicit mappings.
- Build unified account workspace, task/exception queue and management views.

**Done:** the CRM is the live system of engagement without becoming provider, payment or governance truth.

### E07A Data migration and ATS retirement

- Run tenant-bound, versioned migration jobs in test/shadow tenants.
- Preserve source/target identity, lawful basis, mapping, counts, relationships and receipts.
- Archive/delete excluded candidate/CV/document data and disable ATS writes, routes, roles, reports, navigation and seed data.

**Done:** record counts, ownership, consent, relationships and timelines reconcile; no ATS or recruitment object is reachable; rollback is rehearsed.

### E07B Integration contracts

- Accept AISO leads/opportunities idempotently without authorising consequences.
- Project governed quote, payment, communications, mobility and provider observations into the CRM.

**Done:** duplicate handoffs create one canonical transition; CRM cannot overwrite source-system truth.

## W4 — AISO acquisition intelligence

### E13 GPTO transformation

- Reproduce all selected GPTO builds/tests in isolation.
- Inventory scanning, data acquisition, caching, appraisal, strategy, proposal, report, export, price/payment and test components.
- Retain/refactor/replace/add each component; remove GPTO as customer identity.
- Map inherited tables, executors, tokens and external services.

**Done:** selected code has provenance, tenant/site binding and migration mapping; donor behavior does not override the target contract.

### E15 Locked nine-stage AISO route

- Implement admitted scope, evidence classes, five independent modules, exactly-five-pillar scorecard, appraisal acceptance, appraisal-only strategy, strategy acceptance, strategy-only proposal and independent final QA.
- Bind site, tenant, core, pack, organisation profile, rubric, prompt, model, catalogue and source hashes to each stage.
- Invalidate downstream artifacts when material upstream state changes.

**Done:** one chauffeur, one motor-coach and one mixed-fleet fixture pass lineage, scoring, confidence, contamination, package and three-file conformance tests.

### E14 Source/proof repository

- Store approved evidence, claims, freshness, rights, trust gaps and access limits.
- Hydrate pages, prompts, reports and work packets only from permitted sources.

**Done:** every finding resolves to evidence or an explicit unknown; unsupported claims cannot enter accepted artifacts.

### E28 Vertical packs and dynamic demand/pages

- Extract chauffeur/motor-coach behavior into Vertical Intelligence Pack 1 without changing the accepted route.
- Implement pack schema, compiler, reviewer separation, versioning, conformance, revocation and rollback.
- Generate dynamic-page proposals without autonomous publication.

**Done:** a pack cannot alter core pillars, route law, evidence classes or authority; old/new shadow outputs reconcile.

## W5 — Acquisition actions, mobility, quote, payment and communication

### E08 Ride intake and matching

- Implement transport demand profile, missing-state handling, fleet/capability/credential constraints and explainable options.

**Done:** missing licence, permit, insurance, accessibility or capacity becomes a visible hold/unknown; it is never guessed.

### E09 Quote and pricing

- Implement immutable quote versions, assumptions, catalogue/price binding, customer-of-record and approval/expiry.

**Done:** any material payload change invalidates prior approval; accepted quote can be reconstructed exactly.

### E11 Payment

- Implement bounded payment intents, webhook idempotency, refunds/chargebacks, reconciliation and finance approvals.

**Done:** payment projection matches PSP observation; duplicates are safe; unauthorised refund is held.

### E12 Communications

- Implement templates/drafts, consent/contactability checks, approval, exact-recipient/payload binding, send receipts and suppression.

**Done:** an AI draft cannot send itself; unsubscribe, suppression, bounce and do-not-contact are enforced.

### E16 and E21 Governed web/channel actions

- Add CMS/web, organic search, paid search, paid/organic social and email connectors as separately capability-discovered adapters.
- Keep spend, audience, content and publish actions behind exact grants and rollback.

**Done:** no score or recommendation executes directly; dry-run/stub connectors remain visibly non-production.

## W6 — FullSteam and fulfilment

### E10 FullSteam adapter

- Discover supported client/fleet/rate/availability/quote/booking/assignment/status/billing/webhook functions.
- Implement commands, receipts, webhook ingestion, polling/reconciliation, freshness and discrepancy states.

**Done:** one sandbox route distinguishes accepted request from observed provider outcome, survives duplicate webhook and timeout, and exposes an owned exception.

### E10A Portfolio capability port

- Bind provider/company capability, credentials, geography, fleet, service, availability, pricing constraints and expiry.
- Prevent umbrella brand from implying ownership or coverage.

**Done:** unsupported/unverified functions and capacity remain typed and cannot be sold or dispatched.

## W7 — Attribution, compliance and operating system

### E18 Attribution and re-entry

- Join source, page/prompt/campaign, account, opportunity, quote, booking, payment, provider observation and revenue evidence.
- Emit discrepancy and re-entry instructions when evidence changes.

**Done:** telemetry alone cannot prove conversion; corrected outcome deterministically updates downstream reports.

### E20 Pilot operations and E24 portfolio onboarding

- Implement guided account/connector/policy onboarding, readiness gates, cohort templates with delta review and support ownership.

**Done:** one authorised account can be provisioned reproducibly without overwriting tenant-specific claims or permissions.

### E25 Workforce operations

- Implement BPO/fractional assignments, sampling, review, escalation, capacity and audit.

**Done:** every manual/assisted task has owner, scope, evidence, QA and escalation; no shared omnipotent operator account exists.

### E26 Agent authority envelopes

- Bind delegated agent work to objective, sources, tools, audience, spend, consequence, expiry and escalation.

**Done:** agent-to-agent handoff cannot turn candidate state into authority or leak tenant context.

### E27 Management reporting

- Reconcile acquisition, funnel, quote, booking, fulfilment, revenue, cost, partner share, collections, margin, support and risk.

**Done:** dashboard totals reconcile to RouteLog and source observations; discrepancies remain visible.

### E29 Client-site compliance

- Implement cookie/storage inventory, purpose classes, activation/refusal/withdrawal, retention/export/deletion and client/subprocessor responsibility views.

**Done:** optional tracking is blocked before permission; withdrawal propagates and is evidenced; production behavior matches disclosure.

## W8 — Productisation and release decision

### E22 SaaS productisation

- Complete tenant provisioning, guided connector setup, policies, account/channel workspaces, RouteLog, reports, usage, billing, support, export and deletion.

**Done:** customer sees only Alembee identity and can administer its bounded account without donor terminology or cross-tenant exposure.

### E23 Agentic account manager

- Ship shadow mode first; compare proposals, decisions, exceptions and outcomes.
- Enable consequential management only through explicitly approved capability/spend envelopes.

**Done:** shadow evidence and exception performance satisfy approved thresholds; kill, revoke and human takeover are rehearsed.

### E30 Release, security and resilience

- Run migration rehearsal, tenant/security/adversarial suite, load tests, provider/webhook burst, backup/restore, rollback and incident rehearsal.
- Run a controlled cohort/portfolio simulation and document measured limits.

**Done:** named security, data, operations, finance, commercial and product owners sign the release record with open risks and rollback path.

## P0 negative conformance suite

The build fails if any of these are possible:

- cross-tenant state, token, evidence, prompt, connector or replay access;
- consequence without identity, purpose, capability, exact grant or receipt path;
- altered payload or target using an old approval;
- production adapter invocation during replay;
- timeout or HTTP acknowledgement recorded as completed outcome;
- CRM projection overwriting contradictory provider/payment truth;
- AISO output with four/six pillars, broken lineage or recruiting content;
- strategy reading raw evidence, or proposal adding facts not in accepted strategy;
- unverified analytics, rankings, capacity or revenue written as observed fact;
- package selection without score/unknown/rationale and why-not analysis;
- suppressed contact entering a send queue;
- candidate/CV/recruitment history migrating without approved purpose and retention;
- ATS route/role/report/navigation reachable in the CSR release;
- agent widening its own authority, spend, tool or audience;
- missing/expired capability or credential proceeding to allocation/dispatch;
- umbrella brand implying ownership, certification, capacity or coverage;
- cross-client Market Memory without participation and cohort threshold;
- GIA/CIG outage becoming silent allow; or
- provider capability marketed without verified API/right.

## Release statement

The eight-week release is accepted only when the entire section 3.1 route in `PLAN_SOT.md` passes with named commits, environments and evidence. It remains a controlled staging release; it does not by itself prove production adoption, market fit, legal sufficiency, portfolio economics or multi-vertical readiness.


