# BEEM PHASE BUILD PLAN V0.3 — DRIVE SOURCE REPRODUCTION

> Source of record: https://docs.google.com/document/d/1sUfSwkGdGVmRNyaxGrG_m2J8WETQOOLZMJ06p6yfjK4/edit
> Status: CURRENT CANDIDATE / RESTRICTED per Beem pinned map (28 October 2026).
> This is an unedited text extraction of the Drive document. Original Drive document controls formatting and any discrepancy. No new owner decision or technical integration is asserted by this copy.

BEEM / CSR: PHASE ONE AND PHASE TWO BUILD PLAN v0.3

Changelog v0.2 to v0.3 (27 Oct 2026). Label: CANDIDATE / RESTRICTED. CSR and Beem lane only. Built from Plan v0.2 (1OLwBC, kept as SUPERSEDED provenance) and the 26 Oct appraisal, with Si's 27 Oct decisions. No dates or KPIs added.

Header: the plan is the sequencing companion to Spec v1.2, not a planning authority (C4).

Former §4 and §8 moved to Annex D (donor provenance) (expansion 17). §12 cross-lane source reference neutralised.

New P1.5B read-only Limo Anywhere connector with AuthorisationRecord (expansion 1; C11).

New P1.5C Find a Ride Phase 1 surfaces: EMBED, Mode H hand-off, round robin, PartnerGate, Airport Premium, AISO airport pages, Savvy link, consent-gated SMS.

P1.5 builds contracts for all marketing families and activates only those the proofs need (C9). P1.5A code-mode phase split (C5).

P1.6 adds a second proof loop on LA trip data (expansion 16). "Bounded external pilot" becomes "first external reference Account".

5.13 navigation follows Spec §53 (C10). 5.14 adds the forecast baseline (C7) and LA, rotation and SMS acceptance items.

P2.7 points to the autonomy levels now in Spec §59. P2.8 requires three capability classes (C8).

P2.9 (§6.12) rewritten as FullSteam Phase 2 adapters. P2.10 adds Phase 3 doors.

§9 points to the Spec §8 tree instead of restating it (C6).

Update 27 Oct 2026 (Si t362u, t363u): P1.5C adds the Savvy referral fee switch (off by default), the approved LA Plus floor with Black preferred, and the CD plug-in and connector (BPO and CDAI servicing outside Beem). Louisville and Savvy are design references only; no outreach is planned. Companion documents are the FullSteam Ask Register (living, INTERNAL DRAFT, NOT SENT) and the Counsel Check Register (living).

Update 27 Oct 2026 (Si t359u, t360u, t361u): economics of record is Version 4 (draft agreement §8.b, 60% CSR / 40% LA on LA-linked customers only); CSR trades under the Conversion brand and delivers "Conversion Beem" full service at launch (working name); the January Beem tech in Spec v1.2 is the FullSteam ROFR scope; the Premium gate in P1.5C has no vehicle age ceiling; the round robin offers priced jobs with no quoting step and a non-extendable acceptance window (t361u).

Em dashes replaced (27 instances).

Update 27 Oct 2026 (Si t367u, second Lyft batch, CANDIDATE): P1.5C adds the Occasion requirements filter on the RotationPool (FA-49), the Airport Premium named service owner and post-service record (FA-50), a status-only host view for hotel, venue and FBO hosts, and operator airport content templates in AISO pages; 5.14 adds one acceptance line. Sources: Lyft framework v6.0 and Lyft strategy v4.0 (index: CSR folder "Lyft Airport Context (Ken)" 1WLviq8cMtLNhLmC0SJTuhg42xZWreYiN). No pilot, KPIs or dates added.

Status: WORKING PRODUCT / BUILD SPECIFICATION: UPDATED FOR BLCP, CODE-MODE ORCHESTRATION AND PORTABLE INTERFACESPurpose: Preserve the current two-phase Beem programme while incorporating the latest Beem Local Control Plane position, bounded code-mode orchestration, typed capability discovery and portable plugin/MCP/API/SDK interface concepts into the Beem build plan itself.Authority: This document is the sequencing companion to Beem Full Build Specification v1.2 and is subordinate to it. It is not a source of product truth. It does not replace the current Beem Product Canon or Full Build Specification. Where wording conflicts, the current Beem Product Canon and Full Build Specification control. Earlier Beem-facing GIA dependency language is superseded by the current BLCP position.

1. Executive decision

Beem should be built and communicated as two deliberate phases.

PHASE ONE: BEEM GOVERNED COMMERCIAL OPERATING FOUNDATION

Phase One creates the working Beem product foundation: one tenant-isolated Account, one governed state model, one AccountPlan, one WorkPacket route, the CSR-owned Beem Local Control Plane (BLCP) for qualification, policy, authority, exact-operation binding and consequence control, bounded capability execution, typed capability discovery, AISO/GPTO converted into specialist capabilities, evidence/receipt/re-entry, and a first real closed commercial loop.

Phase One must be useful in its own right. A customer or CSR operator should be able to connect an account, understand current state, ask questions against governed current information, receive candidate recommendations, prepare or approve bounded work, execute permitted changes through registered capabilities, and see what actually happened.

Phase One is not merely infrastructure and it is not a stripped-down chatbot. It is the first operational form of Beem.

PHASE TWO: BEEM AGENTIC COMMERCIAL ORCHESTRATOR

Phase Two adds the persistent objective, planning, workflow, automation and long-running agentic application layer above Phase One. The Agentic Account Manager moves from a governed interface that helps a user operate the account into a durable commercial operator that can maintain objectives over time, decompose work, monitor events, choose candidate capabilities, request missing state, prepare WorkPackets, seek approval or authority where required, execute bounded work that is already permitted, observe outcomes and re-plan from measured state.

Phase Two is therefore an extension of Phase One, not a second architecture.

The simplest relationship is:

Phase One: Connect the business, establish governed state and control, prove bounded commercial action and measured re-entry.

Phase Two: Give Beem persistent objectives and controlled autonomy so it can manage the work over time.

2. Why the two-phase structure matters

The current Beem build plan already contains both foundation work and the later Account Manager/orchestration runtime. Separating them into Phase One and Phase Two improves delivery discipline and creates a clear commercial proof point before long-running agentic behaviour is introduced.

The split also mirrors the useful strategic pattern in the Conversion programme without making the products the same. For Conversion, CGS is the governed substrate and the proposed Governed Recruiting Orchestrator is the vertical operating application above it. For Beem, Phase One combines the CSR-owned governed substrate/control route with Beem’s first commercial operating product, while Phase Two adds the persistent orchestration and autonomy layer required to turn that foundation into a general agentic commercial operating system.

This sequencing avoids two dangerous mistakes.

First, Beem must not wait until Phase Two to become properly controlled. Current-state qualification, minimum hydration, policy, authority, exact-operation binding, capability eligibility, bounded execution, receipts, observation, reconciliation, re-entry and non-bypass are Phase One BLCP requirements.

Second, Phase One must not attempt to build every future autonomous workflow, capability, vertical and UI surface before proving one end-to-end commercial loop.

3. Non-negotiable architecture across both phases

The governing Beem route remains:

observe -> qualify state -> understand objective -> hydrate minimum sufficient context -> diagnose/plan -> candidate work -> BLCP policy/authority -> exact operation binding -> bounded capability execution -> evidence/receipt -> observe outcome -> reconcile -> re-enter measured state -> learn/re-plan

The two phases differ in how much of the application/orchestration layer is automated. They do not differ in the underlying control invariants.

Across both phases:

AI output is candidate state, not authority.

BLCP qualification and policy evaluation are Beem-local control functions; neither model output, capability discovery nor program admission is customer authority or consequence permission.

A qualified or admitted state does not mean execute.

Approval is evidence/input into the authority route; approval alone does not mint complete organisational authority.

A connector or provider credential proves technical access, not permission to use every available operation.

A capability allow-list constrains execution; it does not grant consequence authority.

Material operations require an independently resolved exact-operation grant or equivalent binding before execution.

Provider acknowledgement is not verified external change.

Receipt is not observation and observation is not automatically business outcome.

State may cross a boundary; authority does not silently travel with it.

The receiver requalifies state/authority where required.

Conversation history may inform interpretation; it never outranks current authoritative state.

The Account Manager/AccountAgent can coordinate work but cannot mint, widen or inherit its own authority.

Missing state is represented as missing and must not be invented.

4. Donor provenance (moved)

The former §4 (donor programme) and §8 (external Phase Two orchestrator influence) now sit in Annex D. They are provenance, not build requirements. Beem build work does not need them.

5. PHASE ONE: Beem Governed Commercial Operating Foundation

5.1 Phase One product definition

Phase One should establish Beem as a governed commercial operating interface over a real business account.

The customer experiences one persistent Account rather than unrelated dashboards and tools. Beem can resolve current state across connected sources, explain what is happening, identify opportunities/problems, create candidate work, collect missing information, route material actions through the Beem control spine, execute approved/permitted bounded operations, and return evidence and measured state to the account.

Phase One should already feel like the beginning of a digital commercial account manager, but the human remains the principal driver of objectives and sequencing. Persistent autonomous objective management is reserved for Phase Two.

5.2 Phase One core objects

Account is the tenant-isolated operating home for organisation identity, users, services, markets, customers, claims/proof, websites, commercial channels, CRM state, enquiries, quotes, bookings, payments, capacity, partners, budgets, policies, current work, risks, evidence, observations and outcomes.

AccountPlan is the versioned commercial programme holding objectives, markets, offers, audiences, channel allocation, approved claims, proof gaps, budgets, target journey states, active campaigns/work, capacity assumptions, risks, review cadence and success measures.

WorkPacket is the common application-to-consequence unit. It carries the reason/objective, evidence, current and missing state, candidate plan or artifact, consequence class, target, capability, BLCP qualification/policy result, authority/approval requirement, exact-operation binding, execution attempt, receipt, observation, verification/reconciliation and re-entry.

Account Manager is the customer-facing interface in Phase One. It can interpret user goals, interrogate current state, explain, recommend, prepare candidate work, request missing state and route operations. It does not yet need to maintain a fully autonomous long-running objective graph.

5.3 Phase One target architecture

Customer / CSR operator↓Beem Account Manager / Work & Approvals↓Account + AccountPlan + WorkPacket↓Beem state / minimum hydration / BLCP policy / authority / exact-operation route↓Capability discovery / bounded code runtime / direct governed execution↓Typed Beem capability graph + operation-scoped manifests↓Bounded read/candidate program OR direct BLCP-bound consequential call↓AISO / AI / CMS / CRM / email / search / paid media / booking / payment / future capabilities↓Receipt -> observation -> reconciliation -> measured AccountState re-entry

5.4 Phase One workstream P1.0: rights, baseline and donor provenance

Keep the Beem repository as the product trunk. Keep CGS and all other donor estates read-only. Pin every donor source and retain package-local provenance. Resolve applicable code reuse/assignment/licence before donor-derived code is merged or deployed commercially. No donor architecture, plugin concept or code-mode implementation becomes a Beem runtime dependency merely because the pattern is useful.

Exit condition: every imported donor component has source repository, source SHA/path, destination, disposition, test status and rights status.

5.5 Phase One workstream P1.1: governed substrate integration

Complete and stabilise the reusable substrate already being staged from CGS: crypto/canonicalisation, state/version/provenance, deterministic context construction, ledger/correlation/replay, interfaces/validation, authority/control envelopes where useful, bounded execution, and selected proof/conformance utilities.

The purpose is not to reproduce Conversion CGS inside Beem. The purpose is to avoid rebuilding neutral deterministic engineering that already works.

Exit condition: promoted substrate packages build/test in the Beem monorepo with provenance preserved, and no donor terminology is silently promoted into Beem product semantics.

5.6 Phase One workstream P1.2: Beem Local Control Plane and execution spine

Implement the Beem-native BLCP control route around rights-cleared donor mechanics.

This includes CSR identity/account isolation, information-authority binding, state qualification, freshness/conflict handling, minimum-sufficient hydration, candidate-state handling, Beem policy, authority resolution, approval evidence, exact-operation binding, capability eligibility, execution grants/expiry, bounded execution, idempotency, receipts, observations, reconciliation, verification and re-entry.

BLCP is the Beem control plane. Current CGS or other donor governance may contribute neutral deterministic mechanics where rights permit, but donor semantics, permits, role names, authority models and runtime dependencies do not become Beem product law.

Exit condition: one synthetic consequential operation can be reconstructed end-to-end without relying on AISO or a model to supply authority.

5.7 Phase One workstream P1.3: Account, AccountPlan and WorkPacket persistence

Extend the existing Beem/AISO data estate rather than replacing it wholesale.

Add tenant/account membership and actor identity, versioned AccountPlan, WorkPacket, state-qualification and policy decisions, AuthorityResolution, ExactOperationBinding, execution attempt, ProviderReceipt, Observation, ReconciliationCase, Verification and ReEntryRecord relationships.

Existing AISO/site/telemetry/content identifiers should be linked into the new account/evidence model rather than discarded.

Exit condition: one Account can show current commercial state, active plan, candidate work, control decisions, consequence history and observed outcomes with tenant isolation.

5.8 Phase One workstream P1.4: AISO/GPTO as the first specialist capability family

Retain the useful existing AISO assets: website/configuration management, Black Box runtime, structured data, telemetry, materialised insights, AI-search visibility, competitor intelligence, audits, reports and content-generation capability.

Transform their operating position. AISO observes and diagnoses. It may generate candidates. It does not govern the Beem account and it does not turn an approval into a direct consequential deployment path.

AISO output should enter WorkPackets and the common control route before any material external change.

Exit condition: AISO can create an evidence-backed candidate WorkPacket while remaining clearly separate from BLCP policy, authority, exact-operation binding and consequence permission.

5.9 Phase One workstream P1.5: capability registry and first execution adapters

Create the Beem capability contract and registry.

Each material capability declares identity/version, owner/provider, supported operations, typed input/output schemas, effect class, data classification, credential/scopes, required state, consequence class, policy/authority requirements, runtime/spend/quantity bounds, retry policy, idempotency, acknowledgement semantics, observation/reconciliation route, cost/resource class, health/freshness and rollback/compensation support.

Start with the smallest set required to prove the first closed loop, likely AISO, AI generation and one real CMS or equivalent publication capability. Phase One builds the contracts for every Spec §37A marketing family (including consent-gated SMS) but activates only the families the first proofs need (appraisal C9).

Exit condition: a planner/user can select an eligible capability without receiving raw provider authority, and unsupported operations fail closed.

5.9A Phase One workstream P1.5A: capability discovery, bounded code mode and portable interfaces

Introduce a deliberately small model-facing surface over the larger Beem capability estate. Capability discovery returns only the operation-scoped typed view needed for the current objective: opaque handle, operation, schemas, effect class, source/provider identity, restrictions, freshness/version, expiry and cost/resource class. Discovery reveals a possible route; it creates no authority.For multi-step read, analysis and candidate-producing work, allow the model to write a small bounded program against only those admitted handles. Run it in an isolated sandbox with no raw long-lived credentials, no arbitrary network access, bounded CPU/memory/runtime/call count, typed proxies, program digest/run ID, explicit failure states and no scope widening. Intermediate data may remain inside the runtime so only the minimum decision-relevant result hydrates the model.Program admission and operation admission remain separate. A program may compose admitted reads, deterministic transforms and candidate production. Any material mutation, publish, send, spend, booking, payment, permission change or other consequential operation must cross the normal WorkPacket -> BLCP -> ExactOperationBinding -> capability execution boundary at the moment of consequence. Call forty does not inherit permission because calls one to thirty-nine were valid.Expose the same Beem-owned contracts through the interface that best fits the customer or host: Beem UI, plugin/MCP surface, API or SDK. These are adapters over the same operation identity, state basis, capability contract, BLCP route and receipt schema. Interface choice must not change Beem semantics or silently increase authority.Phase split (appraisal C5): the bounded runtime runs read-only in Phase One, including over Limo Anywhere reads. Outward MCP, plugin and API adapters move to Phase Two (Spec Sprint 15A). Any outward call carrying provider-sourced fields is C7 and off by default.Exit condition: one objective can discover and compose at least three read/candidate capabilities inside a bounded run; a non-admitted capability is refused; irrelevant source data stays outside model context; and an attempted consequential call is intercepted and routed through the normal BLCP exact-operation boundary.

5.9B Phase One workstream P1.5B: read-only Limo Anywhere connector

Build the Spec §35A Phase A connector and the §16A AuthorisationRecord before any LA-sourced data is used. Scope: operator account, coverage, vehicle classes, rate card or LQC reference, trips and statuses, booking channel, FlightStats outcomes, surveys, Trip Timeline (Black), compliance and vehicle evidence for gates. Per operator only, no aggregation, fail closed on revocation. Writes stay in Phase Two.

Working assumptions while FullSteam asks are open (Ask Pack FA-04, FA-12, FA-13): the operator authorises Beem through its own LA access; if wider licence coverage is not confirmed, the connector reads only what the operator exposes, and Mode H continues.

Exit condition: one consenting operator's trips, statuses and gate evidence land as Spec §15A objects with AuthorisationRecords; revocation stops reads and quarantines derived data.

5.9C Phase One workstream P1.5C: Find a Ride Phase 1 surfaces

Build the Phase 1 distribution surfaces from Find a Ride Everywhere Canon v0.2 on the luxury core: EMBED kit (link, QR, email block, site tile) routing to a Home Operator's LA surfaces (LQC, ORES, Custom Booking Portals, Passenger Link); Mode H hand-off with pre-fill where FullSteam allows (FA-02); RotationPool and sequential priced-job offers for demand with no named operator (FA-03), with no quoting step: the operator accepts or declines inside an acceptance window of 5 minutes same-day and 15 minutes future that operator settings cannot extend, and expired offers auto-advance (FA-09); PartnerGate pass-or-fail evaluation (Base, Premium, occasion gates; no vehicle age rule, which is each chauffeur company's discretion); Airport Premium surfaces and AISO airport pages (Spec §38A); Savvy link contract (inbound card-typed preferences with consent only) with the referral fee switch per partner, off by default, and the funeral-home hard block (Spec §84B); Airport Premium partner floor LA Plus, Black preferred (approved); CD plug-in and connector into Driver Readiness and operator capacity, with BPO and CDAI servicing outside Beem (Spec §84C); consent-gated SMS through Spec §37A.

Addition 27 Oct 2026 (CANDIDATE; Lyft framework v6.0 §2, §5, §7): special requirements (accessibility, child seats, luggage, group, pets, security, special assistance) are captured before routing and filter the RotationPool pass-or-fail (Spec §15A, FA-49); each Airport Premium job carries the operator's named service owner and a post-service record (FA-50); hotel, venue and FBO hosts see trip status only; AISO airport pages may use operator content templates (per-terminal and FBO arrival guides), Beem AISO only.

Exit condition: one occasion surface and one airport surface hand off to an operator's own LA booking flow with attribution, and one rotation offer is made, accepted or declined, and logged per operator.

5.10 Phase One workstream P1.6: first real closed loop

Recommended first proof:

customer account -> connected website -> AISO observation -> Account Manager explanation -> proposed source-layer improvement -> candidate artifact -> fresh state/minimum hydration -> BLCP policy/authority -> customer approval where required -> exact CMS operation binding -> bounded publish -> provider receipt -> independent website observation -> search/AI visibility measurement -> reconciliation -> Account re-entry

The point is not merely to publish content. The point is to prove the complete separation between candidate, admissibility, authority, attempted consequence, provider acknowledgement, observed external state and measured result.

Second proof loop (runs alongside the website loop): one consenting Black-tier operator -> read-only LA trips and statuses under an AuthorisationRecord -> Service Scorecard v1 for that operator only -> forecast baseline -> Account Manager explanation -> one candidate recovery or reactivation WorkPacket -> BLCP -> permitted action -> observation in LA -> reconciliation -> commercial actual -> Account re-entry.

Exit condition: both loops can be replayed and explained from source state through measured re-entry.

5.11 Phase One workstream P1.7: first CRM/revenue loop

After the website slice is sound, add enough commercial state to prove that Beem operates toward business outcomes rather than visibility metrics alone.

Introduce leads/enquiries, opportunities/quotes, follow-up state and revenue attribution as appropriate. Add one bounded customer communication or CRM action capability.

Example:

AISO identifies a high-value visibility/conversion problem -> CRM shows recoverable dormant demand -> Beem proposes a website fix plus a customer follow-up WorkPacket -> permitted operations execute -> replies/enquiries/bookings/revenue are observed -> AccountPlan progress changes.

Exit condition: at least one measured commercial outcome re-enters the Account and can change the recommended next action.

5.12 Phase One workstream P1.8: operational hardening and internal CSR use

Use CSR as the first operating account where practical.

Prove cross-tenant rejection, changed-payload re-evaluation, stale capability-manifest refusal, non-admitted capability refusal, authority expiry, idempotency, provider timeout, ACK versus observation mismatch, reconciliation, pause/kill, rollback/compensation evidence, bounded-program failure and deterministic replay where practicable.

Establish operational support states rather than treating every failure as a generic error.

Exit condition: Phase One is safe and useful enough for sustained internal operation and a first external reference Account.

5.13 Phase One customer experience

The Phase One interface should converge toward:

Home (Account Pulse)

Account Manager

Plan

Forecast

Pipeline (CRM / Revenue)

Work (including Approvals)

Acquisition (including Website / Visibility and Campaigns)

Connections

Evidence (Results)

Settings (including Policy / Authority)

Navigation follows Spec §53 (appraisal C10).

A customer should already be able to say:

“Why are enquiries down?”

“Show me what changed.”

“Prepare what we should fix.”

“Run the things I’m authorised to approve.”

“Why was that action blocked?”

“Show me exactly what happened.”

5.14 Phase One acceptance criteria

Phase One is complete only when all of the following are evidenced.

A real customer/account source can be decomposed and registered without losing provenance.

Conflicting authoritative state fails closed or enters an explicit conflict-resolution route.

Missing state produces a request/hold rather than invented state.

Conversation history cannot override newer authoritative state.

AISO/model output remains candidate until qualified.

BLCP qualification/policy remains distinct from customer authority and exact consequence permission.

A material operation cannot execute without WorkPacket plus independently resolved exact authority where required.

Changing material payload/target/state after approval forces re-evaluation.

Unsupported capability is blocked.

Duplicate invocation cannot cause duplicate business consequence.

Provider timeout produces UNKNOWN/reconciliation rather than fabricated success/failure.

Provider ACK is distinguishable from observed external change.

At least one external consequence is independently observed.

A measured result re-enters AccountState with provenance.

Ledger/replay reconstructs the route.

Cross-account/tenant access is rejected in conformance tests.

Read-only/analysis operation can remain available when consequential execution is suspended.

A forecast baseline exists and a commercial actual re-enters against it (Spec §108; appraisal C7).

Every LA-sourced record carries an AuthorisationRecord with no_aggregate; revocation fails closed and is tested.

No cross-operator view, ranking or benchmark exists without written opt-in.

Beem never executes driver.assign, dispatch.write or payment.capture; tested as negative cases.

A Find a Ride hand-off lands in the operator's own LA flow with attribution where the platform allows.

A rotation seat payment cannot change pool order; tested as a negative case.

No SMS is sent without a recorded consent for that purpose.

No rotation offer reaches an operator whose evidence does not cover the job's stated requirements; tested as a negative case (Spec §101 test 42).

5.15 Phase One commercial claim

At the completion of Phase One, Beem can credibly claim:

“Beem gives a business one governed commercial operating interface over connected business state and specialist capabilities. It can identify and prepare work, route material actions through explicit admissibility and authority controls, execute bounded permitted operations, and show evidence of what actually happened.”

It should not yet claim fully autonomous long-running commercial management.

6. PHASE TWO: Beem Agentic Commercial Orchestrator

6.1 Phase Two product definition

Phase Two turns the governed operating foundation into a persistent agentic commercial operating system.

The customer no longer has to initiate every sequence of work. They can establish objectives, constraints, budgets, approval rules and automation envelopes. The Agentic Account Manager can then monitor state, diagnose material changes, create and revise plans, manage dependencies, select candidate capabilities, request missing information, create WorkPackets, wait for approvals/events, execute work already permitted by the control route, observe outcomes and re-plan.

The customer manages outcomes and boundaries. Beem manages much more of the complexity.

6.2 Phase Two core application objects

Objective represents a persistent desired business outcome, including account, objective class, target metrics, baseline, target value/date, priority, budget envelope, constraints, applicable markets/services and lifecycle status.

Plan is a versioned candidate strategy for achieving an Objective from a defined AccountState fingerprint. A Plan may contain assumptions, missing-state requirements, work nodes, dependencies, expected effects, risks, estimated cost and candidate capabilities. A Plan is never authority.

WorkflowNode represents one unit of durable work such as observe, analyse, request state, generate candidate, request approval, execute operation, wait, verify, reconcile, notify, human task or re-plan.

AutomationDefinition is the versioned customer-configured envelope that defines trigger, evidence/source requirements, operation class, target, allowed capabilities, limits, budget, authority/approval requirements, schedule, expiry, retry policy, notifications, suspension and verification conditions.

AutomationRun is one immutable/evidenced execution instance of an AutomationDefinition version.

AccountAgent is the durable operating state of the Agentic Account Manager: active objectives, plan versions, tasks, dependencies, waiting conditions, missing-state requests, proposed capabilities, pending approvals, monitoring cadence, exceptions, failures, handoffs and re-plan reasons.

6.3 Phase Two workstream P2.0: orchestration contract lock

Define Objective, Plan, WorkflowNode, AutomationDefinition, AutomationRun, AccountAgent, planner boundary, capability-router boundary, conversation assertion model and workflow status model.

Exit condition: contracts fit cleanly around Account, AccountPlan and WorkPacket without duplicating authority or control semantics.

6.4 Phase Two workstream P2.1: durable orchestration persistence

Add persistent objectives, objective metrics, plans, workflow nodes/dependencies, automation definitions/runs, account-agent state, conversation assertions and monitoring subscriptions.

Long-running work must survive worker restart. Scheduled waits must be durable. Inbound events must be idempotent. Historical plan/automation versions must remain reconstructable.

Exit condition: an objective/workflow can pause for hours or days and resume from persisted state without depending on chat history.

6.5 Phase Two workstream P2.2: conversation and fresh-state boundary

Treat conversation as an interpretation/work surface, not SoT.

Material assertions from a conversation may be represented as user assertion, model assertion, reference to authority, qualified, unresolved, stale, superseded or conflicted.

Before each material decision or consequence, the runtime resolves the current relevant state and current governing artifacts again. Policy changes, authority changes, target changes, payload drift, provider/capability changes, consent, budgets and stale source state can all force re-evaluation.

Exit condition: a stale statement from a long-running conversation cannot resurrect an expired permission or override current authoritative account state.

6.6 Phase Two workstream P2.3: objective and planner runtime

Implement objective creation/maintenance, candidate plans, dependency graphs, missing-state requests, planner-provider abstraction, assumption tracking and plan versioning.

The planner receives minimum-sufficient qualified state, Objective, relevant AccountPlan, active work, capability summaries, constraints, budgets, missing state and recent verified outcomes.

It returns candidate Plan/work, capability requirements, state requirements, risks/uncertainty, expected effects and human questions.

The planner never returns authority.

Exit condition: the Account Manager can take a real commercial objective and produce a durable candidate workflow without executing a consequential operation.

6.7 Phase Two workstream P2.4: workflow and automation runtime

Implement durable workflow state, event triggers, timers, schedules, waits, retries, branches, failure routes, pause, cancellation, suspension conditions and AutomationDefinition/AutomationRun lifecycle.

An automation can automatically commence work. It cannot automatically enlarge its scope or grant itself consequence authority.

Recommended workflow states include DRAFT, PLANNING, WAITING_FOR_STATE, WAITING_FOR_EVENT, WAITING_FOR_APPROVAL, READY, EXECUTING, VERIFYING, RECONCILING, REPLANNING, PAUSED, BLOCKED, FAILED, UNKNOWN, COMPLETED and CANCELLED.

Exit condition: a trigger can create and progress a WorkPacket through the control route without any raw provider bypass.

6.8 Phase Two workstream P2.5: capability router and multi-provider intelligence

The planner/runtime asks the Capability Registry for eligible capability contracts rather than calling raw integrations.

Add health/availability, operation compatibility, provider/account binding, consequence class, data classification, policy eligibility, suspension state and observation support.

Create a multi-provider AI capability so OpenAI, Anthropic and future approved providers can be selected by capability, policy, data class, customer preference, jurisdiction, reliability or price without changing the governing state/authority model.

Exit condition: provider substitution does not change authority semantics or WorkPacket consequence binding.

6.9 Phase Two workstream P2.6: monitoring and re-planning

The Account Manager should not continuously call a model simply to appear autonomous.

Monitoring should primarily use structured events, scheduled checks, thresholds, objective variance, capability health, WorkPacket status and new observations. Invoke planning/re-planning when there is a material reason.

Re-plan causes include new evidence, objective variance, work failure, capability unavailable, authority changed, approval declined, state conflict, budget exhausted, external outcome, deadline risk and invalidated assumptions.

Exit condition: verified new state can deterministically cause the Account Manager to revise the plan while preserving the previous plan and evidence.

6.10 Phase Two workstream P2.7: approval, evidence and autonomy UX

Add Work queue, Approval Centre, Automations view, Evidence timeline, explain-why drawer and obvious pause/kill controls.

Expose graduated autonomy by consequence class rather than a single “AI on/off” setting.

Recommended levels are Observe, Recommend, Prepare, Approval-driven execution and Delegated bounded automation. These levels are now specified in Spec v1.2 §59 with a ceiling per consequence class; no standing C5, C6 or C7 at first.

The customer can set different levels for different operation classes. Website diagnostics might run automatically while a large paid-media budget change or partner commitment requires specific approval/authority.

Exit condition: a customer can understand what Beem is doing, what it can do automatically, what is waiting for them, why something was blocked and what happened afterward.

6.11 Phase Two workstream P2.8: first true multi-capability objective loop

Recommended objective:

“Increase profitable enquiries for a selected service while remaining inside the approved monthly commercial budget and using only current approved claims.”

Possible loop:

Objective behind target -> AISO identifies visibility/conversion opportunity -> CRM identifies dormant/recoverable demand -> Account Manager explains constraint -> planner creates coordinated candidate plan -> WorkPacket A prepares/publishes a governed service-page improvement -> WorkPacket B prepares customer follow-up -> WorkPacket C proposes paid-media adjustment if evidence supports it -> each operation resolves fresh state/admissibility/authority separately -> permitted work executes -> receipts and observations return -> enquiries/replies/bookings/revenue are measured -> AccountState and objective progress update -> Account Manager re-plans.

Exit condition: at least three capability classes (Spec §109; appraisal C8) participate in one persistent Objective and verified external/business outcomes change the next Plan.

6.12 Phase Two workstream P2.9: FullSteam Phase 2 adapters and the wider ground-transport family

Phase Two extends the Phase One LA connector into the Spec §35B Ground Supply Adapter across the FullSteam transport family, as Find a Ride Everywhere Canon v0.2 Phase 2 describes.

LA writes (C2 to C6): notes and preferences write-back, quote creation, and reservation.create only as a C6 hand-off with an idempotency key and confirmation inside LA. Each needs FullSteam's position (FA-04, FA-41 not assumed).

FASTTRAK driver: the public Partner API for coverage, quotes and hand-off (FA-35).

GroundXchange route: SantaCruz and Livery Coach operators through GroundXchange mappings, then WebConnect and GroundApp surfaces.

netPark channel: airport reservation and loyalty touchpoints with netPark operator consent (FA-36).

CENTRAL supply rails: GroundSpan for corporate and TMC demand (FA-39) and further connectors as FullSteam builds them.

FAR: used as a demand, quote and intake donor where useful; its regional "authority" vocabulary is renamed to market scope so it never collides with BLCP or customer consequence authority.

Never: dispatch, driver assignment, passenger payment, or cross-operator data use.

Entry condition: Phase One running on LA with per-operator proof, and FullSteam access to the FASTTRAK Partner API and the GroundXchange route.

Exit condition: one objective uses a second FullSteam platform through the adapter without transmitting Beem account authority into that platform, and the hand-off is observed and reconciled.

6.13 Phase Two workstream P2.10: productisation and vertical packs

Expose automation templates, conversational automation creation, connection onboarding, autonomy settings, domain/vertical packs, multi-account administration and commercial entitlements.

Own state, orchestration and governance first. Connect specialist capabilities. Replace underlying products only where there is a strong economic reason.

Trucking/recruiting can remain a Conversion specialist vertical rather than becoming Beem’s generic domain vocabulary. Other industries/functions should be additive through domain objects, capability packs, policy profiles, workflows and templates.

Phase 3 doors (secondary, after a working Phase Two): non-transport FullSteam brands (hospitality PMS, POS, winery, planner and similar) become demand doors that hand guests to the luxury transport core. Each door needs FullSteam approval for its app or API route. Gated items (Mode O, agentic channel) stay behind FullSteam permission and counsel.

Exit condition: adding a new vertical/domain does not require rewriting the generic orchestration/control runtime.

6.14 Phase Two acceptance criteria

A stale conversational fact cannot override current state.

A model-generated Plan remains candidate state.

AccountAgent cannot create or widen authority.

An AutomationDefinition cannot enlarge its own envelope.

Expired/suspended automation cannot create new consequential execution.

Changed payload/target/material state causes re-evaluation.

Technical connector permission cannot substitute for organisational authority.

Mutation is reachable only through the WorkPacket/consequence boundary.

Duplicate triggers/webhooks cannot cause duplicate business consequences.

Provider timeout produces UNKNOWN/reconciliation.

Provider ACK remains distinct from observed change.

Observed business outcome remains distinct from technical execution success.

Re-entry uses fresh measured/provenanced state and does not inherit authority.

Governance artifacts and automation definitions are versioned and auditable.

Historical workflows retain references to the policy/authority/capability versions under which they ran.

Capability discovery returns only operation-relevant typed handles, not the full capability estate.Generated code cannot access a capability that was not admitted to its current run.Program admission cannot substitute for exact-operation permission on a later consequential call.Intermediate source data can be reduced inside the bounded runtime without unnecessary model hydration.Changing from Beem UI to MCP/plugin/API/SDK does not change operation identity, authority requirements or receipt semantics.

One material Objective can be replayed from state -> Plan -> capability discovery -> bounded candidate composition where used -> WorkPacket -> BLCP policy -> authority -> exact operation -> capability -> attempt -> receipt -> observation -> reconciliation -> re-entry -> next Plan.

6.15 Phase Two customer experience

The customer should be able to say:

“We need another £400k of profitable revenue this quarter.”

“Fix the decline in enquiries.”

“Fill our spare capacity next week.”

“Follow up recoverable quotes automatically inside these limits.”

“Do everything you’re authorised to do and bring me the decisions that need me.”

“Pause all paid-media changes but keep monitoring.”

“Why did you do that?”

“What actually happened?”

“What should we do next?”

Beem should answer from the account, manage the work and preserve the evidence rather than treating each request as an isolated chat turn.

6.16 Phase Two commercial claim

At the completion of Phase Two, Beem can credibly claim:

“Beem gives a business one intelligent Account Manager across its commercial technology estate. It maintains objectives, plans and work over time; coordinates approved AI and software capabilities; executes the automations the customer has authorised within explicit bounds; measures what actually happened; and continuously re-plans from governed business state.”

7. Phase One to Phase Two handoff gate

Phase Two should not be used to hide unfinished Phase One control work.

Before Phase Two receives permission to automate consequential work, Phase One must have proven current-state qualification, minimum hydration, BLCP policy/authority separation, exact-operation binding, capability eligibility, non-bypass, idempotency, receipt/observation/reconciliation, program-boundary enforcement and tenant isolation.

However, Phase Two contract work can begin earlier in parallel where it does not create a bypass. Objective/Plan/Workflow persistence, read-only planning, monitoring and customer UX can be developed against mocked/no-consequence control ports while Phase One closes its external consequence proof.

The handoff principle is:

Phase Two may automate a route only after Phase One has proven that route safe enough to automate.

8. Donor orchestration influence (moved)

Moved to Annex D.2. Any generic component goes through the donor process in Annex D before Beem adoption.

9. Repository/build implications

The repository tree is defined once, in Spec v1.2 §8 (appraisal C6). This plan does not restate it.

Phase One primarily fills the spec's control, domain (account, planning, work, mobility objects from §15A), capability registry and first capability families (including the read-only Limo Anywhere connector), evidence packages, apps/api and the first web surfaces. The bounded code runtime lands here, read-only.

Phase Two primarily fills orchestration (objectives, planner, workflow, automation, capability search, monitoring), apps/worker, the outward interface adapters (MCP, plugin, API, SDK), the Ground Supply Adapter Phase Two drivers, and later capability and vertical packs.

The phases share one Account, one WorkPacket grammar, one capability registry and one governing control route.

10. Non-drift locks for both phases

Beem/CSR is the product.

CGS remains donor/neighbour, not Beem product authority.

Donor governance is not Beem control authority.

BLCP is CSR-owned and is the Beem control plane.

Phase Two does not replace or relax Phase One control requirements.

AISO/GPTO remains a specialist website/search/evidence/appraisal/candidate capability family.

Account is Beem’s persistent operating home.

AccountPlan is the enduring commercial programme.

WorkPacket bridges proposed work to governed consequence.

Objective describes desired outcome.

Plan describes candidate strategy.

AccountAgent manages work; it does not grant authority.

Conversation is a working interface, not organisational SoT.

Fresh governing state is resolved for material operations.

AI output is candidate.

Qualified/admitted state, capability discovery and program admission are not customer authority or consequence permission.

Approval evidence is not authority by itself.

Capability permission is not consequence authority.

Capability discovery is not capability permission.Program admission is not blanket operation permission.Generated code is an ephemeral orchestration artifact, not a durable authority object.The sandbox constrains execution mechanics; BLCP remains the consequence-control boundary.Interface portability changes transport/presentation, not Beem semantics, authority or evidence requirements.

Material consequence requires exact-operation binding and independently resolved authority.

Provider ACK is not verified result.

Re-entry is fresh measured/provenanced state.

Automations operate only inside declared envelopes and cannot enlarge them.

Governance artifacts themselves are versioned/governed.

State may cross boundaries; authority does not silently transmit.

FullSteam is a network/fulfilment capability, not Beem itself. The operator's FullSteam platform is the system of record for every ride; Beem never dispatches, assigns drivers or takes passenger money.

FAR network scope must not be confused with customer/consequence authority.

Donor code is not reusable merely because an idea is attractive; implementation reuse remains evidence/rights/disposition gated.

No feature is described as operational merely because code exists.

11. Final two-phase outcome

PHASE ONE outcome:

Beem can connect a real account, establish governed commercial state, use AISO and other specialist capabilities to observe and prepare useful work, discover only the capabilities relevant to the current objective, compose bounded read/candidate work where useful, route material actions through BLCP policy/authority/exact-operation controls, execute bounded permitted operations, and independently observe/reconcile the result.

PHASE TWO outcome:

Beem can maintain persistent commercial objectives and manage the work over time. The Agentic Account Manager can monitor the business, plan, coordinate capabilities, run customer-authorised automations, recover/re-plan and measure outcomes while never converting model confidence, retrieved information or technical access into authority by itself.

That gives Beem a clean product progression:

Phase One: Governed Commercial Operating Foundation.Phase Two: Agentic Commercial Orchestrator.

The architecture underneath remains one system.The level of persistent orchestration and delegated autonomy increases between the phases.

12. Source basis and working status

This working specification consolidates the current Beem/CSR build direction with the current Beem Product Canon and Full Build Specification, the bounded code-mode orchestration pattern, and general plugin and interface architecture concepts. It adopts the useful orchestration and portability mechanics without importing CGS or GIA as Beem runtime dependencies.

The source material supports a clear distinction: Beem is the broader CSR-owned commercial operating system; CGS and Conversion vertical applications remain separate. The reusable additions adopted here are bounded capability discovery, model-written code-mode composition, minimum-state processing, operation-boundary interception, portable plugin/MCP/API/SDK interfaces, and durable orchestration that repeatedly re-enters fresh Beem state. These are integrated as Beem mechanics under BLCP, not as imported product authority.

This document remains in Google Drive as the sequencing companion to Spec v1.2 until the Phase One/Phase Two framing is promoted into the repository build controls. It is not a planning authority in its own right.

---

Annex D. Donor provenance (moved from §4 and §8)

Kept for provenance only. Not build requirements.

D.1 (formerly §4) Relationship to the current CGS donor programme

The CGS repository remains a read-only engineering donor for Beem where rights permit. The useful donor mechanics already identified include deterministic canonicalisation/hashing, state/version/provenance mechanics, deterministic context construction, ledger/correlation/replay/trace, bounded execution, fail-closed validation patterns and selected control-envelope mechanics.

Those mechanics do not make CGS the Beem product master and do not make current CGS governance the final Beem governor.

The repository-wide KEEP / ADAPT / RETIRE rule continues to apply. Exact donor snapshots may retain legacy terms for provenance. Any new Beem-owned API, domain object, UI, planner, capability registry or control contract must use Beem semantics.

The proposed Conversion Phase Two recruiting orchestrator is immediately useful as a design donor for generic ideas such as persistent objectives, workflow graphs, automation envelopes, durable scheduling, planning, monitoring, capability routing, evidence timelines, approval UX, kill/pause controls and vertical configuration. Future Phase Two code may only become an engineering donor after it exists, is pinned, inspected, proven, dispositioned and rights-cleared.

The recruiting product, recruiting domain model, Conversion UI, Conversion tenant assumptions and CGS control adapter remain Conversion-specific.

D.2 (formerly §8) How the Conversion Phase Two work should influence Beem

The Conversion Governed Recruiting Orchestrator proposal is strategically useful because it makes persistent state, objectives, automations, agentic coordination, connected capabilities, evidence and kill/pause controls concrete in a difficult real operational vertical.

Beem should learn from that build while preserving separation.

The strongest potential future engineering donors are generic objective engine, workflow graph, durable scheduler/runtime, automation engine, planner framework, capability router, conversation working-context machinery, monitoring/re-plan machinery and generic evidence workflow.

The Conversion recruiting pack, trucking-specific object model, Conversion UI, CGS control adapter and Conversion-specific tenant/provider assumptions remain Conversion-specific.

The best future implementation shape on the Conversion side is therefore:

Generic orchestration core↓CGS control adapter↓Recruiting/trucking domain pack↓Conversion Governed Recruiting Orchestrator

If generic Phase Two components later become useful to Beem, they go through the same process as every other donor: pin exact source -> inspect -> test -> rights gate -> KEEP/ADAPT/RETIRE -> donor-clean landing -> Beem adaptation -> Beem tests.

End of Plan v0.3.