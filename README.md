# Grant Figures — Sherley Carboplatin Cohort

Grant-figure versions of the Sherley project's Carboplatin Cohort analyses
(N = 121), re-expressed on the **eGFR difference** scale:
`100 × (eGFR CKD-EPI Cr-Cys, BSA-adjusted − Cockcroft-Gault CrCl) / Cockcroft-Gault CrCl`,
with −10 % as the randomization cutoff.

Live site: https://tianqi-ouyang.github.io/Grant-/

## Data

No patient data is stored in this repository. The page reads the analysis
dataset produced by the Sherley project's data pipeline
(https://github.com/Tianqi-Ouyang/Sherley-project, `qmd/sherley_data.qmd`):

```
/Users/to909/Desktop/Meg/Sherley/sherley_final_master.rds
```

## Rendering

```bash
quarto render
```

Output lands in `docs/` (served by GitHub Pages from `main` / `docs`). Each
figure is also saved as an editable PowerPoint slide under `docs/plots/grant/`;
the post-render script `scripts/inject_pptx_links.py` adds a download link
beneath every figure.
