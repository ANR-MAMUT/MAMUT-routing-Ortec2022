# Changelog: Ortec2022 benchmark family

All notable changes to the Ortec2022 family are recorded here. The family had no changelog before the entry below.

## 2026-11: family repository

- The family, tracked until now directly in the main MAMUT-routing repository, becomes the repository `MAMUT-routing-Ortec2022`, mounted in MAMUT-routing at `benchmarks/Ortec2022`. Its history is extracted from the history of the main repository, under the directory of its problem type. `history/` holds the map from the former to the new commit identifiers.
- Instances and best-known solutions keep their former path after the problem type, for example `VRPTW/final/n=200/ORTEC-VRPTW-ASYM-05362619-d1-n212-k20.vrp.json`.
- No data changes. No instance, no best-known solution and no instance identifier changed. Only the location changed.
- `mamut-collection.json` at the root marks the repository as a family collection (`"layout_version": 2`).
- This layout is read by `mamut-routing-lib` 0.13 and later, which is in development and not released yet. `mamut-routing-lib` 0.12 and earlier read the former layout, which stays available read-only in the archive of the former main repository, `MAMUT-routing-archive-2026-11`.
- The README and LICENSE files move from `VRPTW/` to the root, and CITATION.cff, NOTICE and this changelog are added.
