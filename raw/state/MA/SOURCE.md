# MA — state education directory sources

Agency: Massachusetts Department of Elementary and Secondary Education (DESE) — School and District Profiles, Search / Export

Download date: 2026-10-21

Files are Excel-flavoured HTML tables (server sends `application/excel`, filename search.xls) — saved unmodified with .xls extension; open in Excel or parse as HTML. The search page's export link uses `showEmail=N`; `showEmail=Y` was used to include the Email column. One row per organization with its primary contact (`Function` = Principal for schools, Superintendent for districts, Head of School / Director for private schools).

## `profiles_public_schools_principals.xls`

Public schools incl. charter (org types 6,13) with principal name and email (1,800 of 1,801 rows have email).

- URL: https://profiles.doe.mass.edu/search/search_export.aspx?orgCode=&orgType=6,13&runOrgSearch=Y&searchType=0&leftNavId=11238&showEmail=Y
- How obtained: Direct export link (the export icon on the search results of https://profiles.doe.mass.edu/search/search.aspx?leftNavId=11238 with Organization Type = Public School), showEmail switched to Y.
- Size: 688,039 bytes
- Data rows: 1,801
- Column count: 14
- Columns: `Org Name`, `Org Code`, `Org Type`, `Function`, `Contact Name`, `Address 1`, `Address 2`, `Town`, `State`, `Zip`, `Phone`, `Fax`, `Email`, `Grade`

## `profiles_districts_superintendents.xls`

Districts (incl. charter districts) with superintendent name and email.

- URL: https://profiles.doe.mass.edu/search/search_export.aspx?orgCode=&orgType=5,12&runOrgSearch=Y&searchType=0&leftNavId=11238&showEmail=Y
- How obtained: Same export, Organization Type = Public School District (5,12).
- Size: 201,205 bytes
- Data rows: 517
- Column count: 14
- Columns: `Org Name`, `Org Code`, `Org Type`, `Function`, `Contact Name`, `Address 1`, `Address 2`, `Town`, `State`, `Zip`, `Phone`, `Fax`, `Email`, `Grade`

## `profiles_private_schools.xls`

Private schools with head/contact name and email.

- URL: https://profiles.doe.mass.edu/search/search_export.aspx?orgCode=&orgType=11&runOrgSearch=Y&searchType=0&leftNavId=11238&showEmail=Y
- How obtained: Same export, Organization Type = Private Schools (11).
- Size: 176,823 bytes
- Data rows: 438
- Column count: 13
- Columns: `Org Name`, `Org Code`, `Org Type`, `Function`, `Contact Name`, `Address 1`, `Address 2`, `Town`, `State`, `Zip`, `Phone`, `Fax`, `Email`

## `profiles_charter_schools.xls`

Charter public schools (subset of the public schools file).

- URL: https://profiles.doe.mass.edu/search/search_export.aspx?orgCode=&orgType=13&runOrgSearch=Y&searchType=0&leftNavId=11238&showEmail=Y
- How obtained: Same export, Organization Type = Charter Public School (13).
- Size: 32,446 bytes
- Data rows: 72
- Column count: 14
- Columns: `Org Name`, `Org Code`, `Org Type`, `Function`, `Contact Name`, `Address 1`, `Address 2`, `Town`, `State`, `Zip`, `Phone`, `Fax`, `Email`, `Grade`
