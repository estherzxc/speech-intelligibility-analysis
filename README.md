# Speech Intelligibility Statistical Analysis

## Overview

This project analyzed speech intelligibility outcomes in children with repaired cleft lip and palate and comparison groups. Speech intelligibility was measured using a 154 single-word intelligibility test, where adult listeners transcribed children’s recorded speech.

The study included four groups of children: repaired cleft lip and palate (CLP), repaired cleft palate only (CP), typically developing children (TD), and children with a history of otitis media (OM).

## Research Questions

1. Do children with repaired CLP exhibit lower single-word speech intelligibility compared with children in the other study groups?
2. Do children with repaired CLP exhibit different patterns of phonetic contrast errors compared with children in the other study groups?

## Data

The dataset included 115 children:
- CLP: 23
- CP: 24
- TD: 34
- OM: 34

Each child’s speech was evaluated by three adult listeners. The primary outcome was mean single-word intelligibility score, averaged across listeners. The original dataset is not included in this repository because it is not publicly shareable.

## Methods

The analysis included:

- Descriptive statistics for participant characteristics and intelligibility scores
- Linear regression modeling for mean single-word intelligibility
- Repeated-measures modeling using listener-specific scores
- Child-level random intercepts to account for multiple listener ratings per child
- Adjustment for age and sex
- Analysis of phonetic contrast-level intelligibility patterns
- Sensitivity analyses

## Descriptive Analysis

Descriptive analyses summarized the study population, outcome distribution, covariates, and missingness. The primary outcome was mean single-word intelligibility score, averaged across adult listeners. The dataset included 115 children across four groups: CLP, CP, TD, and OM. Mean intelligibility scores ranged from 44.2% to 98.1%, with an overall mean of 87.9%. Age, sex, cleft type, and hypernasal status were evaluated as covariates.

Exploratory visualizations included boxplots of mean intelligibility scores by group and sex, scatterplots of mean intelligibility versus age by group, and boxplots comparing intelligibility scores by hypernasal status.

## Repository Contents

* [`code/final_analysis_code.qmd`](code/final_analysis_code.qmd): complete analysis code and documentation
* [`code/final_analysis_code.pdf`](code/final_analysis_code.pdf): rendered version of the analysis
* [`report/statistical_analysis_plan.pdf`](report/statistical_analysis_plan.pdf): prespecified statistical analysis approach
* [`report/final_report.pdf`](report/final_report.pdf): final written report and results
* [`presentation/final_presentation.pdf`](presentation/final_presentation.pdf): presentation summarizing the project
* [`data/DATA_NOT_INCLUDED.md`](data/DATA_NOT_INCLUDED.md): explanation of data availability and restrictions

LaTeX source files used to produce the report and presentation are included alongside their corresponding PDF files.


## Data Availability

The original research dataset is not included because it contains non-public study data. The code is provided to demonstrate the statistical workflow and analysis structure.

## Skills Demonstrated

- Biostatistical analysis
- Linear regression
- Repeated-measures analysis
- Mixed-effects modeling
- Random intercept models
- Estimated marginal means
- Multiple-comparison adjustment
- Sensitivity analysis
- Statistical reporting in R
