# CSR/Alembee Corpus-to-Build Traceability

| Source/control | Required interpretation | Plan location | Implementation epic/gate |
|---|---|---|---|
| Curtis Master Corpus v1.5 | Discovery index, precedence, provenance and amendment control | `PLAN_SOT.md` §4, §17 | PD0, E01 |
| SRC-072 signed build control | One Alembee product, repository identity, eight-week envelope, evidence release | `PLAN_SOT.md` §2–§5, §14–§17 | PD0, E00–E30 |
| SRC-074 repository-aligned plan | Full target architecture, 29+ epics, negative tests, migration/cutover | Entire package | `IMPLEMENTATION_PLAN.md` |
| SRC-079 AISO specialist canon | Nine stages, five modules/pillars, evidence classes, scoring, package and QA | `PLAN_SOT.md` §8 | E13–E15, E28 |
| SRC-071 GPTO factual brief | Existing implementation evidence without authority transfer | `REPOSITORY_EVIDENCE_BASELINE.md` | E01, E13 |
| SRC-080 client-site compliance canon | Cookie/storage/purpose/activation/refusal/withdrawal responsibilities | `PLAN_SOT.md` §11 | E29 |
| SRC-081 CSR compliance amendment | CSR-owned compliance contracts, sequence and adversarial tests | `PLAN_SOT.md` §11 | E29, E30 |
| SRC-076 FullSteam specialist application | Chauffeur/coach provider integration and commercial surface | `PLAN_SOT.md` §10, §12 | E08–E12 |
| SRC-070/075/077 | Commercial intelligence, venture/operating context | `PLAN_SOT.md` §12 | E20, E24–E27 |
| SRC-078 patent draft | Legal/IP input and patent-aligned orchestration concepts | `PLAN_SOT.md` §4, §13 | E00, E06 |
| Alembee-cdhq source | ATS/lead-marketplace donor and primary shell | `REPOSITORY_EVIDENCE_BASELINE.md` | E03, E04, E07/E07A/E07B |
| FAR source | Quote/mobility/orchestration donor | `PLAN_SOT.md` §10, §14 | E01A, E08–E12 |
| Conversion CGS source | Governed execution substrate | `PLAN_SOT.md` §5, §7, §14 | E00, E02–E06, E19 |
| GPTO sources | Observation/reporting/AISO donor implementations | `PLAN_SOT.md` §8, §14 | E13–E16 |
| GIA plan/repo | Exact-use admissibility contract; separate product | `PLAN_SOT.md` §5, §7 | E17 |
| CIG plan/repo | Transition boundary contract; separate product | `PLAN_SOT.md` §5, §7 | E17A |

Detailed use-case coverage is in `CAPABILITY_AND_USE_CASE_SPEC.md`; executable conformance is enumerated in `ACCEPTANCE_TEST_CATALOGUE.md`; source/data transition is controlled by `MIGRATION_AND_CUTOVER_PLAN.md`.

## Coverage rule

Every future issue or PR must cite one or more rows above and the exact requirement it implements. A traceability link is not completion evidence; the issue must also contain tests, evidence label, migration and rollback.

