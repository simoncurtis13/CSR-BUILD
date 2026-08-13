# CSR/Alembee Cross-Repository Handover

## Integration topology

| Producer | Consumer | Contract | Authority rule |
|---|---|---|---|
| AISO intelligence | CRM | Qualified acquisition WorkPacket/event | Creates or updates candidate commercial state only; no communication/quote/dispatch authority |
| CRM | Governance substrate | Proposed state mutation or command | Canonical commercial intent; must pass tenant, policy, transition and grant checks |
| Governance substrate | GIA | Exact subject/use admission request | GIA may admit/condition/reject use; unavailable behavior is explicit |
| Governance substrate | CIG | Candidate transition envelope | CIG may admit/hold/reject transition when production-ready; no hidden bypass |
| Governance substrate | Action adapter | Signed exact command/grant | Adapter executes only the bound operation and returns receipt/unknown |
| Mobility/quote | FullSteam adapter | Versioned supported provider command | Provider remains truth owner; acknowledgement is not observation |
| Payment provider | CRM/RouteLog | Idempotent webhook/observation | Payment projection reconciles; CRM cannot overwrite provider truth |
| Every service | RouteLog/read models | Versioned event/outbox | Carries tenant, environment, correlation, causation, schema and evidence |
| Outcome/attribution | AISO/Market Memory | Re-entry packet | Corrections and learning are governed; no default cross-client leakage |

## Mandatory envelope fields

Every cross-repository request/event carries tenant, environment, actor/service identity, correlation ID, causation ID, schema version, object version, source/target IDs, purpose, payload digest, idempotency key and evidence/authority references. Consequential requests additionally carry capability, exact operation, target, expiry, receipt requirement, observation contract, discrepancy owner and rollback/compensation instruction.

## Dependency order

1. Source rights, pins and CSR technical independence.
2. Tenant/service identity and canonical objects.
3. WorkPacket, RouteLog and outbox.
4. Transition/compute decision and exact grants.
5. CRM transformation and migration.
6. AISO nine-stage route and source/proof repository.
7. Quote, payment, communication and mobility commands.
8. Provider adapter with observation/reconciliation.
9. Attribution, reporting and re-entry.
10. SaaS and agentic modes.

UI/read-model work may proceed in parallel, but a live side effect cannot move ahead of its identity, grant, receipt and reconciliation route.

## Compatibility and migration

- Contracts are versioned and additive within a supported compatibility window.
- Old GPTO headers/identities may use a time-bounded mapper; the target is CSR tenant/service identity.
- New CRM schemas are introduced beside ATS schemas; migration is explicit, tenant-bound and receipted.
- GPTO raw provenance is preserved during backfill.
- GIA and CIG ports run in shadow before switch-over.
- FullSteam/payment/comms/CMS run in sandbox or shadow before live authority.
- Every switch has rollback criteria and an owner.

## Repository owner handover packet

Each repository owner receives:

- pinned source and target SHAs;
- retained/refactored/replaced/added/verified file list;
- owned objects and APIs/events;
- incoming/outgoing dependencies and compatibility window;
- migrations and data disposition;
- secrets/accounts and environment owner;
- positive, negative, tenancy, security and replay tests;
- evidence location and label;
- observability, support and incident owner;
- release, rollback and re-entry instructions; and
- unresolved objects that block promotion.

## Merge and release rule

Repository plans may merge independently after review. Runtime changes must follow the dependency order and cannot be promoted on another repository's narrative claim. Cross-repository release is a separate signed decision after integrated evidence is assembled.


