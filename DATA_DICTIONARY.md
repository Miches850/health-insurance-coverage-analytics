# Data Dictionary and File Guide

## Raw annual files
Each `ACSST5Y<YEAR>.S2701-Data.csv` file is an original ACS S2701 export. The first row contains Census variable codes and the second row contains descriptive labels. The original files contain 613 columns.

Approximate row counts excluding the header row:
- 2017: 3,221
- 2018: 3,221
- 2019: 3,221
- 2020: 3,222
- 2021: 3,222
- 2022: 3,223

## Column metadata
`ACSST5Y.S2701-Column-Metadata.xlsx` is retained as the supplied Census metadata workbook.

## Derived data
The consolidated filtered dataset contains 18,679 observations and 310 columns. It begins with identifying fields such as `s_name`, `year`, `GEO_ID`, and `NAME`, followed by selected S2701 estimate fields.

The derived CSV is split into two parts only to satisfy GitHub's browser-upload limit; the schema is unchanged.

## Primary analytical concepts
The final report groups the ACS fields into:
- insured versus uninsured totals;
- age categories;
- disability categories;
- education categories;
- work-experience categories;
- household-income categories;
- ratio-of-income-to-poverty categories.
