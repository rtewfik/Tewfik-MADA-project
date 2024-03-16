# Project Overview

Welcome to Ranni Tewfik's MADA project repository! The sections below provide details to reproduce my analyses and results in R.

Project title: Survival Analysis of Males in the U.S. with Prostate Cancer Based on Race and Ethnicity

Research question: Among males diagnosed with prostate cancer, are race and ethnicity associated with time to all-cause mortality?

Data source: SEER 18 (2000-2018) Registry

All required files can be found within this GitHub repository. The scripts should be run in the following order:

1. processing-code.qmd
2. exploratory-analysis.qmd
3. statistical-analysis.qmd


# Required Packages

Load the following R packages before running any code:
* here
* dplyr
* skimr
* survival
* survminer
* ggplot2
* tidyverse
* gtsummary
* knitr
* car


# Project Folders

* The `data` folder contains the raw data (`data/raw-data` subfolder) and the processed data (`data/processed-data` subfolder).

* The `code` folder contains the R scripts for data processing (`code/processing-code` subfolder) and data analysis (`code/analysis-code` subfolder).

* The `results` folder contains code output, including tables (`results/tables` subfolder) and figures (`results/figures` subfolder).

* The `products` folder contains the project manuscript and the supplementary material.


# Exploratory Analysis

The file for the raw data `SEER.csv` is located in the `data/raw-data` folder. The processing script `processing-code.qmd` in the `code/processing-code` folder is run to load the raw data, clean it, and save it as `processeddata.rds` in the `data/processed-data` folder.

The exploratory analysis script `exploratory-analysis.qmd` in the `code/analysis-code` folder is run to load the processed data and explore the variables in the data. The results of the exploratory analysis are saved in the `results/tables` and `results/figures` folders.


# Statistical Analysis

The statistical analysis script `statistical-analysis.qmd` in the `code/analysis-code` folder is run to load the processed data and do statistical analysis, including assessment of the proportional hazards assumption and fitting Cox proportional-hazards models. The results of the statistical analysis are saved in the `results/tables` and `results/figures` folders.

