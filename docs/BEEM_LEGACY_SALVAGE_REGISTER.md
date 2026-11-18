# Beem legacy salvage, supersession and mothball register

**Authority:** This register does not define product or implementation requirements. It prevents older source material from silently replacing [Product Canon v1.0](./BEEM_FULL_PRODUCT_CANON_v1_0.md), [Build Spec v1.2](./BEEM_FULL_BUILD_SPECIFICATION_v1_2.md) and [Plan v0.3](./BEEM_PHASE_ONE_AND_PHASE_TWO_BUILD_PLAN_v0_3.md). Source-of-record map: [Drive](https://docs.google.com/document/d/1IX3wS33b3JxupcdyFVaOVhZH2QkMU62bCPxiGweWTT4/edit).

## Superseded documents — retained as provenance, not deleted

| Prior source | Current replacement | Salvage / action |
| --- | --- | --- |
| Beem Build Specification v1.0 (this repository docs/BEEM_FULL_BUILD_SPECIFICATION_v1_0.md) | Spec v1.2 | **MOTHBALLED.** Keep historical path and Git history; no developer links from active README. Carry forward generic controls, tests, marketing execution, phases through v1.2. New v1.2 LA, FAR, mobility, authorisation and transport scope controls. |
| Build Specification v1.1 (Drive archived) | Spec v1.2 | Code mode, operation-scoped capability discovery, plugin/MCP/API/SDK semantics were absorbed into v1.2. Do not create third specification. |
| Beem Phase One/Two Plan v0.1 and v0.2 (Drive archived) | Plan v0.3 | Phase split, P1 controlled commercial proof and P2 durable Account Manager survive via v0.3. New P1.5B LA read-only / P1.5C FAR and P2.9 FullSteam expansion are controlling. |
| Find a Ride canon v0.1 | FAR canon v0.2 | Retain source evidence, luxury/occasion use-case provenance; use v0.2 for EMBED, CENTRAL, modes, partner gates and rotation. |
| Alembee / CSR Suite / Beem GIA-dependent placeholder | Product Canon / Spec v1.2 and BLCP boundary | Historical naming and optional engineering patterns only; **no Beem-facing GIA runtime dependency**. |
| Older Developer Handover v1.0 | This README and current spec/plan | Salvage clean-clone baseline receipt, authority stopping conditions, and parallel non-consequential work. Replace stale v1.0 authority pointer. |
| Old CSR-BUILD planning package (see PROVENANCE_STATUS.md, commit `0f4d3ed87c37c92ab074b96f713318180f86d9f7`) | Product Canon / Spec v1.2 / Plan v0.3 | Historical requirements, test fixtures and migration concerns may be inspected only as provenance. Reject conflicting semantics and verify any apparent missing requirement before promoting it. |

## Candidate supplementary source material — not automatically product law

- Beem × FullSteam Blueprint, FullSteam Portfolio Map, Find a Ride Inputs, FullSteam Ask Register, Counsel Check Register.
- Beem Code Mode Orchestration Canon v0.1: **absorbed into build spec**. Preserve only as explanatory donor.
- Connector and Interface Architecture Proposed Addendum v0.1: **proposed, not adopted**; useful for typed interfaces only where consistent with v1.2.
- Minimum Input Booking Copilot v0.1 and Vehicle Taxonomy Canon v0.1: **candidate extensions, not deployed**. Keep authorisation, native operator booking ownership and full fail-closed validation.
- AImon Full Canon: **restricted Curtis research**, not an operative Beem developer specification.
- CDHQ, CGS, FAR and GPTO repositories: implementation/donor evidence, not build authority.

## Salvage matrix — no silent loss

| Capability or concern | Controlling current home | Verification required |
| --- | --- | --- |
| Core Account, AccountPlan, WorkPacket, BLCP, exact-operation policy | Product Canon / Spec v1.2 Parts II–V | Tests, failure paths, tenant isolation, actual implementation state |
| Bounded code mode and portable plugins / MCP / API / SDK | Spec v1.2 §§6.8, 34A–B, 83A, 84A; Plan P1.5A | Scoped manifests; admission vs permission; non-bypass; host parity |
| AISO/GPTO, website/marketing/CRM execution | Spec v1.2 §§37A–42; Plan P1.4–P1.7 | Code donor provenance, operator consent, measured outcome |
| LA data, trip status, provider authorisation and Ground Supply Adapter | Spec v1.2 §§15A, 16A, 35A–B; Plan P1.5B/P2.9 | Customer/partner/API/MCP rights and available provider operations |
| FAR EMBED / CENTRAL, Mode H / H+ / S / O, airport premium, rotation | Spec v1.2 §84B; FAR canon v0.2; Plan P1.5C | Operator gates, expiry, handoff, attribution and LA no-competition |
| CareerDriver plug-in boundary | Spec v1.2 §84C | Select in-Beem modules; BPO and applicant tracking stay outside |
| Lana as potential LA assistant capability | Integration note (research only) | FullSteam official technical permission and controlled sandbox proof |
| Forecast, Recipes, WorkGraph, autonomy, Workspace Compiler | Spec v1.2 Parts IX–XII; Plan Phase Two | Versioning, no authority transfer, outcome re-entry |
| Privacy, migration, resilience, evidence and operational proof | Spec v1.2 Parts XIII–XXIV | Complete negative paths, rights, replay, release evidence |

## Repository donor rule

For each module: source repository, commit SHA, path, legal rights, exact implementation state, KEEP/ADAPT/RETIRE decision, Beem target API, tests, provenance and rollback. Do not merge entire repositories or copy secret/client production data. The `mattrose271/Alembee-cdhq` donor needs a freshly proven isolated non-client snapshot before any reuse. Current CGS/TAIGC boundaries exclude live cross-product runtime and inherited authority.

## Closeout condition

Nick can derive tickets from the current canonical files without seeing older versions as active. Genuine omissions discovered in old sources are recorded as a **proposed canon/spec delta** for owner approval, not silently imported into Beem scope. Old files remain retrievable for audit and are labelled superseded. No production deployment or repository merge is implied.
