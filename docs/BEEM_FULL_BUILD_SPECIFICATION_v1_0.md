# BEEM FULL BUILD SPECIFICATION v1.0

Product: Beem by CSR

Status: OWNER-DIRECTED REPLACEMENT BUILD SPECIFICATION / CURRENT IMPLEMENTATION AUTHORITY

Audience: CSR and Beem product, engineering, data, security, operations and delivery teams

Companion document: BEEM_FULL_PRODUCT_CANON_v1_0.md

Repository role: This specification defines how Beem is to be built. Together with the Beem Full Product Canon, it is intended to replace earlier operative build-plan documents in the developer workflow. Older material may remain as provenance until repository cleanup is complete, but it must not be used to derive competing requirements.

Evidence boundary: This document is a build authority and implementation specification. It is not proof that a capability is implemented, deployed, rights-cleared, operationally exercised or commercially validated.

---

# PART I — BUILD CONTRACT

## 1. Purpose

This document converts the Beem Product Canon into a buildable engineering programme.

It defines:

- the target runtime architecture;

- module ownership and boundaries;

- repository topology;

- canonical domain objects;

- state, truth, freshness and provenance rules;

- Beem Local Control Plane contracts;

- WorkPacket and consequence lifecycle;

- forecasting and sell-through implementation;

- adaptive Recipe Runtime;

- Account Manager orchestration;

- Workspace Compiler;

- capability and connector architecture;

- identity, security, privacy and tenancy;

- eventing, idempotency, receipts, observation and reconciliation;

- APIs and event contracts;

- migration and legacy-code adaptation rules;

- observability, SLOs and operational support;

- test strategy and mandatory negative paths;

- CI/CD and release controls;

- sprint-by-sprint delivery sequence;

- acceptance gates for Phase One and Phase Two;

- Definition of Done;

- open decisions that must remain explicit rather than guessed.

The development team should be able to use this document to create epics, tickets, ADRs, interfaces, migrations, tests and release gates without reconstructing the product from earlier plans.

## 2. Companion-document rule

There are only two operative Beem build documents:

- BEEM_FULL_PRODUCT_CANON_v1_0.md — what Beem is, what it does, product laws, user experience and use cases.

- BEEM_FULL_BUILD_SPECIFICATION_v1_0.md — how Beem is implemented, modularised, tested, sprinted and released.

If this specification appears to conflict with the Product Canon, the Product Canon controls product meaning and this specification must be corrected.

No developer, coding agent or implementation ticket may create a third source of product truth.

## 3. Build objective

Build one CSR-controlled Beem product in which:

- every customer operates through one tenant-isolated Account;

- commercial objectives are durable objects, not conversation-only context;

- AccountPlans are versioned and measurable;

- forecasts are versioned analytical outputs, never authority;

- multiple viable opportunity horizons can be preserved before selection;

- WorkPackets bridge intelligence to consequence;

- Beem acquisition intelligence is a specialist capability inside the same Account;

- CRM and revenue state are part of the same commercial operating model;

- adaptive Recipes package reusable operating knowledge without customer data;

- the Workspace Compiler renders objective-specific workspaces from approved components;

- the Account Manager coordinates durable work without creating authority;

- BLCP owns qualified state, policy, authority, exact-operation binding, receipts, observation, reconciliation and re-entry;

- external systems are reached only through registered capability contracts;

- provider acknowledgement never substitutes for verified business outcome;

- every material consequence is replayable from evidence without replaying the side effect;

- the system can safely hold, request state, recompute, escalate or stop when required state is missing.

## 4. Absolute build locks

- Beem product semantics are owned by CSR/Beem.

- BLCP is the Beem-local control plane.

- No external governance runtime is required for Beem to operate.

- Model output is candidate state, never permission.

- Forecast is candidate analytical state, never permission or guarantee.

- Role membership is access control, not exact consequence authority.

- Connector capability is technical ability, not permission.

- Approval is evidence into authority resolution, not blanket future authority.

- State may cross interfaces; authority and consent do not silently transmit.

- Exact material operations are separately bound.

- Provider acknowledgement is not verified outcome.

- Unknown remains UNKNOWN until reconciled.

- Missing state is requested, held or escalated; it is not invented.

- Conversation memory cannot override current qualified state.

- The Account Manager cannot widen its own authority or tool set.

- Replay cannot trigger live side effects.

- Tenant isolation is fail-closed.

- Recipes never contain customer data or inherited customer authority.

- Workspace compilation uses approved components and manifests; it does not generate arbitrary production code.

- Legacy implementation material is donor input only. Presence in the repository does not make it Beem truth.

- Every maturity claim uses explicit evidence labels.

## 5. Claim ladder

Use only these maturity states:

- PLANNED

- SPECIFIED

- SCAFFOLDED

- IMPLEMENTED

- UNIT_TESTED

- CONTRACT_TESTED

- INTEGRATION_TESTED

- NEGATIVE_PATH_TESTED

- STAGING_DEPLOYED

- PRODUCTION_DEPLOYED

- OPERATIONALLY_EXERCISED

- COMMERCIALLY_VALIDATED

No later state is inferred from an earlier one.

---

# PART II — TARGET SYSTEM ARCHITECTURE

## 6. Layer model

### 6.1 Experience layer

Owns Account Pulse, Account Manager, Plan, Forecast, Pipeline/CRM, Work/Approvals, Acquisition Intelligence, Connections, Evidence, Settings/Policy/Permissions and compiled objective-specific workspaces.

Rule: the experience layer may read Beem APIs and submit commands, but may not call mutating provider clients directly.

### 6.2 Domain layer

Owns Beem meaning:

- Account;

- OperatorFingerprint;

- AccountPlan;

- Objective;

- Plan;

- ForecastDefinition;

- ForecastVersion;

- Scenario;

- Assumption;

- MetricSeries;

- ActualObservation;

- Variance;

- ForecastRun;

- ForecastDecisionLink;

- Signal;

- Opportunity;

- Offer;

- Campaign;

- Lead;

- Contact;

- ConsentState;

- Proposal;

- Quote;

- BookingProjection;

- PaymentProjection;

- RevenueObservation;

- WorkPacket;

- WorkflowNode;

- RecipeDefinition;

- RecipeVersion;

- RecipeRun;

- OpportunityHorizon;

- WorkspaceManifest;

- CapabilityDefinition;

- Connection;

- ExternalAccountBinding;

- PolicyDecision;

- AuthorityResolution;

- ExactOperationBinding;

- ExecutionAttempt;

- ProviderReceipt;

- Observation;

- ReconciliationCase;

- Verification;

- ReEntryRecord;

- AutomationDefinition;

- AutomationRun;

- HumanHandoff;

- RouteLog.

Rule: provider-specific objects are mapped into these Beem-owned contracts rather than leaking provider semantics into the core.

### 6.3 Orchestration layer

Owns AccountAgent state, Objective Manager, Planner, Plan versioning, Opportunity Horizons, WorkGraph, durable workflows, schedules/timers, event subscriptions, human tasks, specialist coordination, retries, compensation, pause/resume/cancel/kill, outcome monitoring, replanning and conversation assertion freshness.

Rule: orchestration coordinates work. It does not create permission.

### 6.4 BLCP layer

Owns State Registry, qualification, Information Authority Binding, freshness/conflict detection, Minimum Hydration Resolver, policy, authority, consequence classification, approval evidence, Exact Operation Binder, capability eligibility, grant expiry/revocation, receipts, observations, reconciliation, verification, re-entry and replay-safe RouteLog.

Rule: no material consequence bypasses BLCP.

### 6.5 Capability layer

Owns capability registry, acquisition intelligence, CRM read/write, content mutation, communications, search/media, payments, quote/booking, mobility/fulfilment, documents/artifacts, human/manual bridges and future external add-ons.

Marketing execution is explicitly first-class across web, organic search/SEO/AI search, paid search, paid social, organic social, email, written content, visual creative/art, CRM and measurement; provider-specific implementations sit behind typed capability contracts.

Rule: capability registration means technically available, not authorised.

### 6.6 Evidence layer

Owns canonical event envelope, outbox/inbox, RouteLog, receipts, observations, discrepancies, reconciliation evidence, verification, replay, audit projections and evidence export.

### 6.7 Infrastructure layer

Owns tenant/environment isolation, identity, service accounts, databases, queues, object storage, secrets, deployment, observability, backups, disaster recovery, cost metering and feature flags.

## 7. Reference runtime flows

Material-action route:

source state -> qualification -> minimum hydration -> objective/request -> candidate plan/work -> policy -> authority -> exact operation binding -> capability -> execution attempt -> receipt -> independent observation -> reconciliation -> re-entry -> plan/forecast update

Adaptive route:

Account -> OperatorFingerprint -> Recipe selection -> Requirement Compiler -> Hydration -> Opportunity Horizons -> candidate Plan -> WorkGraph -> BLCP -> capabilities -> observations -> Recipe/Workspace recompile

## 8. Repository topology

text

/

  apps/

    web/

    api/

    worker/

    operator/

  packages/

    domain/

      account/

      planning/

      forecasting/

      crm/

      revenue/

      work/

      recipes/

      workspace/

      capabilities/

      evidence/

    control/

      state-registry/

      hydration/

      policy/

      authority/

      consequence/

      operation-binding/

      reconciliation/

      re-entry/

    orchestration/

      account-agent/

      planner/

      horizon-engine/

      workgraph/

      workflow-runtime/

      scheduler/

      automation/

      handoffs/

      recovery/

    capabilities/

      registry/

      acquisition-intelligence/

      crm/

      content/

      communications/

      search/

      media/

      payments/

      booking/

      mobility/

      provider-bridge/

      manual/

    evidence/

      events/

      outbox/

      inbox/

      route-log/

      receipts/

      observations/

      replay/

    identity/

    database/

    ui/

    test-fixtures/

    observability/

  docs/

    adr/

    api/

    runbooks/

  scripts/

    migrations/

    evidence/

    local-dev/

  BEEM_FULL_PRODUCT_CANON_v1_0.md

  BEEM_FULL_BUILD_SPECIFICATION_v1_0.md

This is a target ownership model, not an instruction to perform a big-bang folder move.

## 9. Module ownership contract

Every module defines purpose, owned data, public interfaces, events emitted, events consumed, dependencies, forbidden dependencies, maturity state, tests, operational owner, failure behaviour and rollback path.

Forbidden dependencies include:

- UI -> provider SDK directly;

- model client -> database mutation directly;

- connector -> policy database directly;

- AccountAgent -> privileged provider credential directly;

- recipe -> raw customer secret;

- replay -> live capability execution;

- CRM projection -> payment truth overwrite;

- workspace -> authority inference.

---

# PART III — DOMAIN AND DATA CONTRACTS

## 10. Account

Minimum fields:

- account_id

- tenant_id

- legal_entity_ref

- display_name

- status

- timezone

- primary_currency

- locations

- memberships

- service_identities

- connected_sources

- current_plan_id

- active_objective_ids

- active_recipe_run_ids

- state_version

- created_at

- updated_at

Invariants: tenant-bound; conflict-detectable versioning; no material truth solely in conversation; explicit retention/deletion status; cross-tenant references rejected.

## 11. OperatorFingerprint

A derived stable-but-revisable projection used for recipe selection.

Fields: fingerprint_id, account_id, version, compiled_at, source_state_fingerprint, services, locations, capacity_classes, connected_capability_classes, commercial_constraints, operating_constraints, evidence_refs, known_unknowns and freshness_summary.

Rules: derived not authoritative; refreshed on relevant source change; never carries transferable authority.

## 12. AccountPlan

Fields: plan_id, account_id, version, status, predecessor_plan_id, objective_ids, priority, horizon, markets, offers, audiences, channel_allocations, approved_claim_refs, proof_gap_refs, budget_envelopes, capacity_assumptions, forecast_refs, active_initiatives, recipe_run_refs, workgraph_refs, risks, review_at, success_measures and decision_record_ref.

Rules: immutable after activation; supersession creates new version; plan is never permission; affected work is re-evaluated when material assumptions change.

## 13. Objective

Fields: objective_id, account_id, owner_principal_id, statement, metric_definition_refs, baseline_ref, target_state, horizon, priority, constraints, budget_envelope_ref, authority_boundary_ref, status, created_at and closed_at.

## 14. Forecasting objects

### ForecastDefinition

Metric set, horizon, cadence, source requirements, scenario rules, uncertainty representation, observation sources and comparison method.

### ForecastVersion

ID, definition version, account, generated_at, source-state fingerprint, assumptions, scenario refs, metric series, uncertainty, provenance, status and superseded_by.

### Scenario

ID, label, assumption deltas, capacity/budget constraints, expected metric series, uncertainty and linked candidate interventions.

### ActualObservation

Metric, source, observed value, observed_at, source version, qualification status and evidence ref.

### Variance

Forecast version, actual refs, absolute/relative variance, explanatory candidates, attribution status and next-action links.

Rules: forecast never writes actuals; actuals only from registered observation sources; explanations remain candidate; attribution may be UNKNOWN or PARTIAL; intervention-generated state cannot self-confirm success.

## 15. Sell-through objects

Signal, Opportunity, Offer, Campaign, Outreach, Lead, QualifiedOpportunity, Proposal, Quote, BookingProjection, FulfilmentHandoff, PaymentProjection, RevenueObservation and AttributionRecord.

Each object has canonical Beem ID, external IDs if any, source binding, status vocabulary, version, occurred/observed times, evidence, allowed transitions and reconciliation state.

## 16. Contact and consent

Contact separates identity from contactability.

Fields: contact ID, source identity refs, entity-match state, communication channels, consent state, suppression state, purpose, observed_at, source and conflict state.

Record presence does not imply permitted contact.

## 17. WorkPacket

### Intent

work_packet_id, account, objective, reason, desired outcome, accountable owner.

### Qualified state

evidence refs, state fingerprint, freshness, missing state, stale state, conflicts, qualification result.

### Candidate

plan ref, artifact/payload ref, provenance, candidate version, rationale.

### Consequence

class, reversibility, affected objects, target, timing, risk.

### Policy and authority

policy result, authority requirement, eligible approvers, approval evidence, grant/denial/hold, expiry, revocation.

### Exact operation

capability ID/version, target binding, action, payload digest, amount/budget/quantity, idempotency, preconditions, recovery.

### Execution

attempt ID, dispatch state, provider request ID, receipt ref, possible-write state.

### Outcome

observation refs, discrepancy, reconciliation, verification, commercial refs, re-entry, follow-up.

## 18. RecipeDefinition and RecipeVersion

RecipeDefinition: identity, purpose, owner, visibility, licensing state, objective classes, fingerprint conditions and current published version.

RecipeVersion: immutable version, required/optional/prohibited state, freshness, capabilities, workflow graph, branching, missing-state actions, approval rules, consequence classes, workspace template, allowed UI components, cost budget, measurement plan, re-entry rules, expiry/review.

Rules: material RecipeRun pins version; update creates new version; no customer data; no inherited authority.

## 19. RecipeRun

Fields: recipe_run_id, account, recipe version, objective, fingerprint version, hydration fingerprint, selected horizons, workgraph, workspace manifest, authority refs, started_at, state, paused_at, completed_at and outcome refs.

## 20. OpportunityHorizon

Fields: horizon ID, account/objective, source evidence, description, requirements, missing state, expected effects, constraints, estimated cost, risk, reversibility, confidence, selection status and rejection/hold reason.

Rules: horizons may coexist; rejection requires reason; model ranking advisory only; plan selection is not execution authority.

## 21. WorkspaceManifest

Fields: manifest ID, account, objective/recipe run, version, navigation, component instances, component config, data queries, required permissions, action capabilities, read/write distinctions, evidence drawers, feature flags, source fingerprint and generated_at.

Rules: configuration not arbitrary executable code; allow-listed components only; consequential action still requires WorkPacket + BLCP; stale manifest cannot bypass fresh checks.

---

# PART IV — INFORMATION AUTHORITY, STATE AND HYDRATION

## 22. Information Authority Binding

Each binding records truth class, object/field, authoritative source, fallback, precedence, freshness, permitted use, conflict rule, tombstone rule, merge/unmerge rule and observation route.

Example truth classes: account identity, contactability, consent, quote status, booking status, payment status, fulfilment status, capacity, deployed web state, campaign state and revenue observation.

A model never resolves source conflict by fluency.

## 23. Entity resolution

Implement external ID map, deterministic candidates, probabilistic match score where needed, human resolution, merge evidence, unmerge evidence, tombstones and conflict preservation.

No irreversible merge solely on model confidence.

## 24. State qualification

QualificationResult includes source refs, status, intended use, receiver, freshness, conflicts, exclusions, required remediation and evidence refs.

Status vocabulary:

- AVAILABLE

- ADMITTED

- ROUTE_RELEVANT

- MISSING

- STALE

- CONFLICTED

- UNAUTHORISED

- ESTIMATED

## 25. Minimum Hydration Resolver

Inputs: account, objective/work, receiver, consequence class, capability, purpose, source map and privacy/policy restrictions.

Output: admitted state, excluded state with reasons, missing-state requests, freshness requirements, unresolved conflicts and hydration fingerprint.

Algorithm:

- determine route requirements;

- resolve authoritative source classes;

- filter by purpose/tenant;

- apply privacy/consent;

- validate freshness;

- surface conflicts;

- compute missing state;

- include minimum sufficient route-relevant state;

- emit reproducible fingerprint;

- never replace mandatory missing state with invented defaults.

## 26. Freshness and concurrency

Every material truth class defines observed_at, valid_from, valid_to, source_version, stale_after, refresh strategy, object version/ETag and material-change invalidation.

Long-running work re-resolves before consequence when freshness expires or target, payload, amount, provider, policy, state or authority changes.

---

# PART V — BEEM LOCAL CONTROL PLANE

## 27. BLCP services

State Registry; Hydration; Policy; Authority; Consequence; Operation Binding; Capability Eligibility; Grant; Receipt; Observation; Reconciliation; Re-entry.

They may initially share a deployable service, but contracts stay separate.

## 28. BLCP state machine

States:

- DRAFT

- HYDRATING

- MISSING_STATE

- QUALIFIED

- AWAITING_APPROVAL

- DENIED

- HELD

- PERMITTED

- COMMITTED

- DISPATCHING

- DISPATCHED

- ACKNOWLEDGED

- POSSIBLE_WRITE

- OBSERVING

- RECONCILING

- VERIFIED

- UNKNOWN

- FAILED

- COMPENSATING

- COMPLETED

- CANCELLED

- EXPIRED

Key rules:

- DRAFT -> HYDRATING starts the route.

- HYDRATING -> MISSING_STATE if mandatory state absent.

- HYDRATING -> QUALIFIED when sufficient state admitted.

- QUALIFIED -> AWAITING_APPROVAL where needed.

- QUALIFIED -> PERMITTED only when active authority already exists.

- AWAITING_APPROVAL -> PERMITTED only for exact approved scope.

- PERMITTED -> COMMITTED after exact binding persisted.

- COMMITTED -> DISPATCHING under idempotency key.

- DISPATCHING -> DISPATCHED on transmission.

- DISPATCHED -> ACKNOWLEDGED on provider receipt.

- DISPATCHED/ACKNOWLEDGED -> POSSIBLE_WRITE on ambiguous timeout.

- ACKNOWLEDGED -> OBSERVING when acknowledgement is not outcome.

- POSSIBLE_WRITE -> OBSERVING without blind retry.

- OBSERVING -> RECONCILING after observation.

- RECONCILING -> VERIFIED, UNKNOWN or FAILED.

- FAILED -> COMPENSATING only under separately governed compensating operation.

- VERIFIED/FAILED/UNKNOWN -> COMPLETED only after re-entry/closure semantics.

## 29. Policy contract

PolicyResult: policy version, account, operation class, consequence class, status PASS/CONDITIONAL/BLOCK/HOLD, conditions, evidence, approvals, limits, expiry and reasons.

Model output cannot be the sole policy engine.

## 30. Authority contract

AuthorityResolution: principal, tenant/account, operation class, target class, limits, purpose, amount/budget, effective/expiry, approval evidence, delegation chain, revocation, separation-of-duties result and status.

Access token scope is not sufficient authority evidence.

## 31. ExactOperationBinding

Binding ID, WorkPacket, principal, account/tenant, capability, target, action, objects, payload digest, amount/budget/quantity, source-state fingerprint, policy version, authority resolution, approval refs, capability version, idempotency key, expiry, recovery class and correlation/causation IDs.

Any material change requires re-resolution.

## 32. Consequence classes

- C0 READ_ONLY

- C1 INTERNAL_STATE

- C2 REVERSIBLE_EXTERNAL_WRITE

- C3 CUSTOMER_VISIBLE_COMMUNICATION

- C4 COMMERCIAL_COMMITMENT

- C5 SPEND_OR_PAYMENT

- C6 BOOKING_OR_FULFILMENT

- C7 DATA_DISCLOSURE

- C8 HIGH_IMPACT_IRREVERSIBLE

Each defines minimum identity, state, policy, authority, approval, reversibility, observation, retry, compensation, retention and audit requirements.

## 33. Typed runtime outcomes

READY, READY_WITH_CONDITIONS, STAGE, REQUEST_STATE, HOLD, RECOMPUTE, ESCALATE, STOP, UNKNOWN and COMPLETED.

Never collapse these into a Boolean.

---

# PART VI — CAPABILITIES AND CONNECTORS

## 34. CapabilityDefinition

Fields: capability ID/version, owner, environment, supported operations, read/propose/execute class, schemas, consequence class, credential class, scopes, required state, authority requirements, idempotency, receipt semantics, observation method, rate limits, cost, health, suspension and support owner.

## 35. Connection

Fields: connection ID, account, provider class, environment, credential reference, installed capabilities, scopes, source-authority classes, health, freshness, sync cursor, webhook refs, last read/write, last receipt, last observation, suspended_at and support status.

## 36. Capability eligibility

Check connection, environment, tenant/account, credential, operation support, target, health, rate/cost limits, purpose and then BLCP authority.

Eligibility is necessary, never sufficient.

## 37. Manual capability bridge

Where an external API is unavailable:

- create exact provider task;

- include versioned payload/artifact;

- assign authorised operator;

- record handoff;

- capture acknowledgement;

- capture completion evidence;

- observe external/business state;

- reconcile;

- re-enter.

Manual and automated capabilities use the same WorkPacket/evidence contracts.

## 37A. First-class marketing execution capability families

Beem must register and route the following as first-class capability families. A provider connector may implement one or many families; registration means technically available, not authorised:

- web / website: site, page and content reads; candidate changes; exact publishing/mutation operations; live-site observation;

- organic search / SEO / AI search: query/page visibility, technical and structured-data evidence, candidate interventions and post-change observation;

- paid search: campaign, ad-group, keyword/query, audience, creative and landing-page operations; create/update/pause; bid/budget management; conversion and spend observation;

- paid social: campaign/ad-set/audience/creative operations; create/update/pause; bid/budget management; platform performance and spend observation;

- organic social: content planning, creation, approval, scheduling/publishing, engagement observation and commercial re-entry;

- email: composition, templates, segments, sequences, sending, replies, bounce/unsubscribe/suppression state, campaign measurement and CRM re-entry;

- written content: versioned copy creation for web pages, articles, landing pages, emails, ads and social posts;

- visual creative/art: versioned image/art/creative generation or editing, asset management, approval/brand/rights metadata and campaign attachment;

- CRM: audience/contact/consent state, activities, leads/opportunities and governed write-back under source-authority rules;

- measurement: channel observations, spend/cost, conversions, attribution candidates, pipeline/bookings/orders, revenue actuals and re-entry.

### Required operation vocabulary

At minimum, the Capability Registry must be able to represent these provider-neutral operation classes, with provider-specific mappings behind the connector boundary:

- web: web.page.read, web.content.propose, web.publish, web.observe;

- organic/AI search: search.organic.observe, search.ai.observe, search.intervention.propose, structured_data.propose;

- paid search: paid_search.campaign.create, paid_search.campaign.update, paid_search.campaign.pause, paid_search.bid.set, paid_search.budget.set, paid_search.creative.attach, paid_search.landing_page.bind, paid_search.observe;

- paid social: paid_social.campaign.create, paid_social.campaign.update, paid_social.campaign.pause, paid_social.audience.manage, paid_social.creative.attach, paid_social.bid.set, paid_social.budget.set, paid_social.observe;

- organic social: social.post.create, social.post.schedule, social.post.publish, social.engagement.observe;

- email: email.compose, email.sequence.create, email.sequence.update, email.sequence.pause, email.send, email.reply.observe, email.bounce.observe, email.suppression.read, email.unsubscribe.observe, email.campaign.observe;

- written content: content.copy.create, content.copy.version, content.copy.approve;

- visual creative/art: creative.visual.create, creative.visual.version, creative.visual.approve, creative.asset.manage, creative.asset.attach;

- CRM: crm.segment.read, crm.contact.read, crm.consent.read, crm.activity.create and source-authority-governed lead/opportunity write operations;

- measurement: campaign.observe, spend.observe, conversion.observe, attribution.propose, pipeline.observe, revenue.observe.

Candidate-generation operations produce candidate artifacts unless and until an external mutation is separately bound. Any publish, send, spend, bid/budget change, customer-visible mutation or external CRM write is a distinct material operation. It requires WorkPacket, current admitted state, policy/authority/approval as required by consequence class, exact target/payload/budget binding, capability eligibility, idempotency/recovery semantics, receipt, independent observation, reconciliation and re-entry. Email/communications additionally enforce consent and suppression. Visual assets retain provenance, rights/licence status and brand/approval metadata. Channel acknowledgements and model estimates never become commercial actuals by themselves.

The Account Manager may coordinate one campaign across these families, but each channel operation resolves independently under the existing typed runtime outcomes, including READY, READY_WITH_CONDITIONS, STAGE, REQUEST_STATE, HOLD, RECOMPUTE, ESCALATE or STOP. One blocked channel does not create permission for another.

---

# PART VII — ACQUISITION INTELLIGENCE

## 38. Acquisition-intelligence module

Responsibilities:

- website/source inventory;

- structured data;

- search visibility;

- AI-search visibility;

- claim/proof analysis;

- first-party telemetry;

- competitor/category movement;

- diagnostics;

- appraisals;

- opportunity creation;

- content/page candidates;

- post-change observation.

Outputs: EvidenceItem, Finding, CandidateIntervention, ForecastInput and OpportunityHorizon candidates.

Acquisition intelligence owns specialist evidence, diagnosis and candidate interventions. It may feed or consume admitted cross-channel observations, but it does not own paid-search, paid-social, organic-social, email, content/creative or CRM side effects; those execute only through the registered capability families and BLCP route defined in Part VI.

Prohibited: direct publish without WorkPacket/BLCP; direct spend mutation; direct CRM truth overwrite; score/confidence as authority; impact claims from telemetry alone.

## 39. Acquisition data adaptation

Map legacy acquisition data into Account, Site, Page, Signal, Claim, Proof, Finding, Opportunity and EvidenceItem with source, source version, observed_at, classification, confidence, freshness, account/tenant and migration provenance.

---

# PART VIII — CRM, REVENUE AND SELL-THROUGH

## 40. CRM minimum

Implement Account relationship view, Contact, ConsentState, Lead, Opportunity, Activity, Proposal, Quote, BookingProjection, PaymentProjection and RevenueObservation.

Required services: entity resolution, external-ID mapping, dedupe, timeline, tasks, follow-up SLAs, consent/suppression, write-back, reconciliation and attribution.

## 41. Sell-through state machine

Stages:

- SIGNAL

- OPPORTUNITY

- OFFER_DEFINED

- CAMPAIGN_OR_OUTREACH

- LEAD

- QUALIFIED_OPPORTUNITY

- PROPOSAL

- QUOTE

- BOOKING_OR_ORDER

- FULFILMENT_HANDOFF

- PAYMENT_OBSERVED

- REVENUE_OBSERVED

- ATTRIBUTED

- CLOSED_WON

- CLOSED_LOST

- UNKNOWN

Every transition stores source event, actor, timestamp, evidence, truth owner, reason, WorkPacket and forecast/plan link.

## 42. Attribution

Statuses: UNATTRIBUTED, CANDIDATE, PARTIAL, MULTI_TOUCH, VERIFIED_DIRECT and UNKNOWN.

Candidate attribution never rewrites external truth.

---

# PART IX — FORECASTING

## 43. Forecast engine

Support baseline construction, scenarios, capacity constraints, budget constraints, expected pipeline, bookings/orders, revenue, uncertainty, actual ingestion, variance, refresh and decision links.

## 44. Forecast reproducibility

ForecastRun stores source versions, definition version, recipe version where applicable, assumptions, model/tool version, random seed where relevant, generated_at, code version and outputs.

## 45. Anti-self-confirmation

The following are not actuals: Beem recommendation, Beem forecast, Beem execution request, provider acknowledgement or Beem UI state.

Actuals require registered observation sources.

---

# PART X — ADAPTIVE RECIPE RUNTIME

## 46. Recipe Library

Functions: create draft, validate, version, review, publish, deprecate, suspend, compare, search by objective/fingerprint, export state-independent definition and validated import.

Visibility: PRIVATE, ORGANISATION, CSR_CURATED and MARKETPLACE_READY.

Public marketplace behaviour is deferred; data model support is allowed.

## 47. Requirement Compiler

Input: objective, OperatorFingerprint, recipe version and capability registry.

Output: required truth classes, optional truth classes, freshness constraints, capability classes, potential horizons, blockers, workspace requirements and estimated cost envelope.

## 48. Opportunity Horizon engine

Generate candidates from admitted state, preserve multiplicity, attach evidence/missing state, estimate cost/effort, attach reversibility, rank advisory only, allow human selection, allow concurrency, retire with reason and reopen on state change.

## 49. Recipe compilation

- select recipe version;

- resolve OperatorFingerprint;

- compile requirements;

- hydrate state;

- generate viable horizons;

- resolve blockers;

- create candidate Plan;

- build WorkGraph;

- compile WorkspaceManifest;

- persist RecipeRun;

- create required WorkPackets;

- start only state-ready nodes.

## 50. Recipe re-entry

On outcome: write observation; reconcile; update Account; refresh actuals; recompute variance; update objective progress; test current branch fit; create Plan version if needed; recompile workspace if relevant.

---

# PART XI — WORKSPACE COMPILER AND UX

## 51. Approved component registry

Initial components:

- AccountPulse

- KPIGrid

- ForecastPanel

- VariancePanel

- Map

- CapacityGrid

- Calendar

- Timeline

- Kanban

- Pipeline

- QuoteBuilder

- InventorySelector

- ReadinessMatrix

- CommandBoard

- Itinerary

- PricingEditor

- ApprovalInbox

- LeadQueue

- ProviderMap

- ComplianceChecklist

- DemandHeatmap

- CommunicationsCentre

- PaymentStatus

- ExceptionQueue

- EvidenceDrawer

- WorkQueue

- ConnectionHealth

- ObjectiveProgress

Each declares read models, allowed actions, required permissions, consequential actions, evidence links, empty/error states and accessibility.

## 52. Workspace compilation rules

Allow-listed components only; no arbitrary code generation; no direct provider calls; all actions map to Beem APIs; consequential action creates/updates WorkPacket; read model shows freshness; unknown/conflict visible; component version stored.

## 53. Stable navigation

Home; Account Manager; Plan; Forecast; Pipeline; Work; Acquisition; Connections; Evidence; Settings.

Compiled workspaces live within this shell.

---

# PART XII — ACCOUNT MANAGER AND ORCHESTRATION

## 54. AccountAgent state

Persist account, objectives, current plans, open WorkPackets, open questions, missing-state requests, horizons, RecipeRuns, waits, handoffs, exceptions, recent material assertions, conversation provenance, last hydration fingerprint and last replan time.

Conversation text is not the truth store.

## 55. Account Manager actions

Permitted: explain, ask, plan, compare, create candidate, create WorkPacket, create/assign task, request approval, request state, select capability candidate, schedule permitted work, pause, resume, cancel, replan, reconcile and summarise evidence.

No direct grant creation.

## 56. Planner output

State fingerprint, objective, assumptions, missing state, horizons considered, selected work, dependencies, expected effect, cost, risk, capability class, authority class and observation route.

## 57. WorkGraph node types

OBSERVE, ANALYSE, REQUEST_STATE, GENERATE_CANDIDATE, HUMAN_TASK, REQUEST_APPROVAL, REQUEST_EXECUTION, WAIT_TIME, WAIT_EVENT, VERIFY, RECONCILE, NOTIFY and REPLAN.

Node fields: ID, type, dependencies, inputs, outputs, state, owner, deadline, retry class, cost budget, capability class, WorkPacket, wait condition and cancellation semantics.

## 58. Durable workflow states

DRAFT, PLANNING, WAITING_FOR_STATE, WAITING_FOR_EVENT, WAITING_FOR_APPROVAL, READY, EXECUTING, VERIFYING, RECONCILING, REPLANNING, PAUSED, BLOCKED, FAILED, UNKNOWN, COMPLETED and CANCELLED.

Worker restart must not duplicate side effects.

## 59. AutomationDefinition

Trigger, evidence requirements, objective scope, operation scope, targets, capabilities, consequence classes, spend/amount limits, authority refs, approvals, effective period, expiry, retry budget, notifications, suspension and verification.

Activation permits only the declared envelope.

---

# PART XIII — EVENTS, RECEIPTS AND REPLAY

## 60. Canonical event envelope

event_id, event_type, event_version, tenant_id, account_id, source, subject_type, subject_id, occurred_at, received_at, correlation_id, causation_id, idempotency_key, payload_ref, payload_hash, classification, provenance and replay_policy.

## 61. Outbox/inbox

Use transactional outbox when state mutation and event publication must be atomic.

Inbox records provider event ID, signature verification, first seen, duplicate count, processing status and resulting transition.

## 62. ProviderReceipt

attempt ID, provider request ID, provider timestamp, acknowledgement class, raw response reference, response hash, possible-write flag and status.

Receipt never automatically equals outcome.

## 63. Observation

observation ID, source, object, value/state, observed_at, source version, confidence if inferred, independent-from-attempt flag and evidence ref.

## 64. Reconciliation

Compare bound operation, attempted payload, receipt, current external state and business observation.

Outcomes: MATCH, PARTIAL_MATCH, MISMATCH, NOT_FOUND, DUPLICATE, POSSIBLE_WRITE, UNKNOWN and FAILED.

## 65. Replay

Reconstruct qualification, hydration, policy, authority, binding, attempts, receipts and observations. Never call live provider. Flag missing inputs and non-deterministic steps.

---

# PART XIV — IDENTITY, SECURITY, PRIVACY

## 66. Principal types

HUMAN_USER, CSR_OPERATOR, SERVICE_IDENTITY, WORKFLOW_WORKER, CONNECTOR_IDENTITY and READ_ONLY_AUDITOR.

## 67. Roles

Initial roles may include Account Owner, Account Administrator, Account Manager, Commercial Operator, Approver, Analyst, Viewer, CSR Support and CSR Operations.

Role is not exact consequence authority.

## 68. Delegation

Grantor, grantee, account, operation class, target class, amount/budget, consequence class, effective/expiry, revocation and separation-of-duties conditions.

## 69. Tenant isolation

Tenant ID on every material object; row/service isolation; scoped object storage; tenant-aware caches, queues and search indexes; tenant-aware logs; deliberate cross-tenant attack tests.

## 70. Secrets

Secret references only; no secrets in logs, prompts or RouteLog; environment-specific identity; rotation; disable legacy credentials; secret scanning in CI.

## 71. Privacy

Data inventory, purpose, classification, consent, suppression, retention, export, deletion, hold where required, minimisation and access audit.

Evidence prefers references/hashes over raw personal data where possible.

## 72. Environments

Local, test, staging and production remain separate. Production credential cannot work in local/test. Wrong-environment binding fails closed.

---

# PART XV — ERROR, RETRY, COMPENSATION

## 73. Error taxonomy

VALIDATION_ERROR, MISSING_STATE, STALE_STATE, CONFLICTED_STATE, POLICY_BLOCK, AUTHORITY_INVALID, APPROVAL_REQUIRED, CAPABILITY_UNSUPPORTED, CAPABILITY_UNAVAILABLE, RATE_LIMITED, TRANSIENT_PROVIDER, TIMEOUT_BEFORE_WRITE, TIMEOUT_POSSIBLE_WRITE, PERMANENT_PROVIDER, OBSERVATION_MISMATCH, RECONCILIATION_UNKNOWN, INTERNAL_INVARIANT, TENANT_VIOLATION and PRIVACY_BLOCK.

## 74. Retry rules

Retry requires retryable class, idempotency, unchanged material payload, unchanged authority, valid expiry, fresh-enough state, retry budget and provider policy.

TIMEOUT_POSSIBLE_WRITE cannot blindly retry.

## 75. Compensation

Compensation is a new governed operation: cancellation, refund, revert, correction or restoration. It needs authority and observation.

## 76. Dead-letter

Store original node/event, error class, attempts, state fingerprint, authority status, owner, next review, customer impact and recovery options.

---

# PART XVI — APIs

## 77. API rules

All mutating APIs require tenant, account, authenticated principal/service, correlation ID, idempotency where appropriate, expected object version, purpose and current authority reference where material.

## 78. Account APIs

Create/get account; update qualified metadata; list gaps; get/refresh fingerprint; get pulse.

## 79. Planning APIs

Create/version objective; create/compare/accept/supersede plan; pause/close objective.

## 80. Forecast APIs

Create definition; run forecast; create/compare scenario; ingest actual; compute variance; link decision; supersede forecast.

## 81. Work APIs

Create WorkPacket; register candidate; request hydration; request approval; approve/reject; bind exact operation; request execution; cancel; reconcile; re-enter.

## 82. Recipe APIs

Create draft; validate; version; publish; deprecate; find applicable; compile requirements; start/pause/resume/close RecipeRun; recompile workspace.

## 83. Capability APIs

Register capability; update health; install/suspend connection; discover eligible; execute bound operation; record receipt; ingest observation.

## 84. Orchestration APIs

Create WorkGraph; add node; satisfy dependency; assign; wait; resume; retry; compensate; replan; kill.

## 85. Evidence APIs

Append/query evidence; get route timeline; replay; export; create/close reconciliation case.

---

# PART XVII — OBSERVABILITY AND OPERATIONS

## 86. Telemetry dimensions

Environment, tenant/account where permitted, service/module, operation, correlation, trace, WorkPacket, workflow node, capability, consequence class, error class, latency, retry and cost/usage.

Never log secrets or prohibited payloads.

## 87. Dashboards

API health; queue age; workflow backlog; WorkPackets by state; approval age; missing-state age; capability health; timeout/unknown rate; receipt-to-observation lag; reconciliation backlog; forecast freshness; connector freshness; security alerts; usage cost; deploy errors; migration discrepancies.

## 88. Internal SLOs

Define read API, control decision, WorkPacket transition, queue latency, connector freshness, observation lag, reconciliation lag, workflow recovery and evidence availability targets in ADRs.

## 89. Runbooks

Provider outage; possible-write timeout; reconciliation backlog; stale source; webhook failure; credential compromise; cross-tenant incident; queue backlog; bad deployment; failed migration; forecast-source outage; stuck workflow; expired authority; data deletion; rollback.

---

# PART XVIII — COST AND BUDGET

## 90. Usage ledger

Record usage by account, objective, WorkPacket, RecipeRun, model/tool, capability, connector and storage/compute class.

## 91. Budget controls

Per-run, per-account, model, media/spend and provider ceilings; alert threshold; hard stop; approval-on-threshold.

Retry/decomposition cannot bypass ceilings.

## 92. Cost-aware planning

Cost may inform planning but cannot reduce required state, weaken authority or convert UNKNOWN to success.

---

# PART XIX — LEGACY CODE AND MIGRATION

## 93. Donor-adaptation rule

Classify every legacy component as KEEP, ADAPT, REIMPLEMENT, RETIRE, VERIFY or BLOCK.

Manifest fields: source path, source commit, rights state, actual behaviour, tests, secret/data risk, legacy semantics, destination Beem contract, disposition, Beem tests, migration and rollback.

## 94. Legacy schema disposition

Each table: KEEP AS REFERENCE, MAP TO BEEM, SPLIT, REIMPLEMENT, RETIRE or BLOCK.

Never import a mixed legacy schema wholesale.

## 95. Data migration tooling

Dry run, source counts, destination counts, rejected rows, conflict rows, mapping version, checksums, tenant validation, rollback, resumability and audit receipt.

## 96. Terminology migration

Customer-facing code uses Beem terminology. Legacy terms remain only in immutable provenance, fixtures requiring fidelity or migration adapters.

---

# PART XX — TEST STRATEGY

## 97. Unit tests

Domain invariants, qualification, freshness, source precedence, entity matching, forecast calculations, recipe validation, binding invalidation, permission conditions, idempotency and state machines.

## 98. Contract tests

Every API schema, event schema, capability, connector, receipt, observation, outbox/inbox, workspace action and recipe schema.

## 99. Integration tests

API+database; worker+queue; BLCP+WorkPacket; connector test double; receipt+observation+reconciliation; forecast actual ingestion; workspace action; recipe compile+WorkGraph.

## 100. Tenant isolation tests

Deny cross-tenant API read/write, search, evidence, credentials, workflow replay, model context and object storage.

## 101. Mandatory negative tests

The build is not releasable if it permits:

- consequential action without identity;

- consequential action without purpose;

- consequential action without required state;

- consequential action without policy;

- consequential action without authority;

- reuse of binding after payload change;

- reuse after target change;

- reuse after amount/budget change;

- reuse after policy change;

- model confidence becoming authority;

- acquisition score becoming authority;

- AccountAgent widening permission;

- replay invoking live provider;

- duplicate event causing duplicate consequence;

- timeout becoming verified success;

- acknowledgement becoming business outcome;

- CRM projection overwriting contrary external truth;

- customer data entering reusable recipe;

- tenant A hydrating tenant B;

- stale conversation overriding current state;

- paused automation continuing;

- revoked delegation continuing;

- unsupported capability presented as supported;

- provider outage causing unsafe write fallback;

- failed observation treated as success;

- recipe update mutating active run;

- workspace action bypassing WorkPacket;

- UI direct provider write;

- secret entering logs or model prompt;

- possible-write retry causing duplicate consequence.

## 102. Golden tests

### Forecast-to-revenue

Qualified state -> forecast -> variance -> opportunity -> candidate -> WorkPacket -> approval/binding -> execution -> receipt -> observation -> reconciliation -> revenue actual -> forecast/Plan update -> replay.

### Recipe compilation

Same RecipeVersion across two Accounts -> different fingerprints/hydration/horizons/workspaces -> no code fork -> no state leakage.

### Possible-write timeout

Dispatch -> timeout -> POSSIBLE_WRITE -> no blind retry -> observe -> reconcile.

### Authority revocation

Permit -> revoke before dispatch -> dispatch blocked -> re-resolve.

### Worker restart

Durable wait -> worker dies -> restart -> no duplicate consequence -> resume.

### Cross-channel marketing execution

One Objective -> channel plan across web + SEO/AI search + paid search + paid social + organic social + email + written content + visual creative/art + CRM + measurement -> separate WorkPackets/bindings -> mixed READY/HOLD -> publish/send/spend cannot bypass BLCP -> receipts -> reply/bounce/suppression/spend/conversion/channel observations -> reconciliation -> CRM/pipeline/revenue re-entry -> replay produces no external side effect.

---

# PART XXI — CI/CD AND RELEASE

## 103. Pull-request checks

Format, lint, typecheck, unit, contract, migration validation, schema diff, secret scan, dependency scan, rights/notice check where applicable, tenant suite, negative-path subset, build and ownership review.

## 104. Branching

Main releasable; short-lived features; risky migrations isolated; donor-fidelity and Beem adaptation separated where practical; release tags identify deployed code.

## 105. Database migrations

Forward-compatible where possible; expand/contract; no destructive change without rollback/backup; background backfill; migration receipt; tenant counts; post-verification.

## 106. Feature flags

For incomplete consequential capabilities, new connector writes, recipe features, autonomy, forecast models and workspace components.

Flag never bypasses BLCP.

## 107. Release gate

Named commit, environment, migration version, config/policy versions, known issues, rollback, evidence and owner sign-off.

---

# PART XXII — SPRINT DELIVERY PROGRAMME

Sprints are evidence-gated increments. Nominal duration may be one to two weeks depending on team size, but a sprint does not exit until its acceptance evidence exists.

## Sprint 0 — repository baseline, reproducibility and safety

### Objective

Create a trustworthy development base.

### Work

Freeze branch/head; inventory apps/packages; runtime/package-manager lock; reproduce install/build/tests; environment-variable inventory; secret classification; disable unknown side effects; feature flags; donor manifest; schema inventory; ADR directory; CI; test database strategy; environment model; evidence/runbook conventions.

### Deliverables

Reproducible local build, CI, donor manifest, environment schema, architecture map, blockers and baseline test report.

### Acceptance

Clean clone installs/builds/tests; no unknown live call; secrets externalised; unresolved failures documented.

### Not done if

Build depends on local uncommitted files, production credential is required locally or an unknown deploy hook remains active.

## Sprint 1 — tenancy, identity and Account core

### Work

Account, tenant, membership, service identity, authenticated context, tenant middleware, Account CRUD, state version, Account Pulse read model, audit events.

### Tests

Cross-tenant denial, wrong account, service scope, version conflict, audit correlation.

### Demo

Two tenants; neither can access the other.

## Sprint 2 — State Registry, provenance and Information Authority Binding

### Work

SourceDefinition, EvidenceItem, state status, InformationAuthorityBinding, external ID map, freshness, conflicts, tombstones, precedence, source/version fingerprints, entity-resolution queue.

### Demo

One field with conflicting sources remains visibly unresolved.

## Sprint 3 — Minimum Hydration Resolver

### Work

Requirement schema, hydration request/resolver, privacy/purpose filter, freshness/conflict checks, missing-state request, exclusion reasons, hydration fingerprint and safe cache.

### Demo

Same Account hydrates differently for diagnosis versus material write.

## Sprint 4 — WorkPacket and event/evidence spine

### Work

WorkPacket schema, candidate version, consequence class, correlation/causation, event envelope, outbox/inbox, RouteLog, evidence query and replay skeleton.

### Demo

Candidate WorkPacket replayed without execution.

## Sprint 5 — policy, authority and exact-operation binding

### Work

PolicyResult, AuthorityResolution, delegation, approvals, consequence classes, ExactOperationBinding, expiry, revocation and invalidation.

### Demo

Approved operation becomes invalid when payload changes.

## Sprint 6 — capability registry and controlled execution

### Work

CapabilityDefinition, Connection, target binding, eligibility, health, suspension, idempotency, execution adapter, test double, manual bridge and receipt.

### Demo

One bound test operation plus one manual capability route.

## Sprint 7 — observation, reconciliation and re-entry

### Work

Observation, ReconciliationCase, Verification, ReEntryRecord, possible-write handling, polling/webhook observation, discrepancy queue and closure rules.

### Demo

Acknowledgement says success but observation differs; discrepancy preserved.

## Sprint 8 — CRM, consent and sell-through core

### Work

Contact, ConsentState, Lead, Opportunity, Activity, Proposal, Quote, booking/payment projections, RevenueObservation, pipeline read model, timeline, follow-up, dedupe and suppression.

### Demo

Lead -> opportunity -> quote with evidence and consent.

## Sprint 9 — forecasting and actuals

### Work

ForecastDefinition, ForecastVersion, Scenario, Assumption, MetricSeries, ForecastRun, ActualObservation, Variance, ForecastDecisionLink and forecast UI.

### Demo

Two scenarios, actual ingestion, variance and linked candidate action.

## Sprint 10 — acquisition intelligence integration

### Work

Site/source mapping, evidence ingestion, findings, diagnostics, opportunity creation, content/page candidate, live observation, commercial link and direct-write bypass prevention.

### Demo

Observation -> opportunity -> candidate -> bound change -> observation -> commercial follow-up.

## Sprint 10A — first-class marketing execution capability pack

### Work

Implement provider-neutral capability definitions, schemas, WorkPacket/UI mappings and sandbox or rights-cleared connector adapters for every family in 37A. Production enablement may be staged by provider/account, but no family may be omitted from the canonical contract. Unsupported operations surface a typed unsupported/unverified state or ManualCapabilityBridge; they are never simulated as success. Consequential connectors remain feature-flagged until their gates pass.

### Tests

Contract/schema, tenant/account binding, auth/scope, purpose/data class, exact target/payload, consent/suppression, spend/bid/budget limits, idempotency, duplicate/timeout possible-write, receipt/observation/reconciliation, rights/provenance/brand metadata for creative, and cross-channel independence.

### Demo

One approved growth objective compiles web + SEO/AI search + paid search + paid social + organic social + email + written content + visual creative/art + CRM + measurement work into separate WorkPackets/bindings; permitted sandbox operations execute, at least one operation holds, receipts/observations re-enter CRM/commercial state, and no held operation leaks through another channel.

## Sprint 11 — AccountPlan, Objective and Account Manager Phase One

### Work

Objective, AccountPlan, Plan versioning, AccountAgent, Account Manager surface, current context, open work, missing-state requests, approvals, explanations and Plan/Work views.

### Demo

Customer gives objective; Account Manager explains state and creates governed work.

## Sprint 12 — forecast-to-revenue reference loop

### Work

Connect forecast, commercial observations, opportunity, intervention, approval, exact operation, execution, receipt, observation, revenue actual, variance, Plan update and replay.

### Exit evidence

One named Account with commit, environment, source versions, forecast version, WorkPacket, binding, receipt, observation, reconciliation, revenue actual and replay.

## Sprint 13 — durable WorkGraph runtime

### Work

WorkGraph schema, node states, worker, wait states, timers, event wake, retries, dead-letter, restart recovery and pause/resume/kill.

### Demo

Workflow survives restart and human wait without duplicate effect.

## Sprint 14 — Recipe Library and Requirement Compiler

### Work

RecipeDefinition, RecipeVersion, validation, publishing, fingerprint applicability, requirement compiler, cost estimate, missing-state output, immutable versioning and state-independent export.

### Demo

Same recipe evaluated for two Accounts with different requirements.

## Sprint 15 — Opportunity Horizons and Workspace Compiler

### Work

OpportunityHorizon, persistence, compare/select, WorkspaceManifest, component registry, renderer, component permissions and action-to-WorkPacket mapping.

### Demo

Two Accounts compile materially different workspaces from the same recipe without code changes.

## Sprint 16 — automation, delegation and bounded autonomy

### Work

AutomationDefinition, AutomationRun, triggers, schedules/events, delegation, expiry, budgets, approvals, notifications, suspension and revocation.

### Demo

Low-risk bounded automation executes while higher-consequence sibling pauses for approval.

## Sprint 17 — customer operations, privacy and support

### Work

Onboarding, users/roles, connections, consent/suppression, export, deletion, support tooling, operator console, incident queue, usage/cost reporting, evidence export and runbooks.

### Demo

Onboard, operate, export and close/delete a test Account.

## Sprint 18 — hardening and release candidate

### Work

Load, queue saturation, failure injection, security review, dependency review, migration rehearsal, backup/restore, rollback, SLO dashboards, alerts, runbooks and full acceptance suites.

### Exit

Named release candidate with explicit residual risks.

---

# PART XXIII — PHASE ACCEPTANCE

## 108. Phase One

One named CSR/Beem Account must demonstrate tenant/account setup, identity, source admission, explicit unknown/stale/conflicted state, minimum hydration, forecast baseline, specialist/commercial observation, Account Manager explanation, candidate Plan/WorkPacket, policy, authority, exact binding, registered capability execution, receipt, independent observation, reconciliation, commercial actual, Account re-entry, forecast update, Plan update and replay.

## 109. Phase Two

One Objective must demonstrate versioned Plan, durable WorkGraph, at least two capability classes, wait/event/approval, RecipeRun, multiple horizons where applicable, WorkspaceManifest, bounded automation, exact operation, observation, reconciliation and new Plan version.

Also prove worker restart, duplicate event, stale state, changed payload, revoked authority, expired automation, provider timeout and possible-write reconciliation.

---

# PART XXIV — DEFINITION OF DONE

## 110. Feature DoD

Canon match; versioned schema; documented API/event; tenant-safe; identity explicit; errors explicit; observability; unit/contract/negative tests; migration; rollback; maturity update; runbook impact; honest unknown/error UX.

## 111. Connector DoD

Environment, credential reference, supported/unsupported operations, data classes, purpose, rate, idempotency, errors, timeout class, receipt, observation, reconciliation, health, suspension, support, contract tests, test evidence and no direct UI/agent bypass.

## 112. Recipe DoD

Objective class, applicability, required/optional/prohibited state, freshness, capabilities, graph, branch rules, missing-state rules, approval/consequence classes, workspace, measurement, cost, re-entry, immutable version, no customer data, no inherited authority and two-account compilation test.

## 113. Release DoD

Code tag, migration tag, config/policy versions, green tests, green negative/tenant suites, release notes, known issues, rollback, backup verification, dashboards, alerts, runbooks, owner sign-off and maturity evidence.

---

# PART XXV — RISKS AND OPEN DECISIONS

## 114. Blocking decisions before production side effects

- long-term canonical repository owner/name;

- rights/assignment/licensing of legacy donor code;

- legacy schema disposition;

- field-level systems of record;

- initial forecast metrics/horizon;

- first production write;

- first mobility/quote write operations;

- auth/service identity standard;

- privacy owner and retention;

- SLO targets;

- external provider rights/capability state;

- production hosting/data/communications/model ownership;

- first pilot Account;

- named acceptance owners.

## 115. Technical risks

Legacy semantics leaking into Beem; mixed schema wholesale import; duplicate truth masters; direct provider access surviving legacy UI; authority collapsed into RBAC; receipt collapsed into outcome; duplicate events; blind retry after possible write; conversation becoming truth; forecast self-confirmation; over-hydration/privacy leakage; usage runaway; recipe leakage; workspace compiler becoming arbitrary code generation; incomplete observability; unverified provider capability.

---

# PART XXVI — DEVELOPER START INSTRUCTION

## 116. Read order

- BEEM_FULL_PRODUCT_CANON_v1_0.md

- BEEM_FULL_BUILD_SPECIFICATION_v1_0.md

Then code, tests, migrations and ADRs.

Do not derive product requirements from older planning documents.

## 117. Ticket rule

Every ticket includes owning sprint/epic, module, objective, contract/schema, truth behaviour, tenant/security impact, authority/consequence impact, events, errors, tests, acceptance evidence and migration/rollback where relevant.

## 118. First engineering sequence

Sprint 0 baseline; Sprint 1 tenant/account; Sprint 2 truth/provenance; Sprint 3 hydration; Sprint 4 WorkPacket/evidence; Sprint 5 control; Sprint 6 execution; Sprint 7 observation/reconciliation.

Only after those gates may real external side effects be enabled.

UI read models, acquisition inspection, CRM preparation and provider capability discovery may proceed in parallel, but no side effect may get ahead of identity, state, authority, exact binding, receipt and reconciliation.

## 119. Final build statement

Beem is built correctly when the customer experiences one intelligent commercial operating product while the implementation preserves:

- current state versus candidate;

- forecast versus actual;

- recommendation versus permission;

- access versus authority;

- connection versus capability;

- capability versus consequence;

- request versus acknowledgement;

- acknowledgement versus outcome;

- plan versus execution;

- customer state versus reusable recipe;

- conversation versus authoritative state;

- projection versus external truth;

- execution versus observed business result.

The target is not maximum automation.

The target is useful, durable, bounded commercial agency with evidence.
