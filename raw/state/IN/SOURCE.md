# IN — state education directory sources

Agency: Indiana Department of Education (IDOE) — Indiana School Directory

Download date: 2026-10-21

Workbook with three sheets: CORP (school corporations/districts and charters, superintendent name + email), SCHL (public schools, principal name + email), NPSCHL (nonpublic/private schools, principal name + email, Choice scholarship flag). The suggested ArcGIS service https://gis.dhs.in.gov/arcgis/rest/services/Open/SchoolsOpen (MapServer and FeatureServer) was tried on 2026-10-21 and returned `500 GISService not instantiated` for every request, so it was not used; the IDOE file covers the same contact fields.

## `2025-2026-school-directory-2026-03-23.xlsx`

Indiana School Directory 2025-26 (version dated 2026-03-23).

- URL: https://www.in.gov/doe/files/2025-2026-school-directory-2026-03-23.xlsx
- How obtained: Direct link ("2025-2026 Indiana School Directory") from https://www.in.gov/doe/it/data-center-and-reports/
- Size: 447,924 bytes
- Sheet: CORP
- Data rows: 460
- Column count: 17
- Columns: `NCES_ID`, `IDOE_CORPORATION_ID`, `CORPORATION_NAME`, `CORPORATION_TYPE`, `SUPERINTENDENT_FIRST_NAME`, `SUPERINTENDENT_LAST_NAME`, `SUPERINTENDENT_EMAIL`, `ADDRESS`, `CITY`, `STATE`, `ZIP`, `COUNTY_NAME`, `PHONE`, `FAX`, `LOW_GRADE`, `HIGH_GRADE`, `CORPORATION_HOMEPAGE`
- Sheet: SCHL
- Data rows: 1,962
- Column count: 19
- Columns: `NCES_ID`, `IDOE_CORPORATION_ID`, `CORPORATION_NAME`, `IDOE_SCHOOL_ID`, `SCHOOL_NAME`, `PRINCIPAL_FIRST_NAME`, `PRINCIPAL_LAST_NAME`, `PRINCIPAL_EMAIL`, `ADDRESS`, `CITY`, `STATE`, `ZIP`, `LOCALE`, `COUNTY_NAME`, `PHONE`, `FAX`, `LOW_GRADE`, `HIGH_GRADE`, `SCHOOL_HOMEPAGE`
- Sheet: NPSCHL
- Data rows: 420
- Column count: 17
- Columns: `IDOE_SCHOOL_ID`, `SCHOOL_NAME`, `PRINCIPAL_FIRST_NAME`, `PRINCIPAL_LAST_NAME`, `PRINCIPAL_EMAIL`, `ADDRESS`, `CITY`, `STATE`, `ZIP`, `COUNTY_NAME`, `PHONE`, `FAX`, `LOW_GRADE`, `HIGH_GRADE`, `SCHOOL_HOMEPAGE`, `CHOICE_FLAG`, `COMMISSION`
