# ME — state education directory sources

Agency: Maine Department of Education — NEO Contact Search (SuperSearch) and Schools/SAU organizational data

Download date: 2026-10-21

NEO contact data is entered by districts in NEO Staff; the public Contact Search needs no account. On https://neo.maine.gov/DOE/neo/Supersearch/ContactSearch/StaffSearchByNonTeachingPosition the form was submitted with SAU = "Select All", positions Principal (68), Teaching Principal (89), Superintendent of Schools (80), Asst Superintendent of Schools (7), and the **Export to Excel** button (`action:NonTeachingPositionTypeExport`); request replicated with curl (GET page for antiforgery token + cookie, then POST). The export is an Excel-flavoured HTML table (server filename SAUSearchResults.xls), saved unmodified. It covers public SAUs and private/approved schools listed in NEO. Organizational data workbook (SAU ↔ school IDs, no contacts) fetched via headless Chromium (maine.gov returned 403 to curl).

## `NEO_SAUSearchResults_principals_superintendents.xls`

Principals (557), teaching principals (27), superintendents (451) and assistant superintendents (73) with email, phone, address.

- URL: https://neo.maine.gov/DOE/neo/Supersearch/ContactSearch/StaffSearchByNonTeachingPosition
- How obtained: Form POST replicating 'Export to Excel' (positions 68, 89, 80, 7; all SAUs).
- Size: 302,619 bytes
- Data rows: 1,108
- Column count: 12
- Columns: `Position`, `SAU Name`, `School`, `Last Name`, `First Name`, `Phone`, `Email`, `AddressLine1`, `AddressLine2`, `Town`, `State`, `Zip Code`

## `DATA_2026_Organizational_Data_SAUs_and_Schools_10.22.2025.xlsx`

2026 SAU and school organization list (IDs, types) — no contacts.

- URL: https://www.maine.gov/doe/sites/maine.gov.doe/files/inline-files/DATA%20-%202026%20Organizational%20Data%20SAUs%20and%20Schools%20-%2010.22.2025.xlsx
- How obtained: Direct link ("All SAUs and Schools") from https://maine.gov/doe/data-reporting/SchoolsSAU , via headless Chromium.
- Size: 58,770 bytes
- Sheet: Metadata
- Data rows: 16
- Column count: 3
- Columns: `Data Request`, `:`, `2026 SAU and School organization list`
- Sheet: Data Table
- Data rows: 738
- Column count: 7
- Columns: `Year Code`, `Public Flag`, `SAU Id`, `SAU Name`, `School Id`, `School Name`, `School Type`
