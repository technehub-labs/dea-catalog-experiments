# dea-catalog-experiments

> DEA catalog for **Experiment** — OpenDEAM v0.3.0 (ADR-0003).

## Experiment (`EXP`)

- **Entity id:** `dea:entity-experiment`
- **Allocation:** L2 · L2-innovation-foresight
- **Status:** proposed

A bounded, time-boxed test of a Signal's relevance to the enterprise before committing investment.

## Relationships (from the OpenDEAM model)

- **EXP → II** — informs (dependency, 0..N:0..1)
- **SIG → EXP** — triggers (dependency, 0..N:0..N)
- **TRE → EXP** — evaluated via (dependency, 1:0..N)

## Allocation contract

This repo's `metamodel-pointer.yaml` is validated in CI against the pinned
OpenDEAM root model (`v0.3.0`) via the reusable
`validate-against-model.yml` workflow. Drift fails CI.

Content (entity instances) lands when the entity promotes from
`proposed` to `planned`/`scaffold` per the model lifecycle.

## License

Apache 2.0 — see [LICENSE](./LICENSE) and [NOTICE](./NOTICE).
