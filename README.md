# Data Cleaning Pipeline for IMR Machine Learning Project

[![R Version](https://img.shields.io/badge/R-4.0+-blue)](https://www.r-project.org/)
[![Tidyverse](https://img.shields.io/badge/tidyverse-ready-green)](https://www.tidyverse.org/)

## 📌 Overview

This repository contains an **R‑based data cleaning pipeline** for the Infant Mortality Rate (IMR) prediction project. The code prepares the **KDHS 2022** (Kenya Demographic and Health Survey) dataset for machine learning modelling by handling missing values, transforming variables, and engineering features relevant to infant mortality risk.

## 🎯 Purpose

- Clean and preprocess raw KDHS 2022 data
- Handle missing values appropriately
- Transform categorical and continuous variables
- Engineer features for ML models (logistic regression, random forest, KNN, etc.)
- Create a reproducible workflow for IMR prediction

## 🗂️ Data Source

- **KDHS 2022** – Kenya Demographic and Health Survey  
  Contains maternal, child, household, and socio‑economic indicators

## 🧼 Cleaning Steps

| Step | Description |
|------|-------------|
| 1 | Load raw data (`.dta` or `.csv`) |
| 2 | Rename and select relevant variables |
| 3 | Convert numeric codes to labelled factors |
| 4 | Identify and impute missing values |
| 5 | Recode inconsistent categories |
| 6 | Remove duplicate records |
| 7 | Create derived variables (e.g., infant mortality status, age groups) |
| 8 | Apply DHS survey weights (if applicable) |
| 9 | Split into training/testing sets for ML |
| 10 | Export cleaned dataset |

## 📁 Repository Structure
DATA-CLEANING-FOR-IMR-ML-PROJECT/
├── Dofile_var_factor.R # Main cleaning script
├── README.md # This file
└── data/ (optional) raw and cleaned data

## 🔧 Requirements

Install the following R packages:

```r
install.packages(c(
  "tidyverse", "haven", "dplyr", "tidyr",
  "labelled", "naniar", "visdat", "skimr"
))
🚀 Usage
Clone the repository:

bash
git clone https://github.com/Jeremiah-muuo/DATA-CLEANING-FOR-IMR-ML-PROJECT.git
Open Dofile_var_factor.R in RStudio.

Set the correct file path to your KDHS 2022 dataset.
Run the script line by line or source it:

r
source("Dofile_var_factor.R")
📊 Output
Cleaned dataset ready for ML modelling

Summary tables of missing values

Diagnostic plots (e.g., missingness patterns)
Saved .rds or .csv file of the processed data

🤝 Contributing
Suggestions and improvements are welcome. Please open an issue or submit a pull request.

