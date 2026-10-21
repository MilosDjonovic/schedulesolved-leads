# OH — state education directory sources

Agency: Ohio Department of Education and Workforce — OEDS (Ohio Educational Directory System), Public Extract Data

Download date: 2026-10-21

Each CSV starts with a one-line preamble `Generated on <timestamp>` before the header row (kept unmodified). IRN values are written as Excel formulas (`="200001"`). Values that are missing are the literal `N/A`. School file fill rates: principal name 5,030 / 5,321, principal email 3,041, org email 3,110; 905 rows are Nonpublic School (private schools with principal contacts). Request body used for each file (form field `jsonData`): `{"OrgTypes":[...],"OrgCats":[...],"Selected":[all 24 available fields]}`; org type IDs come from https://oeds.education.ohio.gov/Api/generalPage/RefOrgDetailsExtract. Selecting multiple categories in one request returns only the first category, so each category was requested separately.

## `OEDS_extract_schools.csv`

All schools (public, community/charter, nonpublic, STEM, vocational) with principal name/email/phone, superintendent, treasurer, parent district IRN.

- URL: https://oeds.education.ohio.gov/DataExtract/GetRequestOrgExtract
- How obtained: Form POST (the 'Generate Report' button on https://oeds.education.ohio.gov/DataExtract), category School (2), types [60,5,6,7,45,46,48] = STEM, Nonpublic School, Public Community School, Traditional Public School, Vocational School, Night/Adult School, Special Ungraded. Server filename Data.csv.
- Size: 1,904,456 bytes
- Data rows: 5,321
- Column count: 24
- Columns: `IRN`, `ORGANIZATION NAME`, `SCHOOL TYPE`, `GRADE SPAN`, `ORGANIZATION TYPE`, `ORGANIZATION CATEGORY`, `STATUS`, `DESIGNATED COUNTY`, `WEB URL`, `ORG EMAIL ADDRESS`, `ORG MAILING ADDRESS`, `ORG PHONE`, `ORG FAX`, `SUPERINTENDENT`, `SUPERINTENDENT EMAIL`, `SUPERINTENDENT PHONE`, `TREASURER`, `TREASURER EMAIL`, `TREASURER PHONE`, `PRINCIPAL`, `PRINCIPAL EMAIL`, `PRINCIPAL PHONE`, `PARENT IRN`, `PARENT ORGANIZATION NAME`

## `OEDS_extract_districts.csv`

Districts (traditional public, nonpublic, JVSD, CTPD, tech prep) with superintendent and treasurer name/email/phone.

- URL: https://oeds.education.ohio.gov/DataExtract/GetRequestOrgExtract
- How obtained: Form POST, category District (1), types [1,2,3,4,70].
- Size: 284,353 bytes
- Data rows: 778
- Column count: 24
- Columns: `IRN`, `ORGANIZATION NAME`, `SCHOOL TYPE`, `GRADE SPAN`, `ORGANIZATION TYPE`, `ORGANIZATION CATEGORY`, `STATUS`, `DESIGNATED COUNTY`, `WEB URL`, `ORG EMAIL ADDRESS`, `ORG MAILING ADDRESS`, `ORG PHONE`, `ORG FAX`, `SUPERINTENDENT`, `SUPERINTENDENT EMAIL`, `SUPERINTENDENT PHONE`, `TREASURER`, `TREASURER EMAIL`, `TREASURER PHONE`, `PRINCIPAL`, `PRINCIPAL EMAIL`, `PRINCIPAL PHONE`, `PARENT IRN`, `PARENT ORGANIZATION NAME`

## `OEDS_extract_service_centers.csv`

Educational Service Centers and other regional service orgs with superintendent contacts.

- URL: https://oeds.education.ohio.gov/DataExtract/GetRequestOrgExtract
- How obtained: Form POST, category Service Center (7), types [21,22,23,24,25,67].
- Size: 32,650 bytes
- Data rows: 96
- Column count: 24
- Columns: `IRN`, `ORGANIZATION NAME`, `SCHOOL TYPE`, `GRADE SPAN`, `ORGANIZATION TYPE`, `ORGANIZATION CATEGORY`, `STATUS`, `DESIGNATED COUNTY`, `WEB URL`, `ORG EMAIL ADDRESS`, `ORG MAILING ADDRESS`, `ORG PHONE`, `ORG FAX`, `SUPERINTENDENT`, `SUPERINTENDENT EMAIL`, `SUPERINTENDENT PHONE`, `TREASURER`, `TREASURER EMAIL`, `TREASURER PHONE`, `PRINCIPAL`, `PRINCIPAL EMAIL`, `PRINCIPAL PHONE`, `PARENT IRN`, `PARENT ORGANIZATION NAME`
