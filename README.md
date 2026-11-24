# Geoffrey Manda

I am an epidemiologist developing tools for survey analysis, data quality, scientific visualisation and reproducible statistical workflows.

## R packages

| Package | Use it for | Start here | Worked example | Automated checks |
|---|---|---|---|---|
| [dqguard](https://github.com/GeoffreyManda/dqguard-public) | Evaluate data-quality rules, inspect findings and control release decisions. | [Installation and guide](https://github.com/GeoffreyManda/dqguard-public/blob/main/docs/getting-started.md) | [Check and correct a synthetic intake](https://github.com/GeoffreyManda/dqguard-public/blob/main/inst/examples/worked-example.R) | [Installation, tests and example](https://github.com/GeoffreyManda/dqguard-public/actions/workflows/package-checks.yaml) |
| [vellum](https://github.com/GeoffreyManda/vellum-public) | Create scientific figures with plot recipes, palettes and explicit export dimensions. | [Installation and guide](https://github.com/GeoffreyManda/vellum-public/blob/main/docs/getting-started.md) | [Export an interval figure](https://github.com/GeoffreyManda/vellum-public/blob/main/inst/examples/worked-example.R) | [Installation, tests and example](https://github.com/GeoffreyManda/vellum-public/actions/workflows/package-checks.yaml) |
| [manimR](https://github.com/GeoffreyManda/manimR-public) | Build mathematical animations from R scenes and timelines. | [Installation and guide](https://github.com/GeoffreyManda/manimR-public/blob/main/docs/getting-started.md) | [Render a growing-circle GIF](https://github.com/GeoffreyManda/manimR-public/blob/main/inst/examples/worked-example.R) | [Installation, tests and example](https://github.com/GeoffreyManda/manimR-public/actions/workflows/package-checks.yaml) |

The three package workflows passed installation, installed tests and their worked examples on Ubuntu on 24 November 2026: [dqguard](https://github.com/GeoffreyManda/dqguard-public/actions/runs/45383600031), [vellum](https://github.com/GeoffreyManda/vellum-public/actions/runs/45384336582), and [manimR](https://github.com/GeoffreyManda/manimR-public/actions/runs/45383984874). The workflow links above show subsequent results. Optional capability skips are recorded in the test logs.

## Survey analysis and analytical engineering

- [surveystats](https://github.com/GeoffreyManda/surveystats): weighted survey estimates from indicator registers using base R, including stratified cluster variance for proportions, means and totals.
- [TF-RES](https://github.com/GeoffreyManda/tfres): R engineering standards, data contracts, guarded joins and source checks.
- [UOTF](https://github.com/GeoffreyManda/uotf): ontology modelling, validation and compilation with Python, R and Node clients.

## Install an R package

```r
install.packages("remotes")
remotes::install_github("GeoffreyManda/dqguard-public")
library(dqguard)
source(system.file("examples", "worked-example.R", package = "dqguard"))
```

Each package guide explains its dependencies, outputs and practical limits. The worked examples use synthetic inputs. Report issues with a small reproducible example and your R version.
