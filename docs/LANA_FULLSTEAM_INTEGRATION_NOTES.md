# Lana / Limo Anywhere / FullSteam — Beem integration note

**Status:** RESEARCH / IMPLEMENTATION SCOPING; NOT AN APPROVED API OR FEATURE. This is a reconciliation note, not a third operative Beem specification. It is subordinate to Beem Product Canon v1.0, Build Spec v1.2, Plan v0.3 and FullSteam's actual written API terms.

## Why Lana matters

Lana is Limo Anywhere's assistant layer. It is a potential **operator-side specialist capability** for Beem's commercial Account Manager. Beem should send a bounded, operator-authorised query or candidate request to that layer if official access exists; it must **not** duplicate dispatch, LQC administration or LA operational decisions merely because it can reason about them. The spelling/name used here is **Lana**; verify product naming and technical release state against FullSteam documentation before shipping.

## Keep three connections distinct

1. **LA Customer / Partner API, webhooks, Addons and supported booking links:** the primary typed supply and observation connectors. Phase One read-only under per-operator AuthorisationRecord, purpose restriction, revocation and fail-closed controls. Proposed writes are independently gated by exact operation, confirmation in LA and verified rights.
2. **FullSteam/LA-provided MCP interface:** draft-affiliation text refers to an MCP interface, but its actual published endpoint, schemas, auth, supported actions, hosting, pricing and permissions have not been evidenced here. Ask FA-31 remains open. It is **inbound to Beem** as an LA provider surface, if available.
3. **Lana-specific programme interface:** do not infer that Lana is available as an API, MCP server or externally invokable agent. Obtain written proof of its tool/resource surface, permitted operations, tenant/account scoping, on-behalf-of principal semantics, action/approval flow and audit correlation. If there is no supported invocation, offer deep links and operator-guided usage without pretending Beem controls Lana.

Separately, Beem's **own outbound plugin/MCP/API/SDK adapters** expose Beem-owned governed capabilities to ChatGPT and other hosts. An outbound Beem plugin is not proof that it can invoke inbound Lana. Build one shared typed-capability contract, then place separate adapters on either side.

## Proposed service interaction

Account Manager -> qualified Account/WorkPacket -> minimum admitted operator-specific state -> operation-scoped capability discovery -> LA/Lana adapter for permitted read/candidate work -> evidence and source authority -> Beem candidate Plan or WorkPacket -> BLCP policy and exact-operation binding for any material action -> LA native execution / operator approval -> receipt -> independently observed LA outcome -> reconciliation -> Beem Account re-entry.

Where the LA/Lana invocation itself can mutate external state, it is not a free-form code-mode call. Require exact-operation checks at each consequence and ensure Lana cannot silently escalate a Beem user's access.

## Acceptance proof for Lana

- Current FullSteam official technical specification and signed right to connect.
- Operator-specific consent and account binding tested; revoke/suspend immediately blocks use.
- Exact operations, schemas, effects (read/candidate/write), data restrictions and rate limits documented.
- Sandbox demonstrates request, receipt, source attribution, partial failure, denial, timeout, replay and independent observation.
- Prompt or model output cannot access another operator or cause unapproved booking, dispatch, billing, configuration or marketing send.
- If Lana is unavailable, the standard LA connector plus native links and a manual bridge preserve service without invented output.

## Source anchors

- [Beem Spec v1.2](https://docs.google.com/document/d/1dCNjPZW3zjNObHZQtCzGDFpKclTj6Hbfw6YYwtc8IU8/edit), particularly §§35A–35B, 83A, 84A–84B.
- [Plan v0.3](https://docs.google.com/document/d/1sUfSwkGdGVmRNyaxGrG_m2J8WETQOOLZMJ06p6yfjK4/edit), P1.5A–C / P2.9.
- [FullSteam Ask Register](https://docs.google.com/document/d/1CRdRUECvHms-V2_hbHbI-6tUv13Ekx0NYYK8tNHfcK4/edit), FA-04, FA-11, FA-31, FA-41.
- [Beem x FullSteam Blueprint](https://docs.google.com/document/d/1lHITtldGMp4fc1RqRRp3tlIkB_x-8gVcfMiEH9LU47w/edit); draft-agreement analysis and its explicit unresolved licence questions.

**No claim is made that an official Lana-to-Beem bridge is implemented or contractually permitted.**
