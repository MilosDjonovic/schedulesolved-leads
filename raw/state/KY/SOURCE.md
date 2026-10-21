# KY — state education directory sources

Agency: Kentucky Department of Education (KDE) — Open House, District and School Directory

Download date: 2026-10-21

openhouse.education.ky.gov serves an incomplete TLS certificate chain (curl: 'unable to get local issuer certificate'), so it was used through headless Chromium, which completes the chain; TLS verification was not disabled. The /Principals and /Superintendents pages have "Export to Excel" buttons (client-side export of the full list); both were clicked. **No email addresses** are published (names, phone, fax, address only). KDE's nonpublic list ("KBE Certified Non-Public Schools List" PDF on www.education.ky.gov) returned HTTP 403 to curl and did not load in the headless browser; not saved.

## `OpenHouse_Principals.xlsx`

All public school principals with school/district codes, address, phone, fax, grades.

- URL: https://openhouse.education.ky.gov/Principals
- How obtained: Browser click on "Export to Excel" (download named Principals.xlsx).
- Size: 176,733 bytes
- Sheet: Data
- Data rows: 1,540
- Column count: 21
- Columns: `District Code`, `District Name`, `School Code`, `School Name`, `Principal First Name`, `Principal Last Name`, `Address Line 1`, `Address Line 2`, `City`, `State`, `Zipcode`, `Phone`, `Fax`, `Classification`, `Description`, `PSN_ROLE_CD`, `PSN_ROLE_STS_CD`, `role_code_desc`, `LOWGRADE`, `HIGHGRADE`, `Role Title`

## `OpenHouse_Superintendents.xlsx`

All district superintendents with website, address, phone, fax.

- URL: https://openhouse.education.ky.gov/Superintendents
- How obtained: Browser click on "Export to Excel" (download named Superintendents.xlsx).
- Size: 25,176 bytes
- Sheet: Data
- Data rows: 178
- Column count: 13
- Columns: `District Code`, `District Name`, `District Website`, `Superintendent First Name`, `Superintendent Last Name`, `Address Line 1`, `Address Line 2`, `City`, `State`, `Zipcode`, `Phone`, `Fax`, `Role Title`

## `NCESIDS_2025-26_Kentucky_NCES-ID_Codes.xlsx`

State district/school IDs ↔ NCES LEA/school IDs crosswalk.

- URL: https://openhouse.education.ky.gov/Home/Download
- How obtained: Direct link ("National Center for Education Statistics (NCES) ID Codes"), opened in headless Chromium.
- Size: 100,735 bytes
- Sheet: Sheet1
- Data rows: 1,561
- Column count: 8
- Columns: `District ID`, `School ID`, `District Name`, `LEA ID (STATE)`, `LEA NCES`, `SCHOOL ID (STATE)`, `SCHOOL NCES`, `SCHOOL Name`
