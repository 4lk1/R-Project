# Data Analyst Job Market Analysis

## Author

- Alki Leka

## Abstract

This project presents an exploratory statistical analysis of a dataset containing **1,194 observations** related to the Data Analyst profession and closely associated roles. The study combines descriptive statistics, frequency analysis, data visualization, correlation analysis, and simple linear regression to identify patterns in compensation, company characteristics, industry distribution, and geographic concentration.

## Research Objectives

The analysis is designed to address the following questions:

1. What salary levels are most common for Data Analyst-related roles?
2. How are job opportunities distributed across industries, sectors, and locations?
3. What do company ratings and company-size distributions suggest about the market?
4. Is there evidence of association among company founding year, employee count, and annual revenue?

## Dataset Description

The dataset is imported from an Excel file (`Data.Analyst.xlsx`) and contains:

- **8 qualitative variables**
- **3 quantitative variables**

### Variables Used

| Variable | Type |
|---|---|
| `Job Title` | Qualitative |
| `Average Salary $` | Quantitative |
| `Rating` | Quantitative |
| `Company Name` | Qualitative |
| `Location` | Qualitative |
| `Headquarters` | Qualitative |
| `Number of employes` | Quantitative |
| `Founded` | Quantitative |
| `Industry` | Qualitative |
| `Sector` | Qualitative |
| `Average Revenue $` | Quantitative |

## Methodology

The workflow implemented in `Analys.Rmd` follows these stages:

1. **Data loading and structure inspection** (`head`, `str`, `summary`)
2. **Univariate analysis** of salaries, ratings, employees, and revenue
3. **Categorical analysis** using contingency and frequency tables
4. **Visual analysis** through bar plots, scatter plots, pie charts, boxplots, density plots, and mosaic plots
5. **Multivariate analysis** using correlation matrices (`corrplot`, `ggpairs`) and a simple linear regression model (`lm`)

## Software and Packages

The analysis is implemented in **R** with the following libraries:

`dplyr`, `tidyr`, `ggplot2`, `knitr`, `ggpubr`, `readr`, `readxl`, `esquisse`, `corrplot`, `GGally`

## Principal Findings

- Mean salary is approximately **$71,418**, with observed values ranging from **$33,500** to **$150,000**.
- Mean company rating is approximately **3.739/5**, suggesting generally positive employer evaluations.
- The role **Data Analyst** appears with high frequency in the sample.
- **IT Services** is among the most represented industries.
- A strong geographic concentration is observed in **New York**.
- Company founding years are notably concentrated in the period **1980–2005**.

## Reproducibility

To reproduce the analysis:

1. Open `Analys.Rmd` in RStudio or VS Code (with R support).
2. Install any missing packages listed above.
3. Ensure the dataset path points to the local location of `Data.Analyst.xlsx`.
4. Run all code chunks or knit the notebook to generate updated output.

## Repository Contents

- `Analys.Rmd` — source analysis document (R Markdown)
- `Analys.nb.html` — rendered notebook output
- `README.md` — project overview
- `LICENSE` — license file

## Notes

- The current script references an absolute dataset path; replacing it with a relative project path is recommended for portability.
- The original analysis narrative is written in Albanian; this README provides an academic English summary for wider accessibility.
