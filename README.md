# CSR-BUILD — Beem by CSR build control

This repository is Beem's build-control/documentation home, **not proof of a deployed Beem runtime**. Source of record is the [Beem pinned Drive map](https://docs.google.com/document/d/1IX3wS33b3JxupcdyFVaOVhZH2QkMU62bCPxiGweWTT4/edit), rechecked 18 November 2026.

## Current developer read order

1. [Beem Full Product Canon v1.0](./docs/BEEM_FULL_PRODUCT_CANON_v1_0.md) — Beem product meaning and invariant laws. [Drive source](https://docs.google.com/document/d/1dfUt9XutXV8SdyQfADocRRlexfYx_tWAHarL3Ob6hPI/edit).
2. [Beem Full Build Specification v1.2](./docs/BEEM_FULL_BUILD_SPECIFICATION_v1_2.md) — **current candidate implementation specification**; supersedes the repository's old v1.0 pointer. [Drive source](https://docs.google.com/document/d/1dCNjPZW3zjNObHZQtCzGDFpKclTj6Hbfw6YYwtc8IU8/edit).
3. [Beem Phase One / Phase Two Build Plan v0.3](./docs/BEEM_PHASE_ONE_AND_PHASE_TWO_BUILD_PLAN_v0_3.md) — **current candidate sequencing companion** subordinate to Product Canon and Build Specification. [Drive source](https://docs.google.com/document/d/1sUfSwkGdGVmRNyaxGrG_m2J8WETQOOLZMJ06p6yfjK4/edit).
4. [Find a Ride Everywhere Canon v0.2](https://docs.google.com/document/d/1p4lH0cOnKCilD0iEAI0RISpWN8h_mmR_7WJmW0lyUC8/edit) — current candidate mobility/distribution product lane, subordinate to Beem semantics.
5. [FullSteam Ask Register](https://docs.google.com/document/d/1CRdRUECvHms-V2_hbHbI-6tUv13Ekx0NYYK8tNHfcK4/edit) and Counsel Check Register — open partner/rights gates. These are not confirmed technical entitlements.

**Authority rule:** The Product Canon defines what Beem is. The v1.2 specification defines how to build it. Plan v0.3 orders dependent work; it does not create competing product law. Candidate label denotes a source that is current in the pinned map, **not** evidence of deployment, signed API rights or an adopted FullSteam contract. The Google Docs are the controlling source if text extraction in GitHub differs.

## Architecture and implementation boundaries

Beem owns Account, AccountPlan, WorkPacket, Beem Local Control Plane (BLCP), identity/tenant isolation, state admission and minimum hydration, exact-operation permission, capability routing, receipts, observation, reconciliation, re-entry, forecasts, CRM/revenue, Account Manager/AccountAgent, Recipes and workspaces. Model output, code-mode admission, plugin authentication and connector availability never grant authority.

Keep Limo Anywhere and FullSteam as the provider-side record for inventory, quotes, reservations, dispatch, trip messaging and payments. The initial Beem connector is **read-only and operator-authorised**. Use the Ground Supply Adapter as a typed provider abstraction. Provider write paths require explicit rights, operation binding and acceptance tests.

Use a **single Beem capability-graph/plugin/MCP/API/SDK contract** for internal model clients and outward interfaces. Separate (a) Beem exposing governed capabilities from (b) inbound FullSteam/LA integration. Lana is a candidate specialist assistant at the LA boundary; **do not assume official Lana API, MCP tool schemas, scopes or delegation** until FullSteam supplies evidence. See [Lana and FullSteam integration reconciliation](./docs/LANA_FULLSTEAM_INTEGRATION_NOTES.md).

## Phases (dependency sequence, never a staffing schedule)

- **Foundation and Phase One:** repo/rights baseline; tenant Account; qualified state, provenance and hydration; WorkPacket and BLCP; typed capabilities, bounded read/candidate code; AISO/GPTO; read-only LA; Find a Ride EMBED and Mode H; controlled CMS and CRM/revenue loops; receipt-to-observation-to-re-entry proof.
- **Phase Two:** durable objectives, workflows, monitoring, planning, forecasts, Recipes, multi-capability orchestration, autonomy settings, FullSteam expansion through supported adapters, and verified feedback to plans.
- **Product access finish:** Beem UI, approved API/SDK, plugin and MCP surfaces expose the same control semantics; demonstrably safe agentic operation. Find a Ride's own three distribution stages are separate from Beem's two architecture phases.

## Existing code and donor control

- [CSR-BUILD](https://github.com/simoncurtis13/CSR-BUILD) owns build-control documents, not runtime.
- [CSR-Beem-AISO-suite](https://github.com/mattrose271/CSR-Beem-AISO-suite): GPTO/AISO dashboard, Black Box, shared libraries and database tooling; verify and adapt before integration.
- [far](https://github.com/mattrose271/far): Find a Ride web and orchestrator donor; do not assume deployed integration.
- [Alembee-cdhq](https://github.com/mattrose271/Alembee-cdhq): **quarantined donor snapshot only**; rights and live-client separation must be proven before harvesting.
- Conversion CGS source: **read-only engineering donor** subject to licence, scope, version and Beem-side tests; CGS is not Beem BLCP or a live dependency.
- Other product/research repos are not automatically Beem donors. Rights and exact provenance control.

Before turning the scope into tickets, read [Legacy salvage and archive register](./docs/BEEM_LEGACY_SALVAGE_REGISTER.md) and [Provenance status](./docs/PROVENANCE_STATUS.md). Historical v1.0 specification stays in Git history and under the docs path as **mothballed provenance**; do not treat it as current just because it remains accessible.

## Engineering first handback

Return a pinned commit/branch, clean install/build/test results, service/deployment/credential inventory, current migration schema, external write paths, rights status, component maturity/evidence map, and divergence list against the current Drive spec. No dates, resource assignments, or duration targets are dictated by this repository.
