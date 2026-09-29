# CLAUDE.md

@~/.claude/hospital-privacy.md

Grant-figure website for the Sherley carboplatin cohort (N = 121), published at
https://github.com/Tianqi-Ouyang/Grant- (GitHub Pages from `main` / `docs`).

- Single page: `index.qmd`. Render with `quarto render`; output goes to `docs/`.
- Data is read by absolute path from the Sherley project
  (`/Users/to909/Desktop/Meg/Sherley/sherley_final_master.rds`, written by
  `Sherley/qmd/sherley_data.qmd`). Never copy data files into this repo.
- `egfr_difference = 100 * (ckd_epi_gfr_cre_cys_unindex - cockcroft) / cockcroft`
  (percent; BSA-adjusted Cr-Cys eGFR so units match CG, mL/min). −10 % is the
  randomization cutoff. subHRs are reported per 10 % decrease.
- Adjusters: age, sex, ecog_score (numeric), ici, cockcroft; + pre_HGB_45days
  (anemia), pre_PLT_45days (thrombocytopenia), both for composite cytopenias.
- Plots are saved as editable PowerPoint via `.save_plot_pptx(p)` into
  `docs/plots/grant/`; `scripts/inject_pptx_links.py` (post-render) adds the
  per-figure download links.
