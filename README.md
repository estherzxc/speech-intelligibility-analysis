# Speech Intelligibility Statistical Analysis

## Overview

This project examined speech intelligibility among children with repaired cleft lip and palate and comparison groups. The goal was to evaluate whether children with repaired cleft lip and palate had lower overall speech intelligibility and whether they showed different patterns of phonetic contrast errors.

Speech intelligibility was evaluated using recordings from a 154-word single-word test covering 11 phonetic contrast categories. Adult listeners transcribed the recorded words, and intelligibility was measured as the percentage of words correctly understood.

## Research Questions

1. Do children with repaired cleft lip and palate (CLP) exhibit lower single-word speech intelligibility compared with children in the other study groups?
2. Do children with repaired CLP exhibit different patterns of phonetic contrast errors compared with children in the other study groups?

## Data

The original dataset included 115 children across four study groups:

- Repaired cleft lip and palate (CLP): 23
- Repaired cleft palate only (CP): 24
- Typically developing children (TD): 34
- Children with a history of otitis media (OM): 34

Each child’s speech was independently evaluated by three adult listeners. The primary outcome was the mean percentage of test words correctly transcribed across listeners. The project description states that mean intelligibility scores ranged from 44.2% to 98.1%, with an overall mean of 87.9%. :contentReference[oaicite:0]{index=0}

The original dataset is not included because I do not have permission to redistribute it publicly. No individual-level or confidential data are included in this repository.

## Analysis Workflow

### Descriptive and Exploratory Analysis

Descriptive analyses summarized participant characteristics, speech intelligibility scores, covariates, and missingness. Exploratory visualizations examined the distribution of mean intelligibility scores by group and sex, the relationship between mean speech intelligibility and age by group, and mean intelligibility scores by velopharyngeal (VP) status.

### Preliminary Analysis

Several preliminary analyses were conducted to evaluate the data structure and guide modeling decisions.

#### Listener Reliability

Intraclass correlation coefficients (ICCs) were used to assess agreement among listener ratings. Listener Groups 2, 3, and 7 showed poor agreement, with ICC values below 0.5. This step helped evaluate whether listener ratings were sufficiently consistent and whether child-level average speech intelligibility scores could reasonably be used in later analyses.

#### Combining TD and OM Groups

The typically developing (TD) and otitis media (OM) groups were compared to determine whether they could be combined into a single Control group. Shapiro-Wilk tests indicated non-normality in both groups, so a bootstrapped two one-sided test (TOST) equivalence approach was used.

The observed mean difference was 3.08 points, with a 90% bootstrapped confidence interval of 0.87 to 5.68. Although formal statistical equivalence was not fully confirmed, the observed difference was considered clinically negligible. Therefore, TD and OM were combined into a single Control group for subsequent analyses.

#### Influence of Inadequate VP Status

Velopharyngeal inadequacy was examined because it may further compromise speech production in children with cleft palate. All children with inadequate VP status were in the CLP or CP groups, and only six children had inadequate VP status.

Because VP dysfunction is a physiological consequence of cleft palate rather than an independent confounder, children with inadequate VP status were excluded from the primary and secondary analyses. The final analytic sample for the primary and secondary analyses was 108 children. Analyses including these children were presented as sensitivity analyses.

### Primary Analysis

### Secondary Analysis

### Sensitivity Analysis

## Key Findings



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
- Descriptive and exploratory data analysis
- Reliability analysis using ICC
- Equivalence testing using bootstrapped TOST
- Linear regression
- Repeated-measures analysis
- Mixed-effects modeling
- Random intercept models
- Estimated marginal means
- Multiple-comparison adjustment
- Sensitivity analysis
- Statistical reporting in R
