# Psychological Factors and Treatment Outcomes: An R-Based Quantitative Research Project
## Overview

This repository contains a reproducible R-based quantitative research project examining psychological and treatment-related factors associated with symptom outcomes.

The project demonstrates a complete quantitative research workflow, progressing from data preparation and exploratory analysis to regression, moderation, longitudinal mixed-effects modeling, confirmatory factor analysis (CFA), and structural equation modeling (SEM).

**Important:** The dataset used in this project is **simulated for educational and research-training purposes**. It does not represent data collected from human participants, and the findings should not be interpreted as empirical evidence about real patients or treatment effectiveness.


## Research Focus

The project examines how psychological and treatment-related characteristics can be incorporated into quantitative models of symptom outcomes.

The primary variables include:

* Baseline symptoms
* Post-treatment symptoms
* Treatment expectations
* Treatment motivation
* Therapeutic alliance
* Previous treatment experience
* Treatment response

A separate SEM component demonstrates relationships among:

* Overthinking
* Emotional resilience
* Sleep problems

## Research Questions

The project addresses several methodological and substantive questions:

1. Are treatment-related psychological factors associated with symptom outcomes?
2. Does treatment motivation relate to symptom levels?
3. Does treatment motivation moderate change in symptoms over time?
4. Can longitudinal mixed-effects models identify differences in symptom trajectories?
5. Do questionnaire indicators adequately represent latent psychological constructs?
6. Can SEM be used to examine direct and indirect relationships among psychological constructs?


## Analytical Workflow

The project follows a structured quantitative workflow:

```text
Data Preparation
       ↓
Descriptive Statistics
       ↓
Correlation Analysis
       ↓
Multiple Regression
       ↓
Moderation Analysis
       ↓
Longitudinal Mixed-Effects Model
       ↓
Estimated Marginal Means
       ↓
Confirmatory Factor Analysis
       ↓
Structural Equation Modeling
       ↓
Mediation Analysis
       ↓
Visualization & Scientific Reporting
```


## Main Statistical Methods

### Multiple Regression

Multiple regression was used to examine whether treatment-related variables predicted post-treatment symptom levels while accounting for other relevant predictors.

### Moderation

Interaction-based moderation analysis was used to examine whether treatment motivation altered the relationship between treatment expectations and treatment outcomes.

### Longitudinal Mixed-Effects Modeling

A linear mixed-effects model was used to examine symptom change from baseline to post-treatment.

The model included:

* Time
* Treatment motivation
* Time × Treatment motivation

The significant interaction demonstrated how individual differences in treatment motivation can be incorporated into longitudinal models to examine differences in change over time.

### Confirmatory Factor Analysis

CFA was used to evaluate a one-factor measurement model of overthinking based on five questionnaire indicators.

The model demonstrated strong fit in the simulated dataset, with standardized factor loadings ranging from approximately .67 to .82.

### Structural Equation Modeling

SEM was used to examine relationships among overthinking, emotional resilience, and sleep problems.

The model included:

```text
Overthinking
      ↓
Emotional Resilience
      ↓
Sleep Problems
```

Direct paths from overthinking to sleep problems and from emotional resilience to sleep problems were also estimated.

The indirect effect was tested using confidence intervals.

---

## Selected Results

Because the dataset is simulated, these results are presented only as examples of statistical modeling.

### Longitudinal Model

The mixed-effects model demonstrated:

* Significant symptom reduction over time: *B* = −10.00, *p* < .001
* Significant association between treatment motivation and symptoms: *B* = −0.76, *p* = .005
* Significant Time × Treatment Motivation interaction: *B* = −0.65, *p* = .004

The estimated symptom reduction increased across higher levels of treatment motivation in the simulated data.

### CFA

The CFA demonstrated:

* χ²(5) = 1.54, *p* = .908
* CFI = 1.00
* TLI = 1.01
* RMSEA = .000
* SRMR = .007
* Standardized loadings = .67–.82

### SEM

The SEM demonstrated:

* Overthinking → Sleep Problems: β = .27, *p* < .001
* Emotional Resilience → Sleep Problems: β = −.13, *p* = .031
* Overthinking → Emotional Resilience: β = −.09, *p* = .178
* Indirect effect: *B* = .01, 95% CI [−.01, .04], *p* = .289

Thus, the direct association between overthinking and sleep problems was statistically significant, but the hypothesized mediation through emotional resilience was not supported.

---

## Project Structure

```text
psychological-factors-treatment-outcomes/
│
├── data/
│   ├── study_data.rds
│   ├── study_data.xlsx
│   └── SEM_workspace.RData
│
├── R/
│   └── analysis scripts
│
├── Figures/
│   ├── mixed_effects_interaction.png
│   ├── mixed_effects_interaction_final.png
│   ├── SEM_final_APA.png
│   ├── SEM_final_thesis.png
│   ├── SEM_path_diagram.png
│   └── SEM_path_diagram.svg
│
├── Results/
│   ├── cfa_factor_loadings.csv
│   ├── cfa_model_fit.csv
│   ├── estimated_marginal_means.csv
│   ├── mixed_effects_model_results.csv
│   ├── sem_mediation_effects.csv
│   ├── sem_r_squared.csv
│   └── sem_structural_paths.csv
│
├── Report/
│   └── research report
│
└── psychological-factors-treatment-outcomes.Rproj
```

---

## R Packages

The project uses R packages for data import, statistical modeling, longitudinal analysis, latent-variable modeling, and visualization.

Key packages include:

* `readxl`
* `dplyr`
* `ggplot2`
* `lme4`
* `lmerTest`
* `emmeans`
* `lavaan`
* `semPlot`
* `psych`
* `interactions`

---

## Reproducibility

The project follows reproducible research principles by:

* Using an RStudio project
* Organizing files into dedicated directories
* Conducting analyses through R code
* Saving statistical results as structured CSV files
* Saving figures separately from analytical outputs
* Documenting analytical decisions
* Separating analysis, results, and reporting materials

The goal is for another researcher to be able to inspect the workflow and understand how the reported results were generated.

---

## Ethical Statement

This repository contains **simulated data only**.

No real patient data, participant records, or personally identifiable information are included.

The project is intended to demonstrate quantitative research methods and R programming skills rather than to provide clinical or empirical conclusions.

---

## Skills Demonstrated

This project demonstrates experience with:

**R Programming**

* Data manipulation
* Data import/export
* Reproducible project organization
* Statistical programming

**Quantitative Methods**

* Descriptive statistics
* Correlation
* Regression
* Moderation
* Longitudinal analysis
* Mixed-effects modeling
* CFA
* SEM
* Mediation

**Research Practice**

* Hypothesis-driven analysis
* Statistical interpretation
* Confidence intervals
* Effect interpretation
* Scientific visualization
* APA-style reporting
* Reproducible research

---

## Purpose of the Project

This project was developed as an independent quantitative research-training project to strengthen skills in R, longitudinal analysis, latent-variable modeling, and reproducible psychological research.

It is particularly intended to demonstrate the transition from conventional statistical analysis toward more advanced research methods suitable for graduate-level and doctoral-level quantitative research.

---

## Author

**Areeba Fatima**

MS Clinical Psychology
Riphah International University

*Independent R Quantitative Research Project*
