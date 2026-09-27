# BEEM FULL PRODUCT CANON v1.0

Product: Beem by CSR

Status: OWNER-DIRECTED REPLACEMENT PRODUCT CANON / CURRENT BEEM PRODUCT DIRECTION

Audience: Beem product, engineering, data, security, operations, commercial and delivery teams

Date: 26 September 2026

Repository role: Developer context and product authority. When the companion Full Build Specification is committed and the repository cleanup is completed, these two documents are the only operative Beem build documents in the repository. Older or superseded planning documents remain provenance only and must not be used to derive implementation requirements.

Evidence boundary: This canon defines what Beem is intended to be and the product laws the implementation must preserve. It is not, by itself, proof that a capability is implemented, deployed, rights-cleared, commercially agreed, operationally exercised or validated.

## 0. The one-sentence canon

Beem is CSR's adaptive, agentic commercial operating product: it gives a business one persistent Account and Account Manager across its commercial technology estate, compiles the minimum state, expertise, workflow and connected capabilities required for the objective at hand, executes only exact operations that are actually authorised, observes what really happened, and replans from measured reality.

## 1. Reading rule for the development team

This document answers what we are building, why it exists, how the parts relate, what the customer experiences, what Beem may and may not do, and which use cases the architecture must support.

The companion document, BEEM FULL BUILD SPECIFICATION v1.0, will answer how the team builds it, the module boundaries, contracts, sequencing, sprints, tests, gates and acceptance criteria.

Once both documents are present in the canonical Beem repository, do not reconstruct product direction from older plans. In particular:

- older historical product alias naming is historical provenance;

- any Beem-facing dependency on an unrelated external governance runtime is superseded;

- any document that makes Beem merely a marketing dashboard is superseded;

- any document that makes Beem a reskinned donor product is superseded;

- any donor repository, package name or implementation detail is subordinate to the Beem contracts defined here;

- source presence is not proof of rights, production readiness, commercial entitlement or validation.

The rule for developers is simple: the product semantics belong to Beem; donor code supplies mechanics only where explicitly admitted.

## 2. Product identity and hard boundaries

### 2.1 Beem

Beem is a CSR-owned commercial operating product. It is the current customer-facing product identity.

Beem owns:

- the customer Account and workspace;

- the AccountPlan and objective model;

- the Agentic Account Manager;

- forecasting, scenario and commercial planning;

- WorkPackets and durable work;

- the adaptive Recipe Runtime and Workspace Compiler;

- customer-facing CRM and revenue operating state;

- Beem acquisition intelligence as a specialist acquisition-intelligence capability family;

- the first-class marketing execution surface across web, SEO/AI search, paid search, paid social, organic social, email, written content, visual creative/art, CRM and measurement;

- Beem mobility capability as a bounded mobility, quote and fulfilment capability track;

- the Beem Local Control Plane;

- capability and connector registration;

- customer approvals, delegation and autonomy settings;

- receipts, observations, reconciliation and evidence UX;

- the product experience for external provider network and other external add-ons;

- human takeover, pause, correction, escalation and kill controls.

### 2.2 Beem Local Control Plane

The Beem Local Control Plane (BLCP) is the CSR-owned Beem control layer.

It owns the Beem contracts for:

- qualified state;

- minimum sufficient hydration;

- policy evaluation;

- authority resolution;

- consequence classification;

- exact-operation binding;

- capability eligibility;

- execution grants and expiry;

- receipts;

- independent observation;

- reconciliation;

- verification;

- replay-safe evidence;

- fresh state re-entry.

BLCP is a Beem-local control plane. It is not a renamed donor substrate or an external governance runtime. Useful neutral engineering patterns may be donated into its implementation, but its semantics are Beem semantics.

### 2.3 No external governance-runtime dependency

Beem has no required dependency on any separate governance product, external doctrine runtime or unrelated control service.

Everything needed for Beem's own qualified-state, policy, authority, exact-operation, receipt, observation, reconciliation and re-entry route is owned inside Beem through BLCP and the Beem application contracts.

Older architecture notes that place an external governance runtime in the Beem execution path are superseded for Beem scope.

### 2.4 Beem acquisition intelligence

Beem acquisition intelligence is a protected specialist capability family inside Beem. Earlier acquisition implementation labels are provenance only.

Beem acquisition intelligence may observe, diagnose, score, compare, explain, forecast specialist acquisition effects, create recommendations and prepare candidate work. Beem acquisition intelligence does not become the central governor and does not acquire authority to publish, send, spend, charge, book, dispatch or mutate another system merely because it can technically do so.

### 2.5 Neutral donor substrate

Beem may reuse rights-cleared neutral engineering mechanics from a separately owned donor substrate, but the donor is not the Beem runtime.

Candidate mechanics include canonicalisation, hashing, version/provenance patterns, deterministic context construction, bounded execution, idempotency, ledger, correlation, replay and conformance patterns.

Beem does not inherit donor customer data, donor-domain semantics, authority, permits, role names, deployment bindings, product identity or live runtime dependency.

### 2.6 Legacy operational donor

The legacy operational donor source is quarantined and exists only to provide explicitly admitted generic mechanics. It is not a Beem live dependency and not a substitute for a proper connector.

Useful donor candidates include tenancy, scoped access, audit/activity, logging, navigation, generic account/contact/workflow ideas and integration shell patterns. Recruiting, candidate/CV, client-live data, credentials, production domains and deployment bindings do not become Beem meaning by copy.

A future live external recruiting source integration, if ever required, is a separate connector decision with explicit rights, data, tenant, purpose, environment and API approval.

### 2.7 Beem mobility capability

Beem mobility capability remains a separately inspectable bounded capability and adapter track for mobility demand, enquiries, quotes, providers, availability/capacity, bookings, fulfilment, payments and observations.

Beem mobility capability is not a second Beem governor or an autonomous dispatch system. Stub and dry-run functions remain labelled as such until provider evidence says otherwise.

### 2.8 External provider network

The external provider network sits outside the Beem control boundary and is integrated only through explicit capability contracts.

Its provider systems, network, data, tools and company add-ons remain externally owned unless an executed agreement says otherwise. Beem integrates them through explicit, tenant-bound capability contracts.

A external provider network acknowledgement is not booking, dispatch, payment or fulfilment truth. Provider-native state remains authoritative inside the scope that the provider legitimately owns.

### 2.9 Other product programmes

Other product or research programmes remain outside Beem unless a later explicit Beem decision introduces a named, versioned interface.

No cross-product shared mutable substrate, hidden customer-data path, silent authority path or runtime dependency is created merely because teams, ideas or donor mechanics overlap.

## 3. The product thesis

The standard SaaS model says:

Here is our product. Configure our features to fit your business.

Beem's target model is different:

Tell Beem what this business is trying to achieve. Beem resolves what it currently knows, what it still needs, which operating recipe applies, which capabilities are available, what work can safely proceed, what requires a decision, and what should be observed afterwards. It compiles the operating surface for the job, executes only within active authority, and recompiles from reality.

Beem is therefore not intended to become a giant fixed suite in which every industry request becomes a new hard-coded module.

The scalable object is an invariant kernel plus versioned recipes, qualified business state, typed capabilities and compiled workspaces.

The same product can support a chauffeur operator, a tour operator, an event transport business, a marketing client or another service business without creating a new code fork for every operating model.

## 4. The customer promise

The simplest customer promise is:

Connect your business. Tell Beem what you are trying to achieve. Let Beem manage the work within the boundaries you control.

The experience should feel like a persistent digital commercial account manager, not like a chatbot that forgets the business between conversations.

A customer should be able to ask:

- "We need another £400k of profitable revenue this quarter."

- "Why have enquiries dropped, and what should we do?"

- "We have spare capacity next week. Fill it without breaking margin."

- "Improve our AI-search visibility and turn the opportunity into revenue."

- "Follow up every recoverable quote over £5,000 that has been inactive for four days."

- "Which customers are going dormant?"

- "Build a tourism offer around our vehicles, boats and local attractions."

- "We normally run 50 vehicles but need 300 for a major event."

- "Show me which drivers are actually ready for this event and what is missing."

- "Run the work you are already authorised to run and bring me only the decisions that require me."

Beem responds by coordinating current business state, specialist intelligence, plans, humans, software and evidence.

## 5. The canonical operating loop

The Beem loop is:

Account + qualified source state -> minimum sufficient hydration -> objective/request -> viable horizons -> candidate plan/work -> CSR and tenant policy -> authority resolution -> exact-operation binding -> bounded registered capability -> attempt/receipt -> independent observation -> reconciliation/verification -> measured Account re-entry -> forecast/plan update

The system must not collapse these stages.

The most important separations are:

- observation is not prediction;

- prediction is not permission;

- candidate work is not consequence;

- role membership is not exact authority;

- capability is not permission;

- approval is not a blanket future grant;

- provider acknowledgement is not verified outcome;

- CRM projection is not provider-native truth;

- forecast is not actual;

- scenario is not commitment;

- high model confidence is not authority;

- conversation memory is not current business truth;

- re-entry is fresh measured state, not inherited authority.

## 6. Federated truth, not one giant database

Beem is the system of orchestration, qualification, decisions, recipes, work, state projections and evidence. It is not automatically the universal source of truth for every connected system.

Examples:

- a dispatch platform may own provider-native booking and dispatch truth;

- a payment platform may own transaction and settlement truth;

- external training provider or another training provider may own the training result it actually records;

- external recruiting source may own approved recruiting state inside its legitimate boundary;

- Beem mobility capability may own its mobility demand and quote objects;

- Beem acquisition intelligence may own its specialist appraisal artifacts;

- Beem CRM may own Beem-native account, activity, opportunity and work state;

- external provider network-owned products retain their declared provider truth.

Beem stores qualified references or projections, provenance, freshness, conflicts, decisions, receipts and reconciled observations.

When two sources disagree, Beem does not resolve the conflict because a model can produce a fluent answer. The conflict is represented and resolved according to the field-level information-authority binding.

## 7. State qualification and hydration

Beem does not send the entire Account to every user, model, tool or provider.

For each route, the Hydration Engine determines the minimum sufficient permitted state for the intended receiver and consequence.

Material state can be:

- available;

- admitted;

- route-relevant;

- missing;

- stale;

- conflicted;

- unauthorised for the purpose;

- estimated;

- candidate;

- observed;

- verified.

Hydration considers:

- tenant and account;

- purpose;

- objective;

- receiver;

- intended operation;

- consequence class;

- source/provenance;

- object version;

- freshness;

- privacy;

- consent;

- authority-bearing state;

- uncertainty;

- proof requirements;

- connector requirements;

- explicit exclusions.

If the required state is not sufficient, Beem requests it, stages other work, holds, recomputes, escalates or stops. It does not invent the missing state.

## 8. The Account

The Account is the tenant-isolated operating home for the business.

It includes or references, where relevant:

- organisation and legal identity;

- locations and operating geography;

- users, memberships, roles and service identities;

- authority and delegated scopes;

- services, products and offers;

- prices and commercial rules;

- audiences, customers and segments;

- approved claims and proof assets;

- brand and communication rules;

- websites and pages;

- conventional search and AI-search visibility;

- CRM state;

- enquiries and leads;

- opportunities;

- proposals and quotes;

- bookings/orders;

- payment and revenue observations;

- campaigns and channels;

- operating capacity and availability;

- partners and providers;

- budgets and cost ceilings;

- objectives and plans;

- recipes and active recipe runs;

- WorkPackets and workflow nodes;

- approvals and exceptions;

- missing-state requests;

- risks and holds;

- receipts, observations and discrepancies;

- measured outcomes;

- usage and cost receipts.

All material state is source-aware, version-aware and time-qualified.

## 9. Operator Fingerprint

The OperatorFingerprint is a compiled, stable-but-revisable projection of the Account for adaptive operation.

It is not a second truth master.

It describes the business characteristics that matter to recipe selection and workspace compilation, such as:

- services;

- locations;

- fleet/equipment;

- people and roles;

- connected systems;

- available capabilities;

- operating constraints;

- licences/evidence references;

- brand and commercial rules;

- known preferences;

- active policies;

- current capacity;

- current market state.

A recipe is selected and hydrated against the OperatorFingerprint, but authoritative values are still resolved from the underlying source bindings.

## 10. AccountPlan and Objectives

Every Account has a persistent, versioned AccountPlan.

The AccountPlan connects business intent to an executable commercial programme without becoming permission.

It includes:

- objectives and priority;

- baselines and horizons;

- markets;

- services and offers;

- audiences;

- channels;

- approved claims and proof gaps;

- budgets and cost envelopes;

- target journey or operating states;

- capacity assumptions;

- campaigns and initiatives;

- recipe runs;

- active work;

- risks and constraints;

- review cadence;

- success measures;

- escalation requirements;

- linked forecasts and scenarios.

An Objective records the desired measurable state, accountable owner, period, constraints, success measures and authority boundary.

Plans are candidate strategy. A plan may be excellent and still require fresh state, approval or a new exact-operation binding before consequence.

## 11. Forecasting and scenario model

Forecasting is a first-class Beem domain, not a decorative chart.

Canonical forecasting objects include:

- ForecastDefinition;

- ForecastVersion;

- Scenario;

- Assumption;

- MetricSeries;

- ForecastRun;

- ActualObservation;

- Variance;

- ForecastDecisionLink.

Every forecast must be:

- versioned;

- time-bounded;

- reproducible from named source versions;

- explicit about assumptions;

- explicit about uncertainty;

- linked to actual observations;

- clearly labelled as forecast/scenario rather than fact;

- incapable of granting authority.

The system must prevent self-confirmation. A Beem recommendation, campaign, model explanation or provider acknowledgement cannot be used as evidence that the forecast came true.

Forecast accuracy and commercial impact are scored against registered observation sources.

## 12. The sell-through lifecycle

Beem's core commercial path must be explicit:

Signal/Opportunity -> Offer -> Campaign/Outreach -> Lead -> Qualified Opportunity -> Proposal/Quote -> Booking/Order -> Fulfilment handoff -> Payment/Revenue observation -> Attribution -> Re-entry

Every stage has:

- a canonical identity;

- an owning source or system;

- a status vocabulary;

- required evidence;

- permitted transitions;

- reconciliation rules;

- timestamps and versions;

- links back to the objective and work that caused the transition.

Important distinctions:

- a lead is not revenue;

- a CRM stage is not verified revenue;

- a quote is not an accepted order;

- a booking acknowledgement is not completion;

- payment authorisation is not settlement;

- settlement is not automatically recognised margin;

- attribution may remain partial or unknown.

## 13. The adaptive Recipe Runtime

The Recipe Runtime is how Beem becomes deeply configurable without becoming an unmaintainable collection of bespoke products.

The runtime contains nine cooperating functions:

- Operator Fingerprint — compiles the stable operating characteristics of the Account.

- Connector Registry — exposes typed read/propose/execute capabilities.

- Recipe Library — stores reusable versioned operating knowledge.

- Requirement Compiler — determines the state and capability requirements for the objective.

- Hydration Engine — retrieves only the permitted, route-relevant state.

- Opportunity/Horizon Engine — preserves multiple viable routes instead of prematurely collapsing one generated answer into the plan.

- Decision + Consequence Layer — separates recommendation, readiness, conditions, authority and execution.

- Workspace Compiler — renders the appropriate operating surface from an allow-listed component vocabulary.

- Receipt + Re-entry Engine — observes what actually happened and recompiles from the new state.

The Recipe Runtime is Beem product architecture. The public no-code builder, broad vertical SDK and open recipe marketplace are later productisation layers and do not block the first release.

## 14. Recipe canon

A Recipe is not a prompt.

A Recipe is a versioned declarative operating object.

A Recipe contains, as applicable:

- recipe identity and version;

- owner and authorship;

- visibility and licensing;

- objective;

- applicable OperatorFingerprint conditions;

- required state;

- optional state;

- prohibited state;

- freshness requirements;

- required capabilities;

- compatible connector classes;

- workflow graph;

- branch conditions;

- missing-state behaviour;

- approval requirements;

- consequence classes;

- workspace manifest;

- permitted UI components;

- executable capabilities;

- fallback/manual routes;

- measurement plan;

- success and failure observations;

- re-entry rules;

- cost/usage budget;

- expiry and review date.

Recipe is not customer state.

A reusable recipe can encode expert operating knowledge without carrying the originating operator's passenger list, pricing, users, customer data, private history or authority.

## 15. Recipe lifecycle and champion model

Recipe visibility can evolve through:

PRIVATE -> ORGANISATION -> CSR/BEEM CURATED -> MARKETPLACE

The data model should support this lifecycle from the beginning even though the public marketplace is deferred.

Rules:

- a recipe version is immutable once used for a material run;

- improvements create a new version;

- an active run may remain pinned to its original version;

- a destination operator hydrates its own state into the recipe;

- customer state never becomes transferable recipe content;

- customer authority never transfers with the recipe;

- successful outcomes may support a proposed recipe improvement but do not silently rewrite the recipe;

- authorship and licensing remain explicit.

This enables a future Recipe Champion model in which domain expertise becomes reusable platform IP without centralising customer data.

## 16. Workspace Compiler

Beem should not ask a model to generate arbitrary React, SQL or production code for each customer.

The Workspace Compiler emits a versioned WorkspaceManifest using an allow-listed component vocabulary.

Candidate components include:

- Account pulse;

- KPI cards;

- map;

- capacity grid;

- calendar;

- timeline;

- kanban;

- quote builder;

- inventory selector;

- training matrix;

- driver readiness table;

- event command board;

- tour itinerary;

- pricing editor;

- approval inbox;

- lead queue;

- affiliate/provider map;

- compliance checklist;

- demand heatmap;

- communications centre;

- payment status;

- exception queue;

- forecast and variance panel;

- pipeline;

- evidence drawer.

The rendered interface is a projection of the current objective and operator state.

A Utah experience operator may see an Experiences & Tours workspace. A major-event operator may see an Event Command Center. A recruiting-heavy operator may see Driver Pipeline + Readiness. A small local service business may see Leads, Quotes, Today's Work and two recommended growth actions.

Underneath, these are the same Account, Recipe, WorkPacket, capability, authority and evidence contracts.

## 17. The Agentic Account Manager

The Agentic Account Manager is the primary human-facing operating interface.

It is not just chat and it is not governance authority.

It may:

- understand an objective;

- explain current state;

- surface uncertainty and missing state;

- compare viable horizons;

- propose or revise AccountPlans;

- create RecipeRuns;

- create candidate WorkPackets;

- coordinate specialist capabilities;

- request human decisions;

- maintain durable work;

- schedule permitted future work;

- wait for events or providers;

- retry within defined rules;

- compensate or escalate;

- monitor results;

- explain discrepancies;

- re-plan from measured state.

It may never infer that it has authority because:

- a user asked;

- a model recommended;

- the same action worked before;

- another account was allowed;

- a role normally has access;

- a connector has a write endpoint;

- a forecast says the action is attractive;

- Beem acquisition intelligence assigns a high score;

- an old approval exists for materially changed state.

## 18. WorkPacket

WorkPacket is the stable bridge from intelligence to real-world consequence.

A WorkPacket carries:

- objective and reason;

- accountable owner;

- source request/opportunity/issue;

- qualified evidence;

- provenance;

- current state fingerprint;

- missing, stale or conflicted state;

- candidate plan/artifact/payload;

- target system/account/object;

- consequence class;

- requested capability;

- policy result;

- authority requirement;

- approval evidence;

- exact bound operation;

- payload digest;

- budget/quantity/time limits;

- expiry;

- idempotency;

- execution state;

- provider receipt;

- independent observation;

- discrepancy;

- reconciliation;

- verification;

- commercial outcome;

- re-entry link;

- next-plan effect.

The customer should be able to inspect a WorkPacket and understand what Beem wants to do, why, what it knows, what is missing, what will change, who can approve it, what actually happened and what happens next.

## 19. BLCP decision and consequence model

BLCP keeps technical ability separate from business permission.

At minimum it resolves:

### Qualification

Is the required state present, fresh enough, non-conflicted enough and permitted for this use?

### Policy

Does CSR policy, account policy and the relevant operation rule permit the route to continue?

### Authority

Which human or service identity is authorised to approve or perform this class of operation for this account, target, amount, purpose and time window?

### Exact-operation binding

What exact provider, target, action, payload, amount, capability version, evidence set, approval reference, expiry and idempotency key are being authorised?

### Execution

Can the registered capability perform only the bound operation within its declared environment and limits?

### Evidence

What did the provider acknowledge, what was independently observed, and is there a discrepancy?

### Re-entry

What measured state may now enter the Account, and which forecast, plan or recipe branch must be recomputed?

## 20. Runtime outcomes

Do not reduce the internal control result to a single Boolean.

The runtime should distinguish outcomes such as:

- READY;

- READY_WITH_CONDITIONS;

- STAGE;

- REQUEST_STATE;

- HOLD;

- RECOMPUTE;

- ESCALATE;

- STOP;

- UNKNOWN;

- COMPLETED after observation/reconciliation.

The UI may make those states simple to understand, but the underlying system must retain their differences.

Example:

"Can we launch Zion executive tours next month?"

If vehicles, booking and payments exist but required insurance/jurisdiction evidence is missing, the answer is not a misleading "yes" or "no".

The useful answer is:

STAGE the commercially viable work; REQUEST_STATE for the missing evidence; do not activate the blocked branch until the required state is admitted.

## 21. Authority and autonomy

Beem autonomy is granular.

The customer may configure operation classes such as:

- observe only;

- recommend;

- prepare candidate work;

- execute after approval;

- execute automatically within a bounded envelope;

- never execute.

An automation envelope can bind:

- account;

- operation class;

- provider;

- target;

- budget;

- amount;

- claim class;

- content type;

- audience;

- time window;

- data class;

- consequence class;

- required evidence;

- retry limits;

- expiry;

- revocation.

There is no global "autonomous mode" that gives the Account Manager ambient corporate power.

## 22. Capability-based integration

Beem integrates capabilities, not vendor privilege.

A recipe should ask for:

- booking.read;

- quote.create;

- reservation.create;

- dispatch.read;

- driver.read;

- driver.assign;

- availability.read;

- payment.request;

- payment.observe;

- training.assign;

- training.result.read;

- message.send;

- web.publish;

- crm.activity.create;

rather than hard-coding "use vendor X".

The Capability Registry maps the requested operation to an actual connector that is installed, healthy, permitted and compatible for the Account.

If the connector cannot perform the operation, Beem returns a typed unsupported/unverified state or creates a controlled manual work route. It does not fabricate an integration.

### 22.1 First-class marketing execution surface

Beem treats the following as first-class marketing capability families that can be coordinated by the Account Manager in one Plan/WorkGraph:

- web and website operations, including page/content mutation and publishing;

- organic search, SEO and AI-search visibility;

- paid search, including campaign creation and optimisation, bid/budget management, creative/landing-page coordination and measurement;

- paid social, including campaign/audience/creative operations, spend controls and measurement;

- organic social, including planning, creation, approval, scheduling/publishing, engagement observation and commercial re-entry;

- email, including composition, sequencing, sending, replies, bounce/suppression handling, campaign measurement and CRM re-entry;

- written content creation, including copywriting for web pages, articles, landing pages, emails, ads and social posts;

- visual creative/art, including generation, variation, approval-ready asset management and campaign attachment;

- CRM and measurement, including audience/contact/consent state, channel observations, attribution candidates, pipeline/revenue observation and re-entry.

These capability families do not acquire ambient authority. Each consequential publish, send, spend, budget/bid change, customer-visible mutation or external-system write is a separate WorkPacket + BLCP exact operation with capability eligibility, receipts, independent observation, reconciliation and re-entry.

## 23. Connector contract

Every connector declares:

- connector identity and version;

- owner;

- tenant/account binding;

- environment;

- credential reference;

- authentication scope;

- supported read operations;

- supported propose operations;

- supported execute operations;

- prohibited operations;

- input/output/event schemas;

- data classes and declared purpose;

- source-authority classes;

- freshness;

- rate and usage limits;

- cost model;

- consequence class;

- approval class;

- idempotency behaviour;

- webhook/polling mode;

- observation/reconciliation source;

- error taxonomy;

- retry/compensation rules;

- health;

- suspension;

- support/incident owner.

Connected does not mean authorised. Healthy does not mean fresh. Token scope does not mean business authority.

## 24. Beem acquisition intelligence

Beem acquisition intelligence is the first major specialist capability family.

It can support:

- website/source-layer state;

- technical and semantic evidence;

- AI-search visibility;

- conventional search signals;

- schema/structured-data opportunities;

- claim/proof gaps;

- first-party telemetry;

- category/competitor movement;

- appraisals and scorecards;

- strategy candidates;

- content/page candidates;

- post-change measurement.

The canonical Beem acquisition intelligence route is:

Beem acquisition intelligence observation -> Account evidence -> diagnosis/opportunity -> candidate intervention -> WorkPacket -> BLCP -> exact website/content operation -> provider receipt -> live-site observation -> commercial observation -> re-entry

Beem acquisition intelligence scores and recommendations remain candidate state.

## 25. CRM and revenue operating model

CRM is not a side database. It is part of the Account's commercial operating state.

Core CRM/commercial objects include:

- Account;

- Contact;

- ConsentState;

- Lead;

- Opportunity;

- Activity;

- Proposal;

- Quote;

- Booking/Order projection;

- Payment projection;

- RevenueObservation;

- Attribution record.

Beem may be the system of engagement while another provider remains the system of record for specific fields.

Required behaviour includes:

- external-ID mapping;

- dedupe and entity resolution;

- match confidence;

- human resolution where needed;

- tombstones;

- merge/unmerge evidence;

- consent and suppression;

- follow-up SLAs;

- attribution limits;

- safe write-back;

- reconciliation with provider/payment truth.

## 26. Beem mobility capability

Beem mobility capability contributes a bounded mobility and fulfilment capability family.

Potential ports include:

- mobility enquiry;

- demand classification;

- availability/capacity;

- quote options;

- quote issue;

- booking/fulfilment handoff;

- provider status;

- invoice/payment observation;

- completion/cancellation/exception observation.

Beem owns the Account, WorkPacket, exact operation and evidence grammar. The declared provider owns its operational truth.

Beem mobility capability can also act as an opportunity sensor. Recurring demand signals can trigger a Recipe evaluation without automatically turning those signals into a new product or promise.

## 27. External provider network and add-ons

Every external provider or company add-on is an external capability with an explicit manifest.

The manifest must cover:

- product/provider identity;

- owner and legal entity;

- environment;

- tenant installation;

- credentials;

- entitlements;

- supported operations;

- consequence classes;

- schemas/events;

- data role and purpose;

- residency/retention/deletion;

- authority and approval;

- rate/availability/freshness;

- idempotency;

- receipts;

- observation;

- reconciliation;

- UNKNOWN behaviour;

- timeout/retry/compensation/cancellation;

- support and incident ownership;

- commercial entitlement and limits;

- suspension/termination.

No grouped claim such as "external provider network integration complete" is valid. Each function earns its own maturity state.

Where no reliable API exists, Beem may generate an exact manual provider task, wait for evidence and reconcile the outcome. Manual execution is a first-class bounded capability, not an invisible workaround.

## 28. Evidence, eventing and replay

Every material event needs a canonical envelope containing:

- event ID;

- event type and version;

- tenant/account;

- source;

- subject/object;

- occurred time;

- received time;

- correlation and causation;

- idempotency;

- payload reference/hash;

- classification;

- provenance;

- replay policy.

Where state change and event publication must remain atomic, the implementation should use reliable outbox/inbox patterns.

Replay must be side-effect free at production provider boundaries. Replaying evidence cannot resend an email, recharge a card or recreate a booking.

## 29. Receipt, observation and re-entry

Beem must never mark success simply because its own call returned success.

The evidence path distinguishes:

- requested;

- prepared;

- permitted;

- committed;

- dispatched;

- provider acknowledged;

- possible write;

- externally observed;

- commercially observed;

- reconciled;

- verified;

- failed;

- unknown.

Example:

"I sent a quote" is an attempt/receipt.

"The provider shows the quote exists" is an external observation.

"The customer accepted the quote" is a different observation.

"The booking was fulfilled" is another.

"Payment settled" is another.

Those events can influence the next plan only after they enter the Account with their proper status and provenance.

## 30. Customer experience and navigation

Beem has one front door.

The stable product navigation should converge around:

- Home / Account Pulse — what changed, what matters, what is stale or exceptional;

- Account Manager — objective-led conversation and coordination;

- Plan — objectives, current AccountPlan, assumptions, capacity and risks;

- Forecast — scenarios, actuals, variance and decision links;

- Pipeline / CRM — accounts, leads, opportunities, quotes/bookings and follow-up;

- Work / Approvals — WorkPackets, durable work, exact decisions, pause/kill and exception state;

- Beem acquisition intelligence — website, visibility, evidence, appraisals and candidate improvements;

- Connections — connectors, capabilities, scopes, health, freshness, supported operations and suspension;

- Evidence — sources, decisions, attempts, receipts, observations, reconciliation and replay;

- Settings / Policy / Permissions — users, roles, delegations, automation envelopes, budgets, privacy and retention.

The Workspace Compiler may then add objective-specific surfaces inside this stable product frame.

## 31. Evidence UX

For any material recommendation or action, an authorised user should be able to answer:

- What did Beem notice?

- Which source says that?

- How fresh is it?

- What is known, inferred, estimated or missing?

- What conflicts?

- What does Beem recommend?

- What alternatives were considered?

- What will actually change?

- Which capability will do it?

- Who or what may approve it?

- What exact scope/budget/target is bound?

- Has execution been attempted?

- What did the provider acknowledge?

- What was independently observed?

- Is there a discrepancy?

- What entered the Account afterwards?

- What changed in the forecast or Plan?

## 32. Use case canon

The following are representative uses the architecture must support. They are not separate code products.

### 32.1 AI-search visibility recovery

Beem detects declining search/AI visibility for commercially important services.

It:

- hydrates current page, query, claim, proof, demand and capacity state;

- uses Beem acquisition intelligence to explain the evidence;

- creates one or more candidate page/source-layer interventions;

- links the intervention to expected commercial impact without treating the prediction as fact;

- routes the exact publish/change operation through BLCP;

- observes the live site independently;

- observes enquiries/pipeline/revenue separately;

- updates the Plan from the measured result.

### 32.2 Omnichannel campaign creation and execution

A customer gives Beem an approved growth objective.

Beem's first-class marketing execution surface for this use case is web + SEO/AI search + paid search + paid social + organic social + email + written content + visual creative/art + CRM + measurement. The Account Manager may coordinate these channels in one campaign/Plan, but channel consequences remain independently governed and may be permitted, held, staged or rejected separately.

Beem:

- resolves audience, offer, claims, channels, budget and capacity;

- creates a candidate campaign plan;

- creates draft assets;

- creates channel-specific written content for web pages, articles, landing pages, emails, ads and social posts;

- creates or manages visual creative/art variants for approved channel use;

- identifies missing proof or approval;

- binds channel operations separately;

- launches only the operations actually permitted;

- monitors channel and commercial observations;

- recomputes spend and next actions from actuals.

### 32.3 Dormant customer reactivation

Beem detects accounts that are becoming dormant.

It:

- resolves current relationship, consent, hold and commercial state;

- creates eligible segments;

- proposes a bounded sequence;

- excludes held or suppressed contacts;

- executes within the configured communication envelope;

- observes replies, meetings, quotes, bookings and revenue;

- updates opportunity state and future reactivation logic.

### 32.4 Quote and enquiry recovery

Beem detects recoverable unconverted demand.

It:

- identifies enquiries/quotes with no activity;

- checks current status, account holds, validity, margin criteria and contact permission;

- proposes or performs permitted follow-up;

- assigns high-value exceptions to a human;

- observes reply/acceptance/booking/payment;

- preserves unknown outcome if the external system cannot be reconciled.

### 32.5 Capacity-aware demand

Beem detects under- or over-supplied capacity.

It:

- admits current capacity and demand state;

- forecasts near-term gap;

- proposes channel, segment, pricing or follow-up actions;

- never treats capacity context as permission to spend or promise availability;

- rechecks current capacity before material booking or campaign consequence.

### 32.6 Forecast-to-revenue loop

Beem combines Beem acquisition intelligence, CRM, Beem mobility capability and other registered observations.

It:

- produces a versioned forecast/scenario;

- compares actual versus expected;

- identifies candidate constraints or opportunities;

- creates candidate interventions;

- binds exact CRM, communication, CMS, quote or provider operations;

- observes pipeline/revenue outcomes independently;

- reconciles attribution;

- reforecasts from measured state.

This is the minimum commercial proof loop for Phase One.

### 32.7 Utah / Zion tourism expansion

An operator says:

"I have chauffeur vehicles, boats and jet skis. Build me a tourism business around here."

Beem does not hard-code a Zion module.

It evaluates viable branches such as:

- executive national-park transfers;

- private day tours;

- hotel/FBO arrival packages;

- transport-to-water packages;

- equipment rental combinations;

- group/shuttle products;

- partner experiences;

- Vegas-linked itineraries.

The Tourism/Experience Recipe requests the state needed to compare those branches: geography, fleet/equipment, capacity, booking stack, payment capability, insurance/evidence, partner conditions, pricing, seasonality, channels and web capability.

The compiled workspace may show:

Experiences | Availability | Transport | Equipment | Partners | Itineraries | Quotes | Payments | Evidence | Marketing | Results

No new product fork is created.

### 32.8 Major Event Surge

An operator says:

"We normally operate 50 vehicles. We need to behave like a 300-vehicle company for four days."

The Major Event Surge Recipe hydrates:

- reservations and demand curve;

- staging locations;

- owned fleet;

- affiliate supply;

- drivers;

- training and evidence;

- dispatch configuration;

- event instructions;

- authorised passenger/group state;

- pricing/payment;

- incident routes;

- contingency capacity.

The workspace compiles an Event Command Center with demand vs capacity, fleet, affiliates, driver readiness, staging, live exceptions, communications, payments, incidents and reconciliation.

After the event, utilisation, farm-outs, delays, incidents, passenger issues, payment friction and successful procedures return as measured state. The next event run compiles differently.

### 32.9 Driver Readiness

Driver readiness may be distributed across external recruiting source, external training provider or another training system, dispatch, Beem CRM and operator evidence.

Beem compiles one readiness view without claiming that one database owns all facts.

It can show, for example:

- ready;

- training incomplete;

- documentation missing;

- affiliate confirmation pending;

- dispatch-state conflict.

A training provider remains authoritative for the result it actually records.

If Beem cannot perform a training assignment through a verified API, it creates an exact manual/provider WorkPacket and waits for an observation instead of fabricating integration success.

### 32.10 Beem mobility capability demand sensing and fulfilment

Repeated Beem mobility capability requests can become demand evidence.

Beem may detect a recurring pattern and propose:

"There is sufficient repeated demand to evaluate a new service Recipe."

It then evaluates the opportunity against capacity, providers, margins, evidence and operating constraints.

Beem mobility capability stays the demand/quote/fulfilment capability; Beem owns the opportunity, plan, WorkPacket and measured commercial re-entry.

### 32.11 Local service business digital account manager

A local service business opens Beem on Monday.

Beem observes:

- next-week capacity is high;

- airport bookings are below baseline;

- search demand is healthy;

- landing-page conversion has deteriorated;

- a competitor has gained visibility;

- dormant customers exist.

Beem proposes:

- page remediation;

- paid-media adjustment;

- dormant-customer outreach;

- selected account follow-up.

If website changes and customer follow-up are already delegated but paid-media changes above a threshold require approval, Beem executes only the delegated operations and brings the spend decision to the owner.

Observed enquiries, replies, bookings and revenue become new Account state.

### 32.12 external provider network portfolio and cross-vertical recipes

Where rights and interfaces exist, Beem can combine capabilities across external provider network-owned products without making each underlying vertical product become everything.

A cross-vertical Recipe may require transportation, tourism/experience, payment, marketing or other declared capabilities.

The Recipe asks for the capabilities. The Capability Registry chooses only verified installed operations.

Cross-vertical portfolio adjacency is a product direction, not proof that the underlying external provider network products already interoperate.

### 32.13 Recipe Champion

An expert operator describes how a major event, wine tour, NEMT operation, FBO movement or another specialist operation is run.

Beem helps extract the reusable method into a RecipeDraft.

The expert/human team reviews it.

The recipe is tested against synthetic/shadow tenants.

Only the state-independent process is publishable. Customer data and inherited authority remain excluded.

The destination operator receives the recipe, hydrates local state and obtains a locally valid operating configuration.

## 33. Failure behaviour

Failure handling is part of the product, not an implementation afterthought.

Canonical rules:

- every consequential operation has an idempotency key;

- retries cannot double-book, double-charge or double-message;

- provider discrepancy creates reconciliation;

- provider timeout after possible write becomes UNKNOWN until observed;

- stale state forces refresh/replan where material;

- expired or revoked authority stops consequence;

- changed payload/target/budget invalidates the old binding;

- unavailable connector produces a legitimate fallback/manual route;

- missing evidence produces a precise missing-state request;

- recipe/provider incompatibility triggers recompile;

- token/cost limits never convert missing required state into presumed state;

- replay never invokes a live provider;

- one tenant can never hydrate another tenant's state;

- paused or killed automation cannot continue;

- unsupported provider features remain unsupported.

## 34. Privacy, security and tenant isolation

Beem must preserve:

- tenant isolation;

- environment isolation;

- least privilege;

- explicit purpose;

- data classification;

- consent and suppression;

- credential isolation;

- secret references instead of secret payloads;

- service identity;

- target verification;

- cross-tenant denial;

- retention and deletion;

- export and portability;

- audit correlation;

- no raw secret/PII leakage into logs or evidence stores;

- webhook authenticity and replay protection;

- wrong-audience denial;

- non-production synthetic data by default;

- customer/provider data boundaries;

- requalification at boundaries where required.

Evidence stores should prefer references, hashes and minimum non-personal material over raw PII when the raw data is not required.

## 35. Identity, RBAC and delegation

Access control and consequence authority are separate.

The product must support:

- human principals;

- service identities;

- account membership;

- roles and permissions;

- delegated scopes;

- ABAC-style operation/target/data conditions where needed;

- approval authority;

- separation of duties where required;

- expiry;

- revocation;

- cross-tenant denial.

legacy operational donor and neutral donor-substrate access-control patterns may be adapted, but historical role names do not define the final Beem model.

## 36. Freshness and concurrency

Every material source class needs a freshness contract.

Relevant fields include:

- observed_at;

- valid_from;

- valid_to;

- source_version;

- stale_after;

- refresh strategy;

- object version/ETag;

- material-change invalidation rule.

Long-running work must re-resolve material state before consequence if the applicable freshness boundary has passed or the source version changed.

## 37. Cost and usage model

The product architecture should support:

platform retainer + metered consumption + connector/transaction costs where applicable.

The retainer funds the persistent operating estate: tenant, identity, state, recipes, connectors, evidence, storage, support and deterministic runtime.

Metered usage may cover variable work such as model reasoning, deeper hydration, research, large analyses, recipe compilation and premium external functions.

Deterministic work should not burn expensive model tokens merely because a model could perform it.

If state has not changed, Beem may reuse it within the declared freshness rules.

If only a small part changed, delta-hydrate that part.

A high-consequence route cannot under-hydrate merely because the account's usage budget is low. The route holds or requests additional capacity/state.

## 38. Operating modes

Beem supports several service modes over the same contracts:

- CSR-operated managed service;

- operator-assisted Beem;

- customer-operated SaaS;

- hybrid agentic managed mode;

- higher-autonomy mode for explicitly approved operation classes.

Those are operating modes, not separate product forks.

The first commercially useful Beem can be operator-assisted. Durable product state, evidence and control built during managed delivery must remain reusable as automation deepens.

## 39. Product phases at canon level

Detailed sprinting belongs in the Build Specification. At product level, the progression is:

### Foundation

Consolidate the Beem/Beem acquisition intelligence trunk, rights-gated neutral donor-substrate work and quarantined legacy operational donor donor references into one Beem-controlled estate. Prove reproducibility, identity, state, BLCP contracts and tenant safety.

### Phase One — governed commercial loop

Prove one named Account from qualified state through forecast/opportunity, WorkPacket, exact bounded operation, independent observation, revenue/commercial re-entry and Plan update.

Beem acquisition intelligence is the first major specialist capability. Minimum CRM/revenue state is present. Beem mobility capability is bounded. external provider network may be manual/shadow unless verified.

### Phase 1.5 — operator-assisted commercial delivery

Use the Phase One product to deliver real accounts with human supervision, support, billing, cost-to-serve and commercial evidence while deeper automation is still being built.

### Phase Two — durable agentic orchestration and adaptive recipes

Add persistent Objectives, Plans, WorkGraphs, durable waits, schedules/events, retries/compensation, multiple specialist capabilities, RecipeRuns, Opportunity Horizons, compiled workspaces, bounded automations and outcome-driven replanning.

### Phase Three — platform scale

Add self-service onboarding, broader provider coverage, Recipe Studio, curated recipe sharing, deeper external provider network portfolio bridges, optional marketplace/vertical packs and scalable commercial operations after the core route is proven.

## 40. Deferred and explicit non-features

The following do not block the first Beem release:

- a public no-code builder;

- a broad open vertical SDK;

- an open recipe marketplace;

- arbitrary AI-generated production code;

- a proprietary replacement for every CRM/CMS/ads/email/dispatch/payment system;

- a universal cross-company governance platform;

- unrelated external governance runtimes or other product programmes;

- blanket autonomous corporate access;

- unverified external provider network interoperability;

- unsupported scientific-validation claims;

- copying donor customer data into Beem;

- silent live dependency on legacy operational donor or any donor substrate.

## 41. Current implementation estate at this canon

Current Git evidence places the product consolidation in:

canonical Beem repository

Current consolidation branch:

current Beem consolidation branch

The branch combines:

- the Beem/Beem acquisition intelligence application estate;

- the accumulated rights-gated neutral donor-substrate branch stack;

- current Beem/BLCP repository authority;

- quarantined legacy operational donor foundation references under legacy donor area/;

- provenance/disposition controls.

The legacy operational donor donor remains pinned at the inspected donor head and is not a live dependency.

Beem mobility capability remains separate for a bounded capability pass.

This repository evidence is a build baseline, not proof that the combined system is integrated, deployed or production-ready.

## 42. Maturity and evidence language

Every material capability must use explicit maturity labels:

- PLANNED;

- SPECIFIED;

- SCAFFOLDED;

- IMPLEMENTED;

- UNIT_TESTED;

- CONTRACT_TESTED;

- INTEGRATION_TESTED;

- NEGATIVE_PATH_TESTED;

- STAGING_DEPLOYED;

- PRODUCTION_DEPLOYED;

- OPERATIONALLY_EXERCISED;

- COMMERCIALLY_VALIDATED.

No later state is inferred from an earlier state.

A plan is not implementation. Code is not deployment. Deployment is not operational proof. A customer conversation is not a signed agreement. A scenario is not a forecast. A forecast is not a guarantee.

## 43. Phase One product acceptance

Phase One product success means one named Account can demonstrate:

- source admission and identity;

- explicit unknown/stale/conflicted state;

- minimum sufficient hydration;

- a versioned forecast or measurable baseline;

- acquisition intelligence, CRM and mobility or another specialist observation;

- Account Manager explanation;

- candidate Plan/WorkPacket;

- CSR/tenant policy and authority resolution;

- exact-operation binding;

- execution through one registered capability or controlled manual bridge;

- receipt separated from outcome;

- independent external/commercial observation;

- reconciliation and exception ownership;

- Account and actuals re-entry;

- forecast/Plan update from measured state;

- replayable evidence.

## 44. Phase Two product acceptance

Phase Two product success means one Objective produces:

- a versioned Plan;

- multiple viable horizons where applicable;

- a durable WorkGraph;

- at least two specialist capabilities;

- a wait, event or approval state;

- one exact bounded operation;

- observed and reconciled outcome;

- a new Plan version;

- an updated Recipe/Workspace projection where relevant.

The same route must behave safely through worker restart, duplicate event, revoked authority, changed payload, stale state and provider timeout.

## 45. Golden product tests

Before broad autonomy, Beem must demonstrate at least:

- the same recipe can compile materially different workspaces for two operators without a code fork;

- missing state produces a precise request rather than invented assumptions;

- provider acknowledgement cannot mark an operation complete without observation/reconciliation;

- the same material input and recipe/version can reproduce the material decision within declared deterministic boundaries;

- Recipe v2 cannot silently alter an active v1 run;

- Tenant A cannot hydrate Tenant B;

- an unavailable connector produces a real fallback, not false completion;

- payment/booking retries are idempotent;

- usage/token limits cannot weaken mandatory evidence/control;

- an exported recipe contains no customer data or inherited customer authority;

- provider-native truth wins inside the provider's declared scope;

- consequential model output cannot execute without the required binding;

- a real outcome changes the next horizon rather than the system blindly continuing the old plan;

- the user can see what Beem knows, inferred, lacks, recommends and will change;

- cross-tenant read/write/evidence/replay is denied;

- stale or materially changed state invalidates old operation bindings;

- an AccountAgent cannot widen its own authority;

- replay cannot invoke live side effects;

- an unverified external provider network/Beem mobility capability function cannot be presented as supported;

- a paused, expired or revoked automation cannot continue.

## 46. Developer non-drift rules

Every contributor and coding agent must preserve the following:

- Beem is the product.

- BLCP is the Beem control plane.

- No required dependency on an unrelated external governance runtime.

- Beem acquisition intelligence is specialist intelligence, not authority.

- Donor substrate supplies mechanics, not Beem meaning.

- legacy operational donor is a quarantined donor, not a live dependency.

- Beem mobility capability is a bounded capability track.

- external provider network is an external capability/provider boundary.

- AI output is candidate state.

- Forecast is candidate analytical state.

- Role/access is not exact consequence authority.

- Capability is not permission.

- Approval is not a blanket future grant.

- State may transmit; authority and consent do not silently transmit.

- Exact material operations are separately bound.

- Provider ACK is not verified outcome.

- Unknown remains unknown.

- Missing state is requested, never invented.

- Account Manager cannot mint authority.

- Replay is side-effect free.

- Recipes never carry customer data or customer authority.

- Compiled workspaces use approved components, not arbitrary generated production code.

- New donor code requires provenance, disposition, rights and destination-side tests.

## 47. Supersession and source schedule

This canon is a reconciliation of the current owner-directed Beem route, current Git evidence and the supplied Beem working materials.

Controlling product interpretation used here:

- the current Beem boundary and donor-harvest control;

- BEEM_CSR_PHASE_1_AND_PHASE_2_FULL_BUILD_PLAN_v0_1 — registered Beem working build owner, subject to its current owner amendment;

- BEEM_FULL_BUILD_PLAN_PHASE_1_TO_AGENTIC_ORCHESTRATION_v0_2.md — later working build synthesis;

- the current post-donor Phase One working build specification supporting the BLCP architecture;

- Beem_PreBuild_Delta_Review_v0.1.docx and Beem_PreBuild_Delta_Register_v0.1.xlsx — working delta material promoting forecasting, sell-through, BLCP contracts, connector and truth boundaries;

- BEEM FUNCTIONALITY HYDRATION SPEC(1).txt — adaptive Recipe Runtime / hydration / workspace build direction, incorporated here at product-canon level while the open marketplace and broad no-code layer remain deferred;

- Beem musings.txt — product/use-case synthesis used where consistent with the current boundary;

- current consolidated Git repository evidence.

Superseded within Beem scope:

- earlier Beem architecture that required a separate external governance runtime;

- earlier cross-product comparison material that narrowed Beem below the current product direction;

- older build-control wording that exposes unrelated programmes or treats donor architecture as Beem product meaning.

Commercial context such as the CSR/external provider network customer-continuity and growth proposal remains private working commercial material. It may inform launch and integration planning but does not silently become product capability, signed terms, API entitlement, revenue guarantee or implementation proof.

## 48. Open boundaries that the Build Specification must resolve

The product canon intentionally leaves certain implementation and commercial decisions for the companion Build Specification or explicit owner closure:

- canonical long-term repository owner/name after the consolidation branch is accepted;

- exact donor rights/assignment/licence status;

- table-by-table legacy operational donor schema disposition;

- first live CRM/system-of-record choices by field;

- initial forecast horizon and metric set;

- first bounded write operation;

- first Beem mobility capability operations to enable;

- auth/service identity standard;

- internal SLOs and support ownership;

- retention schedule and privacy owner;

- external provider network API/add-on rights and production capability;

- production hosting/database/domain/billing/comms/model ownership;

- first pilot Account;

- named Phase One acceptance owners.

Open implementation choices do not weaken the product locks in this canon.

## 49. Final product statement

Beem is not another suite of boxes and it is not a model with ambient access to customer software.

It is an adaptive commercial operating environment.

It knows what business it is operating for. It knows which state is authoritative, current, missing or conflicted. It can preserve multiple viable next moves. It can compile the workspace and operating recipe appropriate to the objective. It can coordinate specialist intelligence, CRM, mobility, communications, websites, payments, humans and external providers. It can execute bounded work when the exact authority exists. It can stop when the required state or permission does not exist. It observes the result rather than assuming success, and it feeds measured reality into the next forecast, plan and recipe run.

That is the product the Beem codebase is being built to become.
