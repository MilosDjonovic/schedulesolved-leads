# WY — state education directory sources

Agency: Wyoming Department of Education (WDE) — WyEd Online Directory (public People Search)

Download date: 2026-10-21

WDE no longer posts an annual directory PDF (latest found is 2021-22). The public Online Directory (no sign-in needed for People Search) was used in headless Chromium: Role = Principal (63) / Superintendent (66), all organizations, Search, then the grid's **Export** button; downloads named PeopleExport.xlsx. Organization Id = WDE 7-digit district/school code. No private-school contact file (the directory's organization list includes some non-district organizations, but only role-holders in schools/districts appear under these two roles).

## `WyEd_OnlineDirectory_PeopleExport_Principal.xlsx`

All principals (346 rows; a principal may appear once per school served) with phone, email, school, district.

- URL: https://portals.edu.wyoming.gov/wyedpro/Pages/OnlineDirectory/OnlineDirectoryPeopleSearch.aspx
- How obtained: Browser: People Search, role Principal, Search → Export.
- Size: 56,429 bytes
- Sheet: People
- Data rows: 346
- Column count: 20
- Columns: `First Name`, `Last Name`, `Suffix`, `Phone`, `Email`, `Title`, `Organization Id`, `Organization Name`, `Grades Served`, `Parent Id`, `Parent Name`, `Physical Address`, `Physical State`, `Physical Zip`, `Physical Zip Ext`, `Mailing Address`, `Mailing City`, `Mailing State`, `Mailing Zip`, `Mailing Zip Ext`

## `WyEd_OnlineDirectory_PeopleExport_Superintendent.xlsx`

District superintendents (52) with phone, email.

- URL: https://portals.edu.wyoming.gov/wyedpro/Pages/OnlineDirectory/OnlineDirectoryPeopleSearch.aspx
- How obtained: Browser: People Search, role Superintendent, Search → Export.
- Size: 12,569 bytes
- Sheet: People
- Data rows: 52
- Column count: 20
- Columns: `First Name`, `Last Name`, `Suffix`, `Phone`, `Email`, `Title`, `Organization Id`, `Organization Name`, `Grades Served`, `Parent Id`, `Parent Name`, `Physical Address`, `Physical State`, `Physical Zip`, `Physical Zip Ext`, `Mailing Address`, `Mailing City`, `Mailing State`, `Mailing Zip`, `Mailing Zip Ext`
