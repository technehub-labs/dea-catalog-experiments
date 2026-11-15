# Changelog

## [Unreleased]

### CR-EXP-CAT-07: Shard Subdivision (R5 Remedy)

Over-cap shard subdivided into two-character sub-shards (R5 findings resolved); vendored toolchain upgraded to depth-3 shard walking; ids untouched.

### CR-EXP-CAT-06: Canonical Admission Wave

1200 Experiment records promoted from the candidate slot to the canonical slot (provenance ladder completed per record; evidence citations preserved; ids untouched). Index: canonical 1200, candidates 0. All gates green.

### CR-EXP-CAT-04: Experiment Candidate Admission Batch 02

Admitted 1200 new `Experiment` CANDIDATE records through the gated intake workflow (queue gate → admission tool → catalog gates); ids content-derived and collision-checked; records land in `candidates/` subtrees at `lifecycle_status: proposed` / version 0.1.0; candidates count +1200, canonical unchanged; queue entries flipped to `admitted`.

### CR-EXP-CAT-03: Experiment Candidate Corpus

1200 Experiment candidate submissions landed in the contribution queue (sharded, gate-CONFORMANT) from 1 evidence bank(s); published prose + evidence citations + source_refs; provenance in ingestion/manifest.yaml. No catalog entities change; admission follows in EXP-CAT-04+.

### CR-EXP-CAT-02: Entity Ingestion Groundwork (candidate intake queue + gates)

Gated intake workflow stood up: contribution queue + blocking queue gate (`scripts/check_contributions.py`, self-deriving from the projected schema) + admission tool (`scripts/admit_entity.py`: content-derived ids, collision-checked, candidates/ subtrees at `lifecycle_status: proposed` / v0.1.0) + intake template and process docs. CI: queue gate added as a blocking step; metaframework pin v2.6.0 → v2.8.0 with the shard-aware toolchain re-vendored from the v2.8.0 release (cmp'd). No records admitted by this CR.

### `CR-EXP-CAT-01` — catalogue foundation (kit bring-up)

Standard kit generated from the metamodel (org-wide catalog advancement
programme): hybrid pointer pinned to OpenDEAM v0.8.0;
`dependencies.yaml`; schema projection (copied-and-narrowed) with the
catalogue-instance layer; vendored relationship-instance contract; fixtures;
gates 1-6 wired into `validate-catalogue.yml` plus allocation and authorship
workflows; FOUNDATIONS (D-1..D-6) and record documentation standard. No
records admitted (population gated on CR-EXP-CAT-02).
