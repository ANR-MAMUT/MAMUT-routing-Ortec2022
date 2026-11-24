# Ortec2022 benchmark family (VRPTW)

Benchmark family repository of [MAMUT-routing](https://github.com/ANR-MAMUT/MAMUT-routing), mounted there as `benchmarks/Ortec2022`. It contains the MAMUT-routing curation of the static VRPTW instances from the EURO Meets NeurIPS 2022 Vehicle Routing Competition.

## Layout

- `VRPTW/final/n=<size>/` and `VRPTW/public/n=<size>/` hold the instances (`<Name>.vrp.json`) and their best-known solutions (`<Name>.bks.MonoCost.json`), for example `VRPTW/final/n=200/ORTEC-VRPTW-ASYM-05362619-d1-n212-k20.vrp.json` and `VRPTW/final/n=200/ORTEC-VRPTW-ASYM-05362619-d1-n212-k20.bks.MonoCost.json`.
- `mamut-collection.json` at the root marks the repository as a family collection (`"layout_version": 2`).
- `history/` holds the commit map of the former location of this family (see the history section below).

Edition `r1` uses `binary64-exact-v1` to evaluate routes on the materialized static matrix. The certified solution cost is the fraction in `metadata.standard.authoritative_cost`. The top-level `cost` is its binary64 display.

## Library compatibility

This layout is read by `mamut-routing-lib` 0.13 and later, which is in development and not released yet. `mamut-routing-lib` 0.12 and earlier read the former layout, which stays available read-only in the archive of the former main repository, [MAMUT-routing-archive-2026-11](https://github.com/ANR-MAMUT/MAMUT-routing-archive-2026-11).

## License scope

- ORTEC instances and related redistributed BKS files retain the original Creative Commons Attribution-NonCommercial 4.0 International license (CC BY-NC 4.0).
- MAMUT-routing conversions, repairs, metadata, and computed BKS records in this repository are distributed with this family under the same CC BY-NC 4.0 notice unless an individual file states otherwise.
- The MIT license of the MAMUT-routing repository applies to MAMUT-routing source code, not to these ORTEC benchmark data files.

## Attribution

The source material comes from the EURO Meets NeurIPS 2022 Vehicle Routing Competition organized with ORTEC support, https://euro-neurips-vrp-2022.challenges.ortec.com/

The license deed is available at https://creativecommons.org/licenses/by-nc/4.0/

Preserve this README, the LICENSE file of this repository, and the [NOTICE](NOTICE) file of this repository when redistributing this benchmark family.

## Citation

The citation metadata of this repository, with its authors and their ORCID identifiers, is recorded in [CITATION.cff](CITATION.cff). This family is a curation of a third-party benchmark, so also cite the original benchmark, the EURO Meets NeurIPS 2022 Vehicle Routing Competition organized with ORTEC support (https://euro-neurips-vrp-2022.challenges.ortec.com/). Record the exact Git commit used in experiments.

## History of this repository

Until November 2026 the family was tracked directly in the main MAMUT-routing repository, at `benchmarks/VRPTW/Ortec2022`. Its history was extracted from the history of the main repository and rewritten under the directory of its problem type (`VRPTW/`). Only the commits that touched this directory are kept, each with a new identifier. `history/commit-map-MAMUT-routing.tsv` maps the former commit identifiers of the main repository to the new ones, for the kept commits only. It is tab-separated, with the former commit identifier and the new one on each line, after a header line. This repository has no changelog before this reorganisation. See [CHANGELOG.md](CHANGELOG.md) for it.
