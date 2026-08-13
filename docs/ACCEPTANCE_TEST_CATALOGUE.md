# CSR/Alembee Acceptance and Conformance Catalogue

## Test evidence contract

Every test record includes ID, requirement/source, fixture and tenant, environment, commit SHA, schema/policy/pack version, preconditions, action, expected state/events/receipts, actual result, evidence link, reviewer and rerun/rollback instruction. Passing unit tests cannot substitute for migration, adapter, security, staging or operating evidence.

## A. Identity, tenancy and authority

- **TEN-001:** two tenants use identical external IDs; reads and writes remain isolated.
- **TEN-002:** privileged actor supplies another tenant/site ID; route rejects and records security event.
- **TEN-003:** worker starts without service identity; no action or data access occurs.
- **TEN-004:** replay from tenant A requests tenant B evidence; blocked.
- **AUTH-001:** grant consumed with different payload, target, operation, environment or tenant; rejected.
- **AUTH-002:** expired/revoked grant reaches adapter; rejected before side effect.
- **AUTH-003:** agent attempts to raise its own spend/capability; blocked and escalated.
- **AUTH-004:** proposal-only event reaches execution; rejected.

## B. WorkPacket, events and replay

- **WPK-001:** required envelope field missing; packet cannot advance.
- **WPK-002:** duplicate idempotency key; one canonical transition and a duplicate receipt.
- **WPK-003:** material upstream evidence changes; downstream derivatives invalidate.
- **EVT-001:** out-of-order/duplicate event; read model converges deterministically.
- **RPL-001:** replay reconstructs state/decisions without production credentials or side effects.
- **RPL-002:** archived schema/policy/pack version unavailable; replay reports typed gap instead of substituting current rules.

## C. AISO conformance

- **AISO-001:** admitted chauffeur site completes five modules and exactly five pillars.
- **AISO-002:** motor-coach and mixed-fleet fixtures preserve conditional requirements.
- **AISO-003:** pillar count four or six; appraisal rejected.
- **AISO-004:** missing module/source hash; appraisal rejected.
- **AISO-005:** overview strategy attempts raw website/module access; lineage violation.
- **AISO-006:** proposal adds claim/deliverable absent from accepted strategy; rejected.
- **AISO-007:** final package count not exactly three or accessibility/rendering fails; QA fails.
- **AISO-008:** recruiting/candidate/applicant/jobs/ATS content appears; contamination fails.
- **AISO-009:** unverified analytics/search/CWV/CRM/booking is scored as observed failure; rejected.
- **AISO-010:** unsupported ranking/traffic/lead/booking/revenue/ROI outcome appears; claim gate fails.
- **AISO-011:** package lacks score-profile, unknown and why-not rationale; cannot accept.
- **AISO-012:** tenant/site/source/consent/idempotency missing from CRM handoff; rejected.
- **AISO-013:** repair at stage N leaves later artifacts valid; test fails.

## D. Vertical pack and catalogue

- **PACK-001:** pack alters core stage/pillar/evidence/authority; publication rejected.
- **PACK-002:** contradictory conditional rules or schema version; compiler fails deterministically.
- **PACK-003:** prompt requests secret, unapproved tool/source or downstream artifact; compilation rejected.
- **PACK-004:** price/inclusion differs from bound catalogue; proposal rejected.
- **PACK-005:** pack revoked between approval and execution; current route re-evaluates.
- **PACK-006:** pack conformance passes without domain/pilot evidence; label cannot exceed `TESTED`.

## E. CRM migration and operation

- **CRM-001:** approved account/contact/opportunity/activity mappings reconcile counts and relationships.
- **CRM-002:** candidate/CV/document data lacks approved purpose/retention; migration blocked with discrepancy.
- **CRM-003:** source and target tenant differ; migration fails closed.
- **CRM-004:** duplicate AISO lead event; one contact/opportunity transition.
- **CRM-005:** ATS role/route/report/navigation/seed object reachable; release fails.
- **CRM-006:** CRM attempts to change payment/provider truth outside bound packet; rejected.
- **CRM-007:** rollback restores pre-migration state and preserves migration evidence.

## F. Mobility, quote, payment and communications

- **MOB-001:** missing licence/permit/insurance/capability; `ComplianceHold`, no allocation.
- **MOB-002:** credential expires after approval; execution re-evaluates and stops.
- **MOB-003:** request missing passenger/accessibility/capacity detail; visible unknown, not guessed.
- **QTE-001:** accepted quote payload changes; original authorisation invalid.
- **QTE-002:** brand/customer-of-record/provider roles conflict; quote held.
- **PAY-001:** duplicate PSP webhook; one transition and duplicate receipt.
- **PAY-002:** unauthorised refund; held for finance approval.
- **COM-001:** AI draft attempts direct send; blocked.
- **COM-002:** suppressed/unsubscribed contact enters send queue; rejected and compliance event.

## G. Provider and FullSteam

- **PRV-001:** unverified function requested; typed unsupported/unverified and no call.
- **PRV-002:** provider accepts request then times out; state `UNKNOWN`, reconciliation case created.
- **PRV-003:** provider observation contradicts CRM projection; provider truth wins and discrepancy is visible.
- **PRV-004:** duplicate/out-of-order webhook; idempotent convergence.
- **PRV-005:** stale capability/availability used in quote/dispatch; held or refreshed under policy.
- **PRV-006:** provider `200` without observation; RouteLog remains attempted/unknown.

## H. Channel execution and prospecting

- **CHN-001:** acquisition score attempts CMS publish without work packet/proof/approval; blocked.
- **CHN-002:** paid-media action exceeds spend/audience/creative grant; blocked.
- **CHN-003:** Google Ads dry-run or Meta/LinkedIn stub presented as live; conformance fails.
- **PRO-001:** prospect lacks permitted purpose/contact route; no outreach.
- **PRO-002:** expired/revoked/forwarded snapshot; access rejected.
- **PRO-003:** lightweight scan labelled formal appraisal/proposal; blocked.
- **PRO-004:** umbrella brand implies unsupported ownership/capability; claim held.

## I. Compliance and privacy

- **CMP-001:** optional tag/cookie/storage activates before consent; release fails.
- **CMP-002:** refusal produces optional identifier or network call; release fails.
- **CMP-003:** withdrawal does not propagate/delete/disable under contract; release fails.
- **CMP-004:** disclosure and observed runtime inventory differ; discrepancy blocks promotion.
- **CMP-005:** export/delete crosses tenant or omits governed data class; release fails.
- **CMP-006:** subprocessor/purpose/retention is absent for collected field; collection blocked or typed hold.

## J. Market Memory, federation and agents

- **MEM-001:** cross-client query without participation/cohort threshold; tenant-only or block.
- **MEM-002:** raw tenant evidence appears in another tenant; security failure.
- **FED-001:** enterprise request lacks local capability/credential/commercial state; no autonomous allocation.
- **FED-002:** national brand implies provider ownership or certification; held.
- **FED-003:** cross-sell based only on adjacency; remains proposal.
- **AGT-001:** second agent receives recommendation without admissible source/authority; candidate-only or reject.
- **AGT-002:** delegated envelope omits purpose/tool/audience/expiry; delegation rejected.
- **AGT-003:** human kill/revoke during in-flight task; no later consequence and receipt recorded.

## K. Reliability, security and operations

- **SEC-001:** prompt/source injection requests secret/tool/policy change; ignored, recorded and contained.
- **SEC-002:** secret appears in log/prompt/artifact; security gate fails.
- **REL-001:** database/outbox failure between state and publish; recovery produces exactly-once business transition.
- **REL-002:** webhook burst and queue backpressure preserve tenant isolation and reconciliation.
- **REL-003:** backup restore reconstructs current canonical state and RouteLog.
- **OPS-001:** exception lacks owner/deadline/re-entry; cannot leave triage.
- **OPS-002:** operator exceeds scope or uses shared broad credential; rejected.
- **OPS-003:** portfolio simulation exceeds declared capacity; cohort expansion blocked.

## Promotion suites

- **PR suite:** unit, contract, schema, lint/type/build and P0 negative tests for affected components.
- **Integration suite:** cross-repository contracts, idempotency, tenancy, migration and simulated adapters.
- **Controlled staging:** real owned accounts/sandboxes, observation/reconciliation, security/load, backup/rollback and accessible UX.
- **Release review:** traceability, open risks, operational ownership, support/capacity and signed decision.


