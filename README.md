# ESOL Scaffold-Aware Solubility Project

This repository contains a reproducible ESOL analysis workflow for scaffold-aware aqueous solubility modeling.

## Run

```bash
python src/esol_project.py --config config.yaml
```

## Output

The workflow reads:

```text
data/esol.csv
```

and generates:

* `results/tables/*.csv`: quality-control, benchmark, cross-validation, ablation, uncertainty, applicability-domain (AD), error-analysis, and screening-demonstration tables.
* `results/figures/*.png`: distribution, correlation, chemical-space, calibration, applicability-domain, error, bias, and molecular visualization figures.

## Notes

The local dataset contains only ESOL SMILES strings and experimental logS values. Because no external screening library is provided, the virtual-screening section is implemented as a demonstration using locally held-out candidate compounds.
