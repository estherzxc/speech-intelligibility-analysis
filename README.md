# Speech Intelligibility Statistical Analysis

## Overview

This project examined speech intelligibility among children with repaired cleft lip and palate and comparison groups. The goal was to determine whether children with repaired cleft lip and palate had lower overall intelligibility or different patterns of phonetic errors.

Speech intelligibility was evaluated using recordings from a 154-word test covering 11 phonetic contrast categories. Adult listeners transcribed the recorded words, allowing intelligibility to be measured as the percentage of words correctly understood.

## Research Questions

1. Do children with repaired CLP exhibit lower single-word speech intelligibility compared with children in the other study groups?
2. Do children with repaired CLP exhibit different patterns of phonetic contrast errors compared with children in the other study groups?

## Data

The analytical dataset included 115 children across four study groups:

- Repaired cleft lip and palate (CLP): 23
- Repaired cleft palate only (CP): 24
- Typically developing (TD): 34
- History of otitis media (OM): 34

Each child's speech was independently evaluated by three adult listeners. The primary outcome was the mean percentage of test words correctly transcribed across the three listeners.

The original dataset is not included because I do not have permission to redistribute it publicly. No individual-level or confidential data are included in this repository.

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
