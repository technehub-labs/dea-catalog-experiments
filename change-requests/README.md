# Change Requests: dea-catalog-experiments

This index tracks every change request that lands on this repository.

| CR | Title | Status | Notes |
|----|-------|--------|-------|
| [CR-EXP-CAT-04](CR-EXP-CAT-04-catalogue-foundation.md) | Catalogue foundation (kit bring-up) | Landed (this PR) | Standard kit: pointer, dependencies, schema projection, gates 1-6, workflows, FOUNDATIONS, record standard. No records admitted. |
| CR-EXP-CAT-02 | Initial population | Planned | Evidence-gated seed population per FOUNDATIONS §7. |

## Numbering

Series tag `CR-EXP-CAT-NN`, sequential. Cross-repo CRs that touch this
repository are recorded here with their home-repo identifier.
| [CR-EXP-CAT-02](CR-EXP-CAT-02-cr-exp-cat-02.md) | Entity Ingestion Groundwork (candidate intake queue + gates) | **Proposed (this PR)** | Gated intake: queue + blocking queue gate + admission tool (candidate-state subtrees, content-derived ids); pin v2.6.0→v2.8.0 + shard-aware toolchain re-vendor. No records. |
| [CR-EXP-CAT-03](CR-EXP-CAT-03-cr-exp-cat-03.md) | Experiment Candidate Corpus | **Landed (this PR)** | 1200 queue submissions from 1 bank(s); manifest with sha256s; queue gate CONFORMANT; no entities change. |
| [CR-EXP-CAT-04](CR-EXP-CAT-04-cr-exp-cat-01.md) | Experiment Candidate Admission Batch 02 (NCT00000576 — Inhaled Beclomethasone to Prevent Chronic Lung Disease … NCT07936851 — Efficacy and Safety of Percutaneous Nephrostomy Versus Double J Stent Insertion in Pregnant Patients With Symptomatic Right-sided Hydronephrosis: A Randomized Trial.) | **Landed (this PR)** | Admitted 1200 `Experiment` CANDIDATE records via the gated intake workflow (queue gate → admission tool → catalog gates); candidates +1200, canonical unchanged; records at `lifecycle_status: proposed` in `candidates/` subtrees. |
| [CR-EXP-CAT-05](CR-EXP-CAT-05-cr-exp-cat-05.md) | CR Numbering Correction | **Landed (this PR)** | Colliding batch CR numbers renumbered (mapping in the CR); content unchanged. |
| [CR-EXP-CAT-06](CR-EXP-CAT-06-cr-exp-cat-06.md) | Canonical Admission Wave (1200) | **Landed (this PR)** | 1200 records promoted candidates/ -> canonical root; ladder completed; evidence preserved; canonical 1200, candidates 0. |
| [CR-EXP-CAT-07](CR-EXP-CAT-07-cr-exp-cat-07.md) | Shard Subdivision (R5 Remedy) | **Landed (this PR)** | Over-cap shard subdivided; toolchain depth-3; ids untouched. |
| [CR-EXP-CAT-08](CR-EXP-CAT-08-cr-exp-cat-08.md) | Shard Re-spread (R5 Remedy) | **Landed (this PR)** | Degenerate sub-shard re-spread by slug tail; ids untouched. |
