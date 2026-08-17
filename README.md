# Health Insurance Coverage Analytics
## U.S. County-Level Coverage Trends, 2017-2022

**ECMT 673 - Economic Analytics | SAS / U.S. Census ACS data**

## Project overview

This project analyzes U.S. county-level health-insurance coverage from 2017 through 2022 using American Community Survey S2701 data. The analysis compares insured and uninsured populations across age, disability status, educational attainment, work experience, household income, and poverty-level categories, and supplements national trend analysis with county-level geographic heat maps.

The submitted report describes a SAS-based workflow for data cleaning, descriptive statistics, confidence intervals, trend visualization, and geographic analysis. The repository preserves the original Census source files, a derived analysis dataset split into GitHub-uploadable parts, the complete final report, and the report's tables and figures.

## Research focus

The project asks how health-insurance coverage differs across major socioeconomic and demographic groups and how those disparities changed between 2017 and 2022.

## Data

The repository includes the six annual ACS 5-year S2701 county-level extracts used for the project:

- 2017
- 2018
- 2019
- 2020
- 2021
- 2022

Each annual raw file contains more than 3,200 geographic rows and 613 columns in the original Census export format. A consolidated derived dataset contains 18,679 observations and 310 selected fields.

Because the original consolidated CSV and SAS dataset exceed GitHub's browser-upload limit, the derived CSV is split into:

- `filtered_data_2017_2019.csv`
- `filtered_data_2020_2022.csv`

The original 47+ MB `filtered_data.sas7bdat` is not included because the smaller derived CSV files preserve the portable analysis data needed for a public portfolio repository.

## Analytical dimensions

The submitted report examines:

- **Age:** under 19, 19-64, and 65+
- **Disability status:** with and without disability
- **Educational attainment:** less than high school through bachelor's degree or higher
- **Work experience:** did not work, part-time, and full-time
- **Income:** under $25,000 through $100,000+
- **Poverty ratio:** below 100%, below 138%, 138%-399%, and 400%+
- **Geography:** county-level insured and uninsured distributions across the United States

## Methods represented in the submitted project

- multi-year Census data compilation
- county-level data filtering and preparation
- SAS-based descriptive statistics
- mean and standard-deviation summaries
- 95% confidence intervals for means
- insured/uninsured subgroup comparisons
- year-over-year trend visualization
- dual-axis charts
- county-level heat-map analysis
- policy-oriented interpretation of coverage gaps

## Selected findings reported in the project

The submitted report highlights several recurring patterns:

1. Working-age adults ages 19-64 exhibited the largest uninsured coverage gap relative to children and adults age 65+.
2. Higher educational attainment was associated with stronger insurance coverage, while lower educational attainment was associated with larger uninsured populations.
3. Full-time workers maintained stronger coverage than part-time workers and people who did not work.
4. Higher-income groups showed substantially greater coverage and lower uninsured counts than lower-income groups.
5. Insured populations generally increased and uninsured populations generally declined across the 2017-2022 period, while important socioeconomic disparities persisted.

These statements summarize the submitted report and should be interpreted as descriptive findings, not causal estimates.

## Selected figures

### Coverage by income level

![Insured population by income](figures/figure_10_insured_by_income.png)

![Uninsured population by income](figures/figure_11_uninsured_by_income.png)

### County-level geographic patterns

![Insured county heatmaps](figures/appendix_B1_insured_county_heatmaps.png)

![Uninsured county heatmaps](figures/appendix_B2_uninsured_county_heatmaps.png)

## Repository structure

```text
3_health-insurance-coverage-analytics/
├── README.md
├── .gitignore
├── LICENSE_REPOSITORY_DOCS.txt
├── code/
│   └── README.md
├── data/
│   ├── raw/
│   │   ├── ACSST5Y2017.S2701-Data.csv
│   │   ├── ...
│   │   ├── ACSST5Y2022.S2701-Data.csv
│   │   └── ACSST5Y.S2701-Column-Metadata.xlsx
│   └── derived/
│       ├── filtered_data_2017_2019.csv
│       ├── filtered_data_2020_2022.csv
│       └── README.md
├── figures/
├── report/
│   └── Health_Insurance_Coverage_Analytics_Final_Report.pdf
├── docs/
│   ├── PROJECT_SUMMARY.md
│   ├── METHODOLOGY_SUMMARY.md
│   ├── DATA_DICTIONARY.md
│   ├── REPRODUCIBILITY_NOTES.md
│   └── GITHUB_UPLOAD_GUIDE.md
└── outputs/
    └── README.md
```

## Reproducibility status

**Portfolio-ready, but not fully reproducible from code yet.**

The original SAS program used to clean, analyze, and visualize the data was not supplied with the current project files. The repository therefore does **not** fabricate replacement SAS code. The report, original annual Census files, derived data, tables, and figures are preserved as evidence of the completed analysis. If the original `.sas` program is later recovered, it should be added under `code/` and the reproducibility status updated.

See `docs/REPRODUCIBILITY_NOTES.md` for the final correction items.

## Authorship

The submitted report lists **Michael Shannon, Taylor Molina, Shayan Esani, Rabin Mishra, and Reagan Mathai** as project authors. The report is retained as the original academic artifact.

## Suggested GitHub topics

`sas` `health-insurance` `census-data` `american-community-survey` `data-analysis` `public-policy` `healthcare-analytics` `descriptive-statistics` `data-visualization`
