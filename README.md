# Project B: Randall's plaque transcriptomic comparator analysis

Public analysis-source package, version 1.0 (8 October 2026), for GSE73680 and GSE117518.
This repository contains frozen source tables, retained processed inputs, code, approved vector
figures and validation records. It accompanies an author-review BMC Genomics manuscript.

## Download

[Version 1.0 release](https://github.com/caonimasb13-del/projectb-randalls-plaque-analysis/releases/tag/projectb-v1.0.0).

Download **all four archives**, then extract them into the same empty directory:

- [ProjectB_Source_Tables_v1.0.zip](https://github.com/caonimasb13-del/projectb-randalls-plaque-analysis/releases/download/projectb-v1.0.0/ProjectB_Source_Tables_v1.0.zip)
- [ProjectB_Plotting_Input_v1.0.zip](https://github.com/caonimasb13-del/projectb-randalls-plaque-analysis/releases/download/projectb-v1.0.0/ProjectB_Plotting_Input_v1.0.zip)
- [ProjectB_Analysis_Inputs_v1.0.zip](https://github.com/caonimasb13-del/projectb-randalls-plaque-analysis/releases/download/projectb-v1.0.0/ProjectB_Analysis_Inputs_v1.0.zip)
- [ProjectB_Code_Documentation_v1.0.zip](https://github.com/caonimasb13-del/projectb-randalls-plaque-analysis/releases/download/projectb-v1.0.0/ProjectB_Code_Documentation_v1.0.zip)

Run `python code/verify_files.py` to check the extracted files. Read the extracted README.md for
software dependencies and instructions. `Rscript code/reproduce_figures.R` recreates the nine figures;
`Rscript code/recover_analysis.R` validates the primary models and recorded recovery pipeline.

## Verification

- 38 frozen source CSVs and the original plotting RDS are byte-identical to the manuscript sources.
- Refitting all three primary internal models reproduces every coefficient and moderated t statistic exactly.
- 20 recovered tables agree with the frozen sources within numeric tolerance.
- The first three disjoint allocations reproduce stored gene/Hallmark Pearson values within 1e-10.
- All nine reproduced PNG figures are pixel-identical to the reviewed manuscript figures.

## Scope

The original expression datasets remain available at
[GEO GSE73680](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE73680) and
[GEO GSE117518](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE117518).
The public package contains reused processed expression data and public sample metadata.
No new patient records, draft manuscript, cover letter or author correspondence are published here.

No main individual-probe FDR discovery is claimed. Split distributions are dependent, null-tail
fractions are descriptive, and external agreement is selective. This package does not establish
biological antagonism, causation, global replication or validated targets.

MSigDB 2026.1 Hallmark is attributed to its original providers under its official CC BY 4.0 terms.
See THIRD_PARTY_NOTICES.md for provenance and rights. A package-wide reuse license for the original
analysis code/derived outputs remains an author decision; none has been invented. Manuscript
authorship is not finalized. No DOI, journal submission or acceptance is implied.
