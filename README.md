# Tang et al. 2023 — pan-cancer NK atlas (re-analysis + CD160/DGAT overlay)

Re-analysis of the publicly available single-cell dataset from:

> **Tang F, Li J, Qi L, et al. A pan-cancer single-cell panorama of human natural killer cells.**  
> *Cell* 2023. https://doi.org/10.1016/j.cell.2023.07.034  
> Data: Zenodo https://zenodo.org/records/8275845

## Dataset at a glance
- **System:** Pan-cancer human NK cells — 160,011 NK cells from 716 patients, 24 cancer types
- **Assay:** Integrated scRNA-seq atlas
- **NK states:** six functional NK-cell states across healthy and malignant tissues

## What this repository does
Re-processes the Tang et al. pan-cancer NK atlas and scores it for a **CD160-positive NK
signature** and **DGAT expression** across cancer types, tissues and NK subsets, with a
proteomics follow-up. See the numbered `scripts/01–04_*.Rmd` files.

## Repository structure
- `scripts/` — preprocessing, CD160+ signature scoring, DGAT expression, proteomics follow-up
- `results/` — figures (signature scores, expression across histology/tissue)

---
Part of my NK-cell single-cell research programme — see my [GitHub profile](https://github.com/Eomesodermin) and [dilloncorvino.com](https://dilloncorvino.com).  
Author: **Dillon Corvino**

## Environment

Built in a **Seurat**-based single-cell stack in **R** (`Seurat`, `dplyr`, `ggplot2`, and my helper package [`r-utility-functions`](https://github.com/Eomesodermin/r-utility-functions)).

No pinned `renv.lock` is committed; the packages listed above are the required dependencies.
