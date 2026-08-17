# Reproducibility Notes

## 1. Original SAS code is missing
The final report states that SAS was used for cleaning, analysis, confidence intervals, visualization, and geospatial outputs, but the original `.sas` program was not included in the supplied project files.

**Action for final correction pass:** locate the original SAS program or any SAS Enterprise Guide/project file and add it under `code/`.

## 2. Original SAS binary dataset exceeds GitHub browser limits
`filtered_data.sas7bdat` is approximately 47.7 MB. It is not included in the upload-ready package. The portable consolidated CSV has been split into two year-based files instead.

**Action:** if Git LFS is later adopted or the SAS file is needed for exact replication, add it using an appropriate large-file strategy.

## 3. Consolidated CSV exceeds GitHub browser limits
The original `filtered_data.csv` is approximately 33.6 MB. It has been split into 2017-2019 and 2020-2022 parts without changing the schema.

## 4. Descriptive versus causal interpretation
The report links some observed changes to the ACA, Medicaid expansion, employer-sponsored insurance, and other policies. The retained artifacts document descriptive trend analysis rather than a causal research design.

**Action:** keep public-facing claims descriptive unless a causal specification is later documented.

## 5. Income-adjustment language should be verified
The report refers to household income adjusted for inflation and regional variation, but the exact transformation code is unavailable because the SAS program is missing.

**Action:** verify how income categories or adjustments were implemented in the original analysis before making a technical claim about inflation or regional cost-of-living adjustment.

## 6. Missing-data treatment is not fully documented
The report states that incomplete or missing data were accounted for, but the exact rule cannot be verified without the SAS code.

**Action:** recover or reconstruct the original missing-data rule and document it.

## 7. Coauthor/publication permissions
The final report is coauthored. Confirm that public display of the complete PDF is acceptable to the other authors.

## 8. Figure generation is not reproducible from source code yet
All tables/figures are preserved from the report, but the code used to generate them is unavailable.

**Publication position:** portfolio-ready with transparent reproducibility notes; not yet a code-complete replication repository.
